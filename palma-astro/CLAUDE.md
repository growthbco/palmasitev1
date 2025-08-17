# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Palma Cleaning Co. website - A professional cleaning services website built with Astro framework. The site is deployed at https://palmacleaningco.com and serves multiple service areas in Florida including The Villages, Oak Run, Stone Creek, and surrounding areas.

## Technology Stack

- **Framework**: Astro (v5.12.9)
- **Languages**: Astro components, HTML, CSS, JavaScript
- **Deployment**: Netlify
- **Package Manager**: npm

## Common Commands

```bash
# Install dependencies
npm install

# Start development server (runs on localhost:4321)
npm run dev

# Build for production (outputs to ./dist/)
npm run build

# Preview production build locally
npm run preview
```

## Project Structure

```
palma cleaning/
├── src/
│   ├── pages/           # Astro page components (routes)
│   │   ├── index.astro  # Homepage
│   │   ├── services.astro
│   │   ├── [location].astro files for different service areas
│   │   └── [service-type].astro files for different cleaning services
│   └── components/      # Reusable Astro components
│       └── Navigation.astro
├── public/             # Static assets served directly
│   ├── images/         # Image assets
│   ├── styles.css      # Global styles
│   ├── script.js       # Client-side JavaScript
│   └── *.html          # Pre-built HTML pages
└── netlify.toml        # Netlify deployment configuration
```

## Key Service Areas

The site covers multiple locations with dedicated pages:
- The Villages
- Oak Run
- Stone Creek
- Belleview
- Golden Hills
- WEC Area (World Equestrian Center)
- Ocala
- Dunnellon

## Service Types

Each location typically offers:
- Standard Cleaning
- Deep Cleaning
- Move In/Out Cleaning
- Post-Construction Cleaning
- Commercial Cleaning
- Equestrian Facility Cleaning

## Development Guidelines

1. **Page Creation**: New pages go in `src/pages/` and are automatically routed based on filename
2. **Static Assets**: Place images and other static files in `public/`
3. **Components**: Reusable components belong in `src/components/`
4. **Styling**: Global styles are in `public/styles.css`
5. **SEO**: The site uses location-specific pages for better local SEO

## Deployment

- Site is deployed on Netlify
- Production domain: https://palmacleaningco.com
- Redirects are configured to consolidate traffic to the apex domain