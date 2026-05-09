# UnfoldCMS

> The modern Laravel CMS built on shadcn/ui — self-hosted, source-available, one-time license.

[Website](https://unfoldcms.com) · [Live Demo](https://unfoldcms.com/demo) · [Docs](https://unfoldcms.com/docs) · [Pricing](https://unfoldcms.com/pricing) · [Compare](https://unfoldcms.com/compare)

UnfoldCMS is a self-hosted content management system for developers and agencies who want WordPress-class ease of use without WordPress's tradeoffs. Laravel 11 + React 19 + Inertia 2 + Tailwind v4. The entire admin is built on shadcn/ui — 50+ components, 183 pages, three themes.

One-time license per site. No subscriptions, no usage caps, no SaaS lock-in. Runs on a $5/month VPS.

---

## Why UnfoldCMS

- **Owned, not rented.** Source code, database, and content live on your server. Full SQL + files export at any time.
- **Modern stack.** Laravel 11 + React 19 + TypeScript + Tailwind v4 + shadcn/ui. The admin is your code, not a vendor widget.
- **One-time pricing.** $99 Solo, $199 Pro, $499 Agency. No monthly bill that scales with your traffic.
- **Built for developers.** Schema-as-code via PHP migrations. Service-provider extension model. No vendor framework to learn.
- **Cheap to host.** ~80 MB RAM idle on a $5/month Hetzner VPS. Shared hosting works too.

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

## Quick start

> **Note:** This public repository is a read-only mirror of the core CMS. The full source ships under a source-available license to license holders. See the [License](#license) section below.

For a live preview, use the [demo](https://unfoldcms.com/demo) — admin credentials are on the demo page.

For a paid install:

1. Buy a license at [unfoldcms.com/pricing](https://unfoldcms.com/pricing)
2. Download the release zip from your account
3. Extract to your server (or run via Composer if licensed)
4. Run `php artisan migrate` and `php artisan key:generate`
5. Configure `.env` and visit your domain

Full installation docs: [unfoldcms.com/docs](https://unfoldcms.com/docs)

## Comparisons

UnfoldCMS isn't the right answer for every team. We're explicit about who it fits and who it doesn't:

- [vs WordPress](https://unfoldcms.com/unfoldcms-vs-wordpress) — for Laravel teams tired of WP plugin sprawl
- [vs Contentful](https://unfoldcms.com/unfoldcms-vs-contentful) — for SMBs priced out of Contentful Lite
- [vs Sanity](https://unfoldcms.com/unfoldcms-vs-sanity) — for teams who want owned data
- [vs Payload CMS](https://unfoldcms.com/unfoldcms-vs-payload) — Laravel vs Node tradeoff
- [vs Strapi](https://unfoldcms.com/unfoldcms-vs-strapi) — Laravel vs Node, paid vs free
- [Full comparison hub](https://unfoldcms.com/compare)

## Roadmap

- **Q3 2026:** Public headless API (REST + GraphQL), signed content webhooks
- **Q4 2026:** Official `@unfoldcms/{nextjs,astro,sveltekit,nuxt}` SDK packages
- **2027:** Multi-tenant edition, plugin manifest system, AI-assisted content workflows

## Contributing

This is a one-way mirror — the core CMS source is developed in a private repository and published here on each release. We don't accept pull requests directly, but we read every issue and discussion.

How to contribute:

- **Bug reports:** [Open an Issue](https://github.com/hpakdaman/unfoldcms/issues/new) with a reproduction case
- **Feature requests:** [Start a Discussion](https://github.com/hpakdaman/unfoldcms/discussions)
- **Patches:** Paste your diff into an Issue or Discussion. Accepted patches are credited in the release notes.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full process.

## License

UnfoldCMS is **source-available** under the UnfoldCMS Source-Available License. You can:

- ✅ Read the source code in this repository
- ✅ Run UnfoldCMS for your own sites with a valid license
- ✅ Modify the code for your own use
- ✅ Submit patches via Issues or Discussions

You can't:

- ❌ Run UnfoldCMS in production without a paid license
- ❌ Redistribute the code or sublicense it
- ❌ Use the UnfoldCMS name or logo in derivative products

See [LICENSE](LICENSE) for the full terms.

## Built by

[Hamed Pakdaman](https://github.com/hpakdaman) — a Laravel developer who got tired of fighting WordPress for client work and built a CMS that doesn't fight back.

If UnfoldCMS solved a problem for you, [contact me](https://unfoldcms.com/contact). Honest critique welcome.
