# Changelog

All notable changes to this project are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project uses [Semantic Versioning](https://semver.org/).

## [0.1.0] - 2026-10-07

First release of the Millennials website, a premium car detailing and coating studio site built with Next.js 16, React 19, Tailwind CSS 4 and TypeScript.

### Added

- **Home page** with hero, studio stats, service highlights, before/after showcase and calls to action.
- **Services**
  - Services overview, split into Major and Minor categories (`/services/major`, `/services/minor`).
  - Individual service pages (`/services/[slug]`) for Paint Protection Film, Graphene Coating, Ceramic Coating, Window Tint, Repaint and Repair, Interior Detail, Exterior Detail, Headlight Detail and Glass Detail.
- **Gallery** of before/after transformations grouped by service, with per-service detail pages (`/gallery/[slug]`) and an interactive before/after slider.
- **Videos** page with a video library linked to services.
- **Book Now** page with a booking form that sends the request through WhatsApp.
- **Location** page with address, opening hours, service areas and a Google Maps link.
- **Reviews** and **FAQ** pages (currently hidden from the menu).
- Custom 404 page.
- Shared layout: sticky header with dropdown navigation, mobile menu, footer, mobile "Book" bar and back-to-top button.
- Menu switchboard (`src/lib/menu.ts`): hiding a menu item also removes it from navigation and the sitemap, returns 404 for its page and hides links to it.
- Central business details and content in `src/lib/site.ts` (contact info, hours, stats, services, testimonials).
- Theme system (`src/lib/theme.ts`) with color presets and an on-site Theme Editor for live color previews, saved per browser, with a "Copy theme code" export.
- SEO: page metadata, `sitemap.xml`, `robots.txt`, favicon and app icons.
- Brand logo in `public/images/logo.jpg`.

### Notes

- Contact details, address and service areas in `src/lib/site.ts` are placeholders and must be replaced before launch.
- Set `showThemeEditor` to `false` in `src/lib/theme.ts` to hide the Theme Editor before launch.
