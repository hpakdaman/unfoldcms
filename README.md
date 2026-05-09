<div align="center">

# 🪻 UnfoldCMS

**The modern Laravel CMS built on shadcn/ui — self-hosted, source-available, one-time license.**

[![Website](https://img.shields.io/badge/🌐_Website-unfoldcms.com-2563EB?style=flat-square)](https://unfoldcms.com)
[![Demo](https://img.shields.io/badge/🎬_Live_Demo-Try_Now-10B981?style=flat-square)](https://unfoldcms.com/demo)
[![Docs](https://img.shields.io/badge/📚_Docs-Read-6366F1?style=flat-square)](https://unfoldcms.com/docs)
[![Pricing](https://img.shields.io/badge/💎_Pricing-From_$99-F59E0B?style=flat-square)](https://unfoldcms.com/pricing)
[![License](https://img.shields.io/badge/📄_License-Source--Available-7C3AED?style=flat-square)](LICENSE)

[![Laravel](https://img.shields.io/badge/Laravel-11.x-FF2D20?style=flat-square&logo=laravel)](https://laravel.com)
[![PHP](https://img.shields.io/badge/PHP-8.3+-777BB4?style=flat-square&logo=php&logoColor=white)](https://php.net)
[![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![Tailwind](https://img.shields.io/badge/Tailwind-v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![shadcn/ui](https://img.shields.io/badge/shadcn/ui-50+_components-000000?style=flat-square)](https://ui.shadcn.com)

</div>

---

UnfoldCMS is a self-hosted content management system for developers and agencies who want WordPress-class ease of use without WordPress's tradeoffs. **Laravel 11 + React 19 + Inertia 2 + Tailwind v4.** The entire admin is built on shadcn/ui — 50+ components, 183 pages, three themes.

🎯 **One-time license per site.** No subscriptions, no usage caps, no SaaS lock-in.
💰 **Runs on a $5/month VPS.** ~80 MB RAM idle. Shared hosting works too.
🔓 **You own your data.** Full SQL + files export at any time.

---

## Why UnfoldCMS

| | |
|---|---|
| **Owned, not rented** | Source code, database, and content live on your server. Full SQL + files export at any time. |
| **Modern stack** | Laravel 11 + React 19 + TypeScript + Tailwind v4 + shadcn/ui. The admin is *your* code, not a vendor widget. |
| **One-time pricing** | $99 Solo, $199 Pro, $499 Agency. No monthly bill that scales with your traffic. |
| **Built for developers** | Schema-as-code via PHP migrations. Service-provider extension model. No vendor framework to learn. |
| **Cheap to host** | ~80 MB RAM idle on a $5/month Hetzner VPS. Shared hosting works too. |
| **Multi-language ready** | Translatable fields, hreflang tags, locale-prefix routing built in. |

---

## What's in the box

| Module | Description |
|---|---|
| **Posts and Pages** | Block editor (Tiptap-based), structured fields, scheduled publishing |
| **Media Library** | Spatie Media Library, polymorphic associations, on-demand conversions |
| **Menus** | Tree-based builder, drag-and-drop reorder, internal/external/content links |
| **Forms** | JSON-schema builder, submissions table, CSV export, webhooks |
| **Settings** | Config-driven schema, admin UI auto-generated, frontend reads via `Setting::get()` |
| **Theming** | CSS variables + Tailwind v4 `@theme` directive, runtime swap, no build step |
| **Templates** | Full frontend designs (Aurora ships by default), seedable demo content |
| **SEO** | Meta tags, Open Graph, JSON-LD schema (Article, BreadcrumbList, Organization), hreflang |
| **RBAC** | Spatie Permission, granular per-model + per-action |
| **Multi-language** | spatie/laravel-translatable, JSON locale maps, URL-prefix routing |
| **Activity log** | Spatie ActivityLog, audit trail for all admin actions |
| **Subscribers** | Newsletter capture, double opt-in, segmentation, export |

---

## Stack

```
Backend     Laravel 11 + PHP 8.3 + Inertia 2
Frontend    React 19 + TypeScript + Vite
UI          shadcn/ui (50+ components) + Tailwind v4
Database    MySQL 8 / MariaDB 10.6+ (SQLite for dev)
Editor      Custom block editor on Tiptap foundation
Auth        Laravel Fortify + 2FA
Media       Spatie Media Library
Forms       Spatie Honeypot + custom schema engine
SEO         ralphjsmit/laravel-seo + custom JSON-LD layer
Hosting     Any LAMP host or $5/mo VPS (Hetzner, DigitalOcean, Linode)
```

---

## By the numbers

| Metric | Value |
|---|---|
| Lines of code | ~80K PHP + ~45K TS/TSX |
| Admin pages | 183 |
| shadcn components | 50+ |
| Themes shipped | 3 |
| Memory footprint (idle) | ~80 MB |
| Cold start | ~250 ms first request, ~40 ms warm |
| Build time (Vite + Inertia) | ~12 seconds |
| Test coverage | ~80% on critical paths (~600 PHPUnit tests) |

---

## Quick start

> **Note:** This public repository is a read-only mirror of the core CMS. The full source ships under a source-available license to license holders. See the [License](#license) section below.

### Try the demo

No install needed — admin login is on the demo page:

**[unfoldcms.com/demo](https://unfoldcms.com/demo)**

### Install with a license

```bash
# 1. Buy a license at https://unfoldcms.com/pricing
# 2. Download the release zip from your account dashboard
# 3. Extract and configure
unzip unfoldcms-{version}.zip
cd unfoldcms
cp .env.example .env
composer install --no-dev
php artisan key:generate
php artisan migrate

# 4. Set your license key in .env
echo "UNFOLD_LICENSE_KEY=your-key-here" >> .env

# 5. Visit your domain — admin is at /admin
```

Full installation docs: **[unfoldcms.com/docs](https://unfoldcms.com/docs)**

---

## Comparisons

UnfoldCMS isn't the right answer for every team. We're explicit about who it fits and who it doesn't:

| Comparison | Best for |
|---|---|
| [vs WordPress](https://unfoldcms.com/unfoldcms-vs-wordpress) | Laravel teams tired of WP plugin sprawl |
| [vs Contentful](https://unfoldcms.com/unfoldcms-vs-contentful) | SMBs priced out of Contentful Lite |
| [vs Sanity](https://unfoldcms.com/unfoldcms-vs-sanity) | Teams who want owned data |
| [vs Payload CMS](https://unfoldcms.com/unfoldcms-vs-payload) | Laravel vs Node tradeoff |
| [vs Strapi](https://unfoldcms.com/unfoldcms-vs-strapi) | Laravel vs Node, paid vs free |
| [vs Storyblok](https://unfoldcms.com/unfoldcms-vs-storyblok) | Visual editing vs structured content |
| [vs Ghost](https://unfoldcms.com/unfoldcms-vs-ghost) | Multi-page sites vs single-purpose blogs |
| [vs Webflow](https://unfoldcms.com/unfoldcms-vs-webflow) | Code-first vs visual builder |
| [vs Directus](https://unfoldcms.com/unfoldcms-vs-directus) | CMS-first vs database-first |
| [vs Hygraph](https://unfoldcms.com/unfoldcms-vs-hygraph) | Self-hosted vs SaaS GraphQL |
| [Full comparison hub](https://unfoldcms.com/compare) | Browse all comparisons |

---

## Roadmap

- **Q3 2026** — Public headless API (REST + GraphQL), signed content webhooks
- **Q4 2026** — Official `@unfoldcms/{nextjs,astro,sveltekit,nuxt}` SDK packages
- **2027** — Multi-tenant edition, plugin manifest system, AI-assisted content workflows

---

## Documentation

- [Installation guide](https://unfoldcms.com/docs)
- [Theming guide](https://unfoldcms.com/docs/theming)
- [Migration guides](https://unfoldcms.com/compare) — WordPress, Contentful, Sanity, Strapi
- [Why UnfoldCMS exists](https://unfoldcms.com/blog/why-developers-leaving-wordpress)
- [The complete guide to headless CMS in 2026](https://unfoldcms.com/blog/what-is-headless-cms)

---

## Contributing

This is a one-way mirror — the core CMS source is developed in a private repository and published here on each release. We don't accept pull requests directly, but we read every issue and discussion.

| Want to | Do this |
|---|---|
| Report a bug | [Open an Issue](https://github.com/hpakdaman/unfoldcms/issues/new) |
| Suggest a feature | [Start a Discussion](https://github.com/hpakdaman/unfoldcms/discussions) |
| Submit a patch | Paste your diff into an Issue or Discussion |
| Report a security issue | Email **support@unfoldcms.com** |

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full process.

---

## License

UnfoldCMS is **source-available** under the UnfoldCMS Source-Available License.

✅ **You can:**
- Read the source code in this repository
- Run UnfoldCMS for your own sites with a valid license
- Modify the code for your own use
- Submit patches via Issues or Discussions

❌ **You can't:**
- Run UnfoldCMS in production without a paid license
- Redistribute the code or sublicense it
- Use the UnfoldCMS name or logo in derivative products

See [LICENSE](LICENSE) for the full terms.

---

## Built by

**[Hamed Pakdaman](https://github.com/hpakdaman)** — a Laravel developer who got tired of fighting WordPress for client work and built a CMS that doesn't fight back.

If UnfoldCMS solved a problem for you, [tell me](https://unfoldcms.com/contact) — honest critique always welcome.

<div align="center">

**[Website](https://unfoldcms.com)** · **[Demo](https://unfoldcms.com/demo)** · **[Docs](https://unfoldcms.com/docs)** · **[Pricing](https://unfoldcms.com/pricing)** · **[Compare](https://unfoldcms.com/compare)**

⭐ **Star this repo** if you find UnfoldCMS interesting — it helps with discoverability.

</div>
