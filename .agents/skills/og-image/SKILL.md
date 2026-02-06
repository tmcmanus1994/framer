---
name: og-image
description: This skill should be used when the user wants to generate Open Graph (OG) images for Nuxt pages. It discovers pages from app/pages/, identifies which are missing OG images, generates beautiful HTML designs, converts them to PNG via html2png.dev API, and saves them to public/og-images/. Trigger phrases include "generate og image", "create og images", "make social preview", "og-image", or "/og-image".
---

# OG Image Generator

Generate Open Graph images for Nuxt pages with consistent, high-quality designs.

## Workflow

### Step 1: Discover Pages

Scan `app/pages/` directory for Vue files to identify available pages:

```bash
find app/pages -name "*.vue" -type f
```

**Filtering rules:**
- Skip dynamic routes containing `[` brackets (e.g., `[...slug].vue`, `[category].vue`)
- Skip blog-specific pages in `blog/` directory (they have separate OG handling)
- Exception: Can generate one generic blog OG if requested

### Step 2: Check for Missing OG Images

For each discovered page, derive the slug and check if OG image exists:

| Page Path | Slug | OG Image Path |
|-----------|------|---------------|
| `app/pages/index.vue` | `index` | `public/og-images/index.png` |
| `app/pages/about.vue` | `about` | `public/og-images/about.png` |
| `app/pages/pricing/index.vue` | `pricing` | `public/og-images/pricing.png` |
| `app/pages/blog/index.vue` | `blog` | `public/og-images/blog.png` |

Present the list of pages with missing OG images to the user and ask which one to generate.

### Step 3: Read Page Content

Read the selected page's Vue file to understand:
- Page purpose and content
- Key messaging or value propositions
- Any existing title/description meta tags

Also check for `docs/design-system.md` if present for brand guidelines (colors, fonts, style).

### Step 4: Generate OG Image HTML

Create a single-file HTML document optimized for 1200x630 dimensions:

**Template structure:**
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=1200, height=630">
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Inter', sans-serif; }
  </style>
</head>
<body>
  <div style="width: 1200px; height: 630px;" class="...">
    <!-- OG image content -->
  </div>
</body>
</html>
```

**Design guidelines:**
- Use Tailwind CSS for styling
- Use Google Fonts (Inter recommended as default)
- Fixed dimensions: 1200x630px
- Bold, readable typography (text should be visible in small thumbnails)
- Clean, professional layouts
- No glitch effects, no glow effects
- Include brand elements if design system is available
- Check existing html for other og-s if present, so that we can continue consistent og image generation

**Save HTML to:** `keep/og-images/<slug>.html`

Ensure the `keep/og-images/` directory exists before saving.

### Step 5: Convert HTML to PNG

Use the html2png.dev API to convert the HTML:

```bash
curl -X POST "https://html2png.dev/api/convert?width=1200&height=630&format=png&deviceScaleFactor=2" \
  -H "Content-Type: text/html" \
  --data-binary @keep/og-images/<slug>.html
```

The API returns JSON with a `url` field containing the generated image URL.

### Step 6: Download and Save PNG

Download the image from the returned URL and save to `public/og-images/<slug>.png`:

```bash
curl -o public/og-images/<slug>.png "<returned-url>"
```

Ensure the `public/og-images/` directory exists before saving.

### Step 7: Report Success

Inform the user:
- Which OG image was generated
- Path to the saved PNG
- Path to the preserved HTML source
- Reminder to add og:image meta tag to the page if not already present

## Directory Structure

```
project/
├── keep/
│   └── og-images/
│       └── <slug>.html    # Preserved HTML source
├── public/
│   └── og-images/
│       └── <slug>.png     # Generated OG images
```

## Meta Tag Integration

After generating an OG image, the page should include:

```vue
<script setup>
useSeoMeta({
  ogImage: '/og-images/<slug>.png',
  twitterCard: 'summary_large_image',
  twitterImage: '/og-images/<slug>.png',
})
</script>
```
