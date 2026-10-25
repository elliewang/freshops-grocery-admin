# FreshOps — Grocery Company Operations Portal

A Walmart-style **internal grocery retail operations** dashboard, built as a standalone static GitHub Pages portfolio project. FreshOps is an original fictional brand and is not affiliated with Walmart.

## Included modules

- **Overview:** KPI cards, sales visualization, replenishment alerts, supplier activity.
- **Inventory:** Search SKUs, edit stock and reorder thresholds, create products.
- **Purchase Orders:** Create new supplier orders; receive orders and increase inventory.
- **Store Network:** Browse and edit stores and store-level sales.
- **Fulfillment:** Create demo customer orders; progress order statuses.
- **Employees:** Browse and add employee records.
- **Reports:** Sales summaries, inventory by category, CSV export.
- **FreshOps Assistant:** Browser-only rule-based chatbot answering questions from current demo inventory, purchasing, fulfillment, staffing and store data.

Demo data is stored in the browser's `localStorage`. Click **Reset Demo** to restore it. No server or build tools required.

## Run locally

Open `index.html` in a modern web browser. All references are relative and work in a GitHub Pages project subdirectory.

## Publish on GitHub Pages

1. Create a public GitHub repository, for example `freshops-grocery-admin`.
2. Upload `index.html`, `styles.css`, `app.js`, `.nojekyll`, and this `README.md` into the **repository root**. Do not upload an extra enclosing folder.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, branch **main**, folder **/(root)**, then Save.
5. Visit `https://YOUR_USERNAME.github.io/freshops-grocery-admin/` after publication.

## Security and limitations

**Demo only.** Product, store, employee, and order data is fictional. The assistant is rule-based, not a hosted LLM. The browser's `localStorage` is not a shared database; each device/browser has independent data. GitHub Pages is public and cannot protect internal business information or implement secure staff authentication. Do **not** upload real customer/employee data or confidential business information.

A production internal system would need enterprise SSO/RBAC, audited APIs, private deployment, centralized persistent database, encrypted transport, and integrations to inventory, POS/ERP/WMS/HR systems. A production AI assistant additionally needs a secured server-side model integration and authorization-aware tool calls.
