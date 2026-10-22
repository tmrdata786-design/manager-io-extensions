# Promo ERP — Manager.io Extensions

A suite of free, self-contained extensions for [Manager.io](https://www.manager.io) — each a single `index.html` file you can host anywhere and install by URL. No backend, no build step, no data leaves your machine.

**By [Promo ERP](https://promoerp.it/)** — scalable ERP solutions, custom apps, integrations & AI automation for businesses of all sizes.

---

## Extensions

| Extension | Folder | What it does | Access |
|---|---|---|---|
| 📊 **Sales Analytics Dashboard** | [`sales-analytics-dashboard/`](sales-analytics-dashboard/) | Daily sales analytics — day-by-day breakdowns, multi-month comparisons, KPI cards, interactive Chart.js charts, smart trend insights | Read-only |
| 🧰 **Developer Toolkit (Prompt Builder)** | [`developer-toolkit/`](developer-toolkit/) | Explore any `/api4/` endpoint, inspect its schema, and generate a complete AI prompt that produces a ready-to-install extension | Read-only |
| 📒 **Chart of Accounts Studio** | [`chart-of-accounts-builder/`](chart-of-accounts-builder/) | Browse, edit and bulk-import Profit & Loss accounts, Balance Sheet accounts, and Subsidiary Accounts via Excel templates | Read + Write (whitelisted COA endpoints) |
| 🧾 **Itemized Statement** | [`itemized-statement/`](itemized-statement/) | Line-by-line customer/supplier statements — full tax breakdowns, running balances, batch generation, print-ready layout, CSV export | Read-only |

Each extension includes an in-app **📖 README** button that opens the full user manual.

---

## Install (any extension)

1. Host the extension's `index.html` on any static host — **GitHub Pages**, [Netlify](https://netlify.com), or [Vercel](https://vercel.com) — to get a public URL.
2. In Manager.io: **Settings → Extensions → Add Custom Extension** (or **Settings → Custom Buttons** for the Itemized Statement).
3. Paste the URL as the **Endpoint**, pick a **Placement**, save.

All API calls go through Manager.io's native `postMessage` bridge — nothing is sent to any external server.

---

## Support & Custom Development

These tools are free. Need a custom Manager.io extension, an integration, a custom app, or AI automation for your business?

- 🌐 Website: [promoerp.it](https://promoerp.it/) · [promoautomations.vercel.app](https://promoautomations.vercel.app) · [Google Site](https://sites.google.com/view/promoerp/home)
- 📧 Email: [info@promoerp.it](mailto:info@promoerp.it) · [promoerp786@gmail.com](mailto:promoerp786@gmail.com)
- 📱 WhatsApp: [+92-321-8833616](https://wa.me/923218833616)
- 📘 Facebook: [facebook.com/promoerp786](https://facebook.com/promoerp786)
- ▶️ YouTube: [@PromoERP](https://www.youtube.com/@PromoERP)

---

## Disclaimer

These are independent, community-built tools and are **not officially affiliated with or endorsed by Manager.io**. Always backup your Manager.io data and verify figures before relying on any output.

## License

Free to use, modify, and share. Attribution appreciated but not required. The Itemized Statement component includes an MIT `LICENSE` file.

© Promo ERP 2026
