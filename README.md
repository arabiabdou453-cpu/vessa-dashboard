<div align="center">

# 🌿 Vessa — Skincare Lab Stock & Supply

**Modern, ultra-responsive inventory management and fulfillment dashboard engineered for cosmetics labs and skincare manufacturing.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-18%2B-339933?logo=node.js&logoColor=white)](https://nodejs.org/)
[![JavaScript](https://img.shields.io/badge/ES_Modules-Vanilla_JS-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)
[![Design System](https://img.shields.io/badge/CSS3-Design_Tokens_%26_Grid-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/arabiabdou453-cpu/vessa-dashboard/pulls)

[🚀 Live Demo](https://arabiabdou453-cpu.github.io/vessa-dashboard/#/dashboard/overview) • [Overview](#-overview) • [Quick Start](#-quick-start) • [Architecture](#-architecture--tech-stack) • [Modules](#-core-modules) • [Keyboard Shortcuts](#-keyboard-shortcuts)

---

</div>

## 📖 Overview

**Vessa** is an enterprise-grade, lightweight stockroom and supply chain application designed specifically for skincare and cosmetics laboratories. It seamlessly orchestrates operations across production batches, inventory across multiple locations (warehouses, cleanrooms, and retail shops), purchase orders, suppliers, and sales fulfillment boards.

Built with a **zero-overhead, vanilla web architecture**, Vessa delivers sub-millisecond route transitions, fluid micro-interactions, robust keyboard navigation, and native light/dark adaptive theming without third-party framework weight.

---

## ✨ Key Features

| Category | Capability | Description |
| :--- | :--- | :--- |
| 🧪 **Batch Tracking** | Quality Release & Expiration | Monitor formulations, chemist allocations, QA release dates, lot numbers, and shelf-life expirations. |
| 🏢 **Multi-Location Inventory** | Real-Time Stock Allocations | Track physical items across Central Warehouses, Testing Labs, and Retail Outlets with live capacity meters. |
| 📋 **Order Fulfillment** | Pick · Pack · Ship Board | Kanban-style sales order pipeline with instantaneous status updates and fulfillment progress tracking. |
| 🔔 **Predictive Stock Alerts** | Automated Safety Buffers | Intelligent reorder warnings, safety stock depletion alerts, and vendor lead-time notifications. |
| 📈 **Financial Analytics** | Valuation & Sales Velocity | Daily closing balance charts, 30/90/365-day inventory holding trends, and target revenue velocity. |
| 🔎 **Global Quick Finder** | Command Palette (`⌘K` / `Ctrl+K`) | Search instantly across products, SKUs, lot batches, customers, orders, and suppliers. |
| 🌓 **Adaptive Theme Engine** | Light / Dark & Accent Palettes | Automatic OS sync with manual overrides and customizable accent tones (*Pine, Cobalt, Ocean, Graphite*). |

---

## 🏗️ Architecture & Tech Stack

Vessa is built around performance-first web principles:

```
┌────────────────────────────────────────────────────────┐
│                      Client Layer                      │
├────────────────────────────────────────────────────────┤
│  • Vanilla ECMAScript (ES Modules & Dynamic Imports)   │
│  • Modern CSS Grid & Flexbox with CSS Custom Properties│
│  • SVG Vector Data Visualization (Charts & Gauges)     │
│  • Native Accessible Dialogs & Keyboard Trap Navigation│
├────────────────────────────────────────────────────────┤
│                      Runtime Layer                     │
├────────────────────────────────────────────────────────┤
│  • Zero-Dependency Node.js Static Server               │
│  • Client-Side Hash Router (#/dashboard/overview)      │
│  • LocalStorage State Persistence & Fallbacks          │
└────────────────────────────────────────────────────────┘
```

- **Frontend Core:** Pure Modern JavaScript (ES Modules, Dynamic `import()`, Custom Components)
- **Styling Architecture:** Semantic CSS3, Design Tokens (`--bg`, `--surface`, `--primary`, `--pine`, `--shadow`), Sub-grid Alignment
- **Charts & Sparklines:** Native Scalable Vector Graphics (SVG) with mathematical Bezier line generation
- **Micro-Interactions:** Magnetic button effects, spring-like cubic bezier transitions, and fluid state toggling

---

## 📁 Repository Structure

```text
vessa-dashboard/
├── assets/                  # Compiled JavaScript modules and styles
│   ├── index-*.js           # Application kernel & routing engine
│   ├── index-*.css          # Global design system & typography tokens
│   ├── dashboard-*.js       # Overview, KPIs, charts, and activity streams
│   ├── dashboard-*.css      # Grid layout & card specifications
│   ├── products-*.js        # Catalog & SKU inventory management
│   ├── orders-*.js          # Order processing & shipping board
│   ├── analytics-*.js       # Valuation and metrics visualization
│   └── ...                  # Additional dedicated view modules
├── photos/                  # Skincare product photography assets
│   └── vessa/               # Balms, serums, oils, fluids, and duos
├── index.html               # Main application shell with SEO & pre-paint script
├── server.js                # Lightweight zero-dependency HTTP server
├── package.json             # Project metadata and run scripts
├── .gitignore               # Ignored environments and system caches
└── README.md                # Comprehensive documentation
```

---

## 🚀 Quick Start

### Prerequisites
- [Node.js](https://nodejs.org/) v18.0.0 or higher.
- A modern web browser (Chrome, Edge, Firefox, Safari).

### 1. Clone the repository
```bash
git clone https://github.com/arabiabdou453-cpu/vessa-dashboard.git
cd vessa-dashboard
```

### 2. Launch the application
```bash
npm start
```
*Alternatively, run directly:*
```bash
node server.js
```

### 3. Open in your browser
Navigate to:
```
http://localhost:3000/#/dashboard/overview
```

---

## 🧩 Core Modules

### 1. Dashboard Overview (`#/dashboard/overview`)
The command hub presenting high-level stock counts, asset valuations, 30-day sales trajectory, live shipping meters, and real-time laboratory activity logs.

### 2. Products & Inventory (`#/products`)
Granular management of all skincare formulations, unit sizes, unit costs, wholesale values, minimum safety thresholds, and active lot batches.

### 3. Orders Board (`#/orders`)
Visual order fulfillment stream featuring pick list generation, packing verification, shipping labels, and customer attribution.

### 4. Warehouses & Transfers (`#/warehouses`)
Multi-site allocation manager monitoring cubic capacity, bin assignments, and stock transfer movements between labs and distribution hubs.

### 5. Analytics & Reports (`#/analytics`)
Executive summaries on inventory turn rates, gross margin performance, stockout risks, and monthly replenishment budgets.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action | Description |
| :---: | :--- | :--- |
| <kbd>⌘</kbd> + <kbd>K</kbd> / <kbd>Ctrl</kbd> + <kbd>K</kbd> | Global Search | Open quick search for SKUs, orders, and batches |
| <kbd>Esc</kbd> | Dismiss Modal | Close active modal dialog or command palette |
| <kbd>Tab</kbd> | Focus Next | Accessible tab navigation through interactive elements |

---

## 🎨 Theme Customization

Vessa includes built-in persistence for visual settings in `localStorage`:

- **Theme Mode:** `vessa:theme` (`"light"`, `"dark"`, `"system"`)
- **Accent Color:** `vessa:accent` (`"pine"`, `"cobalt"`, `"ocean"`, `"graphite"`)
- **Sidebar State:** `vessa:side` (`"1"` for expanded, `"0"` for collapsed)

---

## 🤝 Contributing

Contributions, feature requests, and suggestions are warmly welcome!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">
  <sub>Crafted for high-efficiency cosmetic labs and modern stockrooms. Built with passion by <a href="https://github.com/arabiabdou453-cpu">Abdou Arabi</a>.</sub>
</div>
