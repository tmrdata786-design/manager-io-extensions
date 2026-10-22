# 📒 Chart of Accounts Studio — for Manager.io

A bulk-import chart-of-accounts extension for [Manager.io](https://www.manager.io) — browse, edit, and bulk-create/update Profit & Loss accounts, Balance Sheet accounts, and Subsidiary Accounts via Excel templates, in a single self-contained HTML file.

**By [Promo ERP](https://promoerp.it/)** — scalable ERP solutions, custom apps, integrations & AI automation for businesses of all sizes.

---

## ✨ Features

- **Load live data** — pulls Profit & Loss accounts, Balance Sheet accounts, and all groups from Manager
- **Four workspaces** — Profit & Loss · Balance Sheet · Subsidiary Accounts · Control Accounts
- **Report tab** — sortable columns, instant search, inline row editing
- **🔢 Bulk Numbering** — auto-assign sequential codes to selected rows
- **Bulk Import** — download a tailored Excel template (with your valid Groups / Types / Control Accounts baked in), fill it, and import
- **Safe re-imports** — matching by Code: existing Codes are updated, new Codes created — never duplicated
- **Full preview before write** — every bulk import shows exactly which rows will be created vs updated before a single request is sent
- **Read + Write** — uses Manager's chart-of-accounts API endpoints (whitelisted)

---

## 📌 Before You Touch This Extension

1. **Create your Groups in Manager first (manually)** — this extension imports accounts *into groups*; it does not create the groups themselves. Every group name you plan to use in Excel must already exist in Manager, spelled exactly the same way.
2. **Create at least one Control Account "bucket" per type (manually)** — in **Settings → Control Accounts**. Subsidiary Accounts import needs a bucket to attach each account to.
3. **Fixed Assets & Intangible Assets need TWO buckets each** — a main bucket plus an "Accum. Depreciation / Amortization" bucket. Create these manually, or import them via the Subsidiary Accounts sheet first.

---

## 🚀 Installation

1. Enable GitHub Pages on this repo *(Settings → Pages → Deploy from main branch)*
2. Your extension URL will be:
   ```
   https://<your-username>.github.io/manager.io-chart-of-accounts-builder/
   ```
3. In Manager.io go to **Settings → Extensions → Add Custom Extension**
4. Paste the URL above and save

---

## 🧭 How to Use

1. Press **⬇ Load Data** to fetch your current accounts and groups from Manager — do this every time you open the extension, and again after making changes directly in Manager.
2. Pick a tab: **Profit & Loss**, **Balance Sheet**, **Subsidiary Accounts**, or **Control Accounts**.
3. Use the **Report** tab to browse, search, sort, and edit rows inline. On P&L / Balance Sheet you can tick rows and use **🔢 Bulk Number** for sequential codes.
4. Use the **Bulk Import** tab — download the template, fill it in, preview the changes, then import.
5. Re-importing is always safe — matching is done by **Code**. A Code that already exists gets **updated**, never duplicated.
6. If something fails, the real Manager error message is shown on screen — open the browser console (F12) for full technical detail.

---

## ⚙️ Technical Details

| Property | Detail |
|---|---|
| File type | Single self-contained `.html` file |
| External library | ExcelJS from cdnjs (for building/reading `.xlsx` templates only) |
| Access | Read + Write — whitelisted chart-of-accounts API endpoints only |
| Security | Origin-pinned postMessage, endpoint whitelist, XSS-safe rendering, full write preview |
| Storage | Nothing stored between sessions — no localStorage, cookies, or databases |
| Framework | Vanilla HTML / CSS / JavaScript — no build step required |

---

## ⚠️ Disclaimer

This extension is an independent, community-built tool and is **not officially affiliated with or endorsed by Manager.io**. Always backup your Manager.io data before bulk imports. Review every import preview carefully before confirming writes.

---

## 📄 License

Free to use, modify, and share. Attribution appreciated but not required.

---

## 👤 Author

**Promo ERP** — dedicated ERP service provider specializing in scalable, feature-rich solutions for businesses of all sizes. We synchronize your company operations by integrating finance, inventory & sales into a single, unified platform — plus customization, integrations, custom apps & AI automation.

- 🌐 Website: [promoerp.it](https://promoerp.it/) · [promoautomations.vercel.app](https://promoautomations.vercel.app) · [Google Site](https://sites.google.com/view/promoerp/home)
- 📧 Email: [info@promoerp.it](mailto:info@promoerp.it) · [promoerp786@gmail.com](mailto:promoerp786@gmail.com)
- 📱 WhatsApp: [+92-321-8833616](https://wa.me/923218833616)
- 📘 Facebook: [facebook.com/promoerp786](https://facebook.com/promoerp786)
- ▶️ YouTube: [@PromoERP](https://www.youtube.com/@PromoERP)
