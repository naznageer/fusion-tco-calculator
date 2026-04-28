# Fusion HCI vs Cloud — Comparative TCO Calculator

A fully interactive, browser-based **Total Cost of Ownership (TCO)** calculator comparing **IBM Fusion HCI with GPU nodes** against **Cloud Dedicated GPU** infrastructure over a 5-year period.

> No server required. No dependencies. No installation. Open the HTML file and it works.

---

## 🌐 Live Demo

👉 **[Launch the TCO Calculator](https://YOUR-USERNAME.github.io/YOUR-REPO-NAME)**

*(Replace with your GitHub Pages URL after publishing)*

---

## 📊 What It Does

This tool helps sales teams, solution architects, and customers quickly model and compare the total cost of on-premises HCI infrastructure versus cloud GPU services, including:

- **5-Year NPV, ROI, IRR, and Payback Period**
- **Annual cash flow breakdown** for both solutions
- **Category-by-category cost comparison** (GPU, compute, storage, networking, power, operations)
- **Token economics** — cost per 1M tokens/sec for AI/LLM workloads
- **Hardware configuration builder** with live Bill of Materials pricing
- **Fully adjustable assumptions** — all inputs are editable and recalculate instantly

---

## 🗂️ What's Inside

```
fusion-tco-site/
├── index.html        ← The entire application (single file)
├── README.md         ← This file
├── .nojekyll         ← Tells GitHub Pages not to process the site with Jekyll
└── .github/
    └── FUNDING.yml   ← Optional: GitHub Sponsors config (can delete)
```

All logic, styling, and interactivity lives in `index.html` — no frameworks, no build tools, no npm.

---

## 🚀 How to Publish (GitHub Pages — Free)

### Step 1 — Create a GitHub account
Go to [github.com](https://github.com) and sign up (free).

### Step 2 — Create a new repository
1. Click the **+** icon → **New repository**
2. Name it something like `fusion-tco-calculator`
3. Set visibility to **Public** (required for free GitHub Pages)
4. Click **Create repository**

### Step 3 — Upload the files
**Option A — Browser upload (easiest):**
1. On your new repo page, click **Add file → Upload files**
2. Drag all files from this folder into the upload area
3. Click **Commit changes**

**Option B — Git command line:**
```bash
cd fusion-tco-site
git init
git add .
git commit -m "Initial release — Fusion HCI vs Cloud TCO Calculator"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git push -u origin main
```

### Step 4 — Enable GitHub Pages
1. In your repo, go to **Settings** → **Pages** (left sidebar)
2. Under **Source**, select **Deploy from a branch**
3. Set branch to **main**, folder to **/ (root)**
4. Click **Save**
5. Wait ~60 seconds, then visit: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME`

---

## 🔧 Customizing Default Values

All default assumptions are set in `index.html`. To change them, open the file in any text editor and find the `value="..."` attributes on the input fields, or edit the constants at the top of the `<script>` section.

Key constants you may want to adjust:

| Constant | Description | Default |
|---|---|---|
| `GPU_PRICES.H200` | H200 GPU list price | $231,273 |
| `SW_LIST` | Fusion HCI software list price | $442,074.24 |
| `SHIPPING` | Shipping cost | $5,511.50 |
| `i-gpuhr` input | Cloud GPU cost/hr | $10.00 |
| `i-hdh` input | HCI hardware discount | 75% |
| `i-sdh` input | HCI software discount | 75% |

---

## 📋 Tabs & Features

| Tab | Description |
|---|---|
| 📊 TCO Summary | KPI dashboard, payback timeline, category chart, full cash flow table |
| ☁ Cloud Cash Flow | Line-item cloud costs matching spreadsheet structure |
| ⚡ HCI Cash Flow | Line-item HCI costs with Year 3 GPU refresh, token cost isolation |
| 🔥 Token Economics | $/1M tokens/sec comparison for AI/LLM workloads |
| ⚙ Assumptions | All editable inputs — recalculates everything instantly |
| 🔧 HCI Config | Hardware configurator with live Bill of Materials |

---

## 💡 Tips for Use

- **Share the URL** — anyone with the link can use it; no login required
- **All calculations run in the browser** — no data is ever sent to a server
- **Works offline** — once loaded, the page works without internet (except for the Google Fonts)
- **Print/PDF friendly** — use your browser's Print → Save as PDF to export results
- **Mobile friendly** — responsive layout works on tablets and phones

---

## 🔒 Custom Domain (Optional)

To use a URL like `tco.yourcompany.com` instead of the GitHub Pages URL:

1. Buy a domain at [Namecheap](https://namecheap.com) or [Google Domains](https://domains.google)
2. In GitHub Pages Settings, enter your custom domain
3. Add a `CNAME` DNS record pointing to `YOUR-USERNAME.github.io`
4. GitHub handles the HTTPS certificate automatically

---

## 🛡️ Access Control (Optional)

To restrict access to specific users or require a password:

- **Netlify** — drag-and-drop `index.html` at [app.netlify.com/drop](https://app.netlify.com/drop), then enable password protection in site settings (~$19/mo)
- **Cloudflare Access** — put any URL behind Google/SSO login for free
- **Company intranet** — copy `index.html` to any internal web server or SharePoint

---

## 📄 License

This tool is provided for internal sales and pre-sales use. Modify freely for your organization's needs.

---

## 🙋 Support

To update pricing, discounts, or default assumptions, edit `index.html` directly — all values are clearly labeled in the Assumptions tab and the `<script>` constants at the top of the file.
