# CLAUDE.md

This file provides guidance to Claude Code when working with this Framer template business repository.

## Project Overview

This is a **Framer Template Business** workspace. The purpose is to use Claude to design and build high-quality website mockups and examples in code (HTML/CSS/JS, React, Vue, etc.) which will then be recreated as Framer templates to sell on the Framer marketplace and other platforms.

**Business Model:**
1. Generate distinctive website designs using Claude + the `/frontend-design` skill
2. Preview and refine the HTML/CSS output
3. Recreate the designs in Framer as templates
4. Sell on Framer Marketplace, Gumroad, or direct

## Installed Skills

This repo has 27 skills installed for design and marketing:

**Design:**
- `/frontend-design` - Create distinctive, production-grade UI designs
- `/og-image` - Generate Open Graph images for social previews

**Marketing (from coreyhaines31/marketingskills):**
- `/copywriting` - Write compelling marketing copy
- `/page-cro` - Optimize page conversions
- `/pricing-strategy` - Structure pricing and tiers
- `/launch-strategy` - Plan product launches
- `/content-strategy` - Plan content marketing
- See `.claude/skills/` for all 25 marketing skills

## Workflow

### Generating Template Designs

1. **Describe the template you want:**
   ```
   Create a SaaS landing page for a project management tool.
   Target: startup founders. Style: minimal, professional.
   ```

2. **Invoke the frontend-design skill:**
   ```
   /frontend-design
   ```

3. **Claude generates production-ready HTML/CSS** with:
   - Distinctive typography and color choices
   - Animations and micro-interactions
   - Responsive layouts
   - Polished visual details

4. **Save and preview** the output, then recreate in Framer

### Template Categories to Build

Consider building templates across these categories:
- SaaS / Startup landing pages
- Agency / Portfolio sites
- E-commerce / Product pages
- Blog / Content sites
- Personal / CV sites
- App download pages
- Coming soon / Waitlist pages

## Project Structure

```
framer/
├── CLAUDE.md              # This file - project context
├── .agents/skills/        # Universal skill definitions
├── .claude/skills/        # Claude Code skill symlinks
├── templates/             # Generated template designs (create as needed)
│   ├── saas/
│   ├── agency/
│   ├── ecommerce/
│   └── ...
├── assets/                # Shared assets (create as needed)
└── docs/                  # Business docs and guides
    └── business-guide.md  # Reference guide
```

## Quick Commands

```bash
# List all installed skills
ls -la .claude/skills/

# Generate a new template design
# Just describe what you want and invoke /frontend-design

# Generate OG images for marketing
# /og-image (for Nuxt projects)
```

## Tips for Best Results

1. **Be specific about the target audience** - "startup founders" vs "enterprise buyers" yields very different designs
2. **Specify a style direction** - minimal, bold, playful, luxurious, etc.
3. **Mention key sections** - hero, features, pricing, testimonials, CTA
4. **Request variations** - ask for 2-3 color/style options
5. **Use marketing skills** for copy - `/copywriting` for headlines and CTAs
