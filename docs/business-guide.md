# Framer Template Business Guide

A comprehensive reference for building and selling Framer templates using Claude as your design partner.

---

## Table of Contents

1. [Business Model Overview](#business-model-overview)
2. [Template Creation Workflow](#template-creation-workflow)
3. [Template Categories & Ideas](#template-categories--ideas)
4. [Pricing Strategy](#pricing-strategy)
5. [Where to Sell](#where-to-sell)
6. [Marketing Your Templates](#marketing-your-templates)
7. [Design Prompts Library](#design-prompts-library)
8. [Framer Recreation Tips](#framer-recreation-tips)
9. [Quality Checklist](#quality-checklist)
10. [Revenue Goals Tracker](#revenue-goals-tracker)

---

## Business Model Overview

### The Process

```
Claude generates design → You preview HTML → Recreate in Framer → Sell template
```

### Why This Works

- **Speed**: Claude generates production-quality designs in minutes
- **Variety**: Each generation is unique with distinctive aesthetic choices
- **Quality**: The `/frontend-design` skill ensures polished, non-generic output
- **Scalability**: Generate 5-10 concepts daily, pick the best to recreate

### Revenue Potential

| Templates | Avg Price | Monthly Sales | Monthly Revenue |
|-----------|-----------|---------------|-----------------|
| 5         | $49       | 20            | $980            |
| 10        | $49       | 40            | $1,960          |
| 20        | $59       | 80            | $4,720          |
| 50        | $69       | 150           | $10,350         |

---

## Template Creation Workflow

### Step 1: Ideation

Decide on:
- **Category**: SaaS, Agency, E-commerce, Portfolio, etc.
- **Niche**: AI tools, fintech, health tech, creative agencies, etc.
- **Style**: Minimal, bold, playful, luxurious, brutalist, etc.

### Step 2: Generate with Claude

Use the `/frontend-design` skill with a detailed prompt:

```
Create a landing page for [type of business].

Target audience: [who will use this]
Style: [aesthetic direction]
Key sections: hero, features, pricing, testimonials, CTA
Special requests: [animations, dark mode, specific colors, etc.]
```

### Step 3: Preview & Iterate

1. Save the HTML output to `templates/[category]/[name].html`
2. Open in browser to preview
3. Ask Claude for variations or refinements
4. Pick the best version

### Step 4: Recreate in Framer

1. Open Framer and create new project
2. Rebuild the layout section by section
3. Add Framer-specific interactions and animations
4. Set up responsive breakpoints
5. Add CMS collections if needed

### Step 5: Package & Publish

1. Add preview images and thumbnails
2. Write compelling description
3. Set pricing
4. Publish to marketplace(s)

---

## Template Categories & Ideas

### High-Demand Categories

| Category | Examples | Price Range |
|----------|----------|-------------|
| **SaaS Landing Pages** | AI tools, productivity apps, dev tools | $49-99 |
| **Agency Sites** | Creative, marketing, design agencies | $59-129 |
| **Portfolio** | Designers, developers, photographers | $39-79 |
| **E-commerce** | Product pages, storefronts | $69-149 |
| **Startup** | Pitch decks, coming soon, waitlists | $29-59 |
| **Blog/Content** | Writers, creators, newsletters | $39-69 |

### Niche Ideas (Less Competition)

- AI/ML product landing pages
- Fintech and banking apps
- Health and wellness platforms
- Developer tools and APIs
- Climate/sustainability startups
- NFT and Web3 projects
- Podcast and creator sites
- Real estate platforms
- Legal and consulting firms
- Restaurant and hospitality

### Template Bundle Ideas

- "SaaS Starter Pack" (5 templates) - $199
- "Agency Bundle" (3 templates + components) - $149
- "Dark Mode Collection" (5 templates) - $179
- "Minimal Series" (4 templates) - $159

---

## Pricing Strategy

### Factors That Increase Value

- Multiple pages (not just landing page)
- CMS integration
- Complex animations/interactions
- Responsive design across all breakpoints
- Dark + light mode variants
- Documentation included
- Figma source file included

### Pricing Tiers

| Tier | What's Included | Price Range |
|------|-----------------|-------------|
| **Basic** | Single landing page | $29-49 |
| **Standard** | Multi-page + CMS | $59-89 |
| **Premium** | Full site + advanced features | $99-149 |
| **Bundle** | Multiple templates | $149-299 |

### Pricing Psychology

- Use $49 instead of $50 (charm pricing)
- Offer bundles at perceived discount
- Limited-time launch pricing creates urgency
- Compare value to hiring a designer ($500-2000)

---

## Where to Sell

### Primary Platforms

| Platform | Commission | Pros | Cons |
|----------|------------|------|------|
| **Framer Marketplace** | 30% | Built-in traffic, trusted | High competition |
| **Gumroad** | 10% | Low fees, easy setup | Need own traffic |
| **Lemonsqueezy** | 5-8% | Low fees, good analytics | Need own traffic |
| **Your Own Site** | 0% | Full control, all profit | Need traffic + payments |

### Secondary Channels

- **Creative Market** - General design marketplace
- **UI8** - Premium UI resources
- **Envato Elements** - Subscription model
- **ProductHunt** - Launch new templates
- **Twitter/X** - Build audience, share previews

### Multi-Platform Strategy

1. Launch on Framer Marketplace (built-in traffic)
2. Sell direct via Gumroad (higher margins)
3. Use Twitter/X to drive direct sales
4. Build email list for launches

---

## Marketing Your Templates

### Content Strategy

Use these skills for marketing:
- `/copywriting` - Template descriptions, landing pages
- `/social-content` - Twitter/X posts, LinkedIn
- `/launch-strategy` - ProductHunt launches
- `/content-strategy` - Blog posts, tutorials

### Marketing Channels

**Twitter/X (Primary)**
- Share design process videos/GIFs
- Post before/after comparisons
- Engage with Framer community
- Use #FramerTemplates, #WebDesign

**YouTube/Loom**
- Template walkthrough videos
- "How I designed this" process
- Framer tutorial content

**Email List**
- New template announcements
- Exclusive discounts
- Design tips and insights

### Launch Playbook

1. **Pre-launch** (1 week before)
   - Tease design on Twitter
   - Build anticipation
   - Collect emails

2. **Launch Day**
   - Post on ProductHunt
   - Twitter thread with details
   - Email announcement
   - Limited-time discount (20% off)

3. **Post-launch**
   - Share customer testimonials
   - Create tutorial content
   - Answer questions publicly

---

## Design Prompts Library

Copy these prompts and customize for your needs:

### SaaS Landing Pages

```
Create a SaaS landing page for an AI writing assistant.
Target: Content marketers and copywriters
Style: Modern, clean, with subtle gradients
Sections: Hero with demo, features grid, pricing table, testimonials, CTA
Colors: Deep purple primary, light backgrounds
```

```
Create a landing page for a developer API platform.
Target: Backend developers and startups
Style: Dark theme, terminal-inspired, technical
Sections: Hero with code snippet, features, documentation preview, pricing
Include: Syntax highlighting, monospace fonts
```

### Agency Sites

```
Create a creative agency homepage.
Target: Tech startups looking for branding
Style: Bold, artistic, lots of white space
Sections: Hero with showreel, case studies grid, services, team, contact
Animations: Smooth scroll reveals, hover effects on projects
```

### E-commerce

```
Create a product landing page for premium headphones.
Target: Audiophiles and music producers
Style: Luxurious, dark, cinematic
Sections: Hero with product shot, features, specs, reviews, purchase CTA
Effects: Parallax scrolling, product rotation on scroll
```

### Portfolio

```
Create a portfolio site for a UX designer.
Target: Tech companies hiring designers
Style: Minimal, elegant, generous whitespace
Sections: Brief intro, project gallery, about, contact
Typography: Sophisticated serif headings, clean sans body
```

---

## Framer Recreation Tips

### Matching the Design

1. **Typography**
   - Note exact font families from the HTML
   - Match font sizes, weights, line heights
   - Use Framer's Google Fonts integration

2. **Colors**
   - Extract CSS variables/colors from the code
   - Create a color palette in Framer
   - Use color styles for consistency

3. **Spacing**
   - Pay attention to padding and margins
   - Use Framer's spacing system
   - Keep consistent rhythm

4. **Animations**
   - Note CSS transition/animation properties
   - Recreate with Framer's animation tools
   - Use scroll-triggered animations

### Framer-Specific Enhancements

- Add CMS collections for dynamic content
- Create component variants for reusability
- Set up responsive breakpoints (desktop, tablet, mobile)
- Add Framer-native interactions (hover, click, scroll)
- Include page transitions

### Common Gotchas

- Framer handles fonts differently - test loading
- Complex CSS animations may need simplification
- SVG imports sometimes need cleanup
- Test on actual devices, not just preview

---

## Quality Checklist

Before publishing any template:

### Design Quality
- [ ] Distinctive, non-generic aesthetic
- [ ] Consistent typography system
- [ ] Cohesive color palette
- [ ] Professional imagery/placeholders
- [ ] Balanced whitespace

### Technical Quality
- [ ] Responsive on all breakpoints
- [ ] Animations are smooth (60fps)
- [ ] All links/buttons work
- [ ] Forms are functional
- [ ] Fast loading

### Marketplace Ready
- [ ] Compelling thumbnail image
- [ ] Clear, benefit-focused description
- [ ] Preview images for all pages
- [ ] Accurate category/tags
- [ ] Fair, competitive price

### Documentation
- [ ] Setup instructions
- [ ] Font list
- [ ] Color palette reference
- [ ] Customization tips

---

## Revenue Goals Tracker

Use this to set and track your goals:

### Monthly Goals

| Month | Templates Created | Revenue Target | Actual |
|-------|-------------------|----------------|--------|
| Month 1 | 3 | $200 | |
| Month 2 | 5 | $500 | |
| Month 3 | 5 | $1,000 | |
| Month 4 | 4 | $1,500 | |
| Month 5 | 4 | $2,000 | |
| Month 6 | 4 | $2,500 | |

### Key Metrics to Track

- Templates published (total)
- Monthly revenue
- Best-selling template
- Average sale price
- Conversion rate (views to sales)
- Customer reviews/ratings
- Refund rate

### Milestones

- [ ] First template published
- [ ] First sale
- [ ] $100 in revenue
- [ ] 5 templates live
- [ ] $500/month
- [ ] 10 templates live
- [ ] $1,000/month
- [ ] First 5-star review
- [ ] Featured on marketplace
- [ ] $2,500/month
- [ ] 25 templates live
- [ ] $5,000/month

---

## Quick Reference

### Skills to Use

| Task | Skill |
|------|-------|
| Generate designs | `/frontend-design` |
| Write descriptions | `/copywriting` |
| Plan launches | `/launch-strategy` |
| Price templates | `/pricing-strategy` |
| Social media posts | `/social-content` |
| Optimize pages | `/page-cro` |

### Daily Workflow

1. Generate 2-3 design concepts
2. Pick the best one to recreate
3. Spend 2-3 hours in Framer
4. Post preview on Twitter
5. Publish when ready

### Weekly Tasks

- [ ] Publish 1-2 new templates
- [ ] Engage on Twitter (30 min/day)
- [ ] Respond to customer questions
- [ ] Analyze sales data
- [ ] Plan next week's templates

---

*Last updated: February 2026*
