# 🚢 ChokePoint Map

A data-dense, open-source macroeconomic monitoring tool built with pure vanilla web technologies. ChokePoint Map ingests automated satellite AIS data from the IMF PortWatch platform to map global tanker flows, assess port strategic vulnerabilities, and simulate major supply chain disruptions—such as closing the Suez Canal or Strait of Hormuz—with real-time algorithmic economic inference generation.

**Live Demo:** [https://solomonnaraine.github.io/chokepoint-map/](https://solomonnaraine.github.io/chokepoint-map/)

No build step. No framework. No backend. Clone, serve, and deploy.

## ✨ Core Features

| Module | Description |
| :--- | :--- |
| 🗺️ **Live Mapping** | Interactive Leaflet map with ~2,000+ global port nodes, styled using a smooth, dark vector basemap that perfectly integrates with our custom ocean-intelligence palette. |
| 🧠 **Dynamic Inference Engine** | Click any port to generate tiered macroeconomic narratives based on throughput (Primary Hub · Regional Node · Feeder Port) with congestion risk scoring. |
| 🎯 **Strategic Vulnerability Index** | Haversine-distance analysis against five monitored chokepoints (Suez, Panama, Hormuz, Bab el-Mandeb, Malacca) with Low → Critical vulnerability scoring. |
| ⚡ **Geopolitical Shock Simulator** | Toggle chokepoint closures to instantly escalate dependent ports to CRITICAL (DISRUPTED), flash map markers in high-visibility hot pink, and inject crisis alerts into live analysis text. |
| 🔎 **Data Filtering & Sorting Suite** | Slice the fleet by region, risk level, and sort metric—map markers and global aggregate stats update in real time. |
| 📄 **Client-side Report Exporter** | One-click export of the full scenario state (filters, closures, stats, port narrative) to `chokepoint-map-scenario.md`. |
| 📚 **Economic Methodology Drawer** | Built-in documentation primer covering nowcasting theory, chokepoint vulnerability, and Cape of Good Hope rerouting economics. |

## 🏗️ Tech Stack

* **HTML5:** Semantic layout frame.
* **Styling:** Tailwind CSS (via CDN) + custom `styles.css` for rich transitions and modal layouts.
* **Mapping:** Leaflet.js 1.9.4.
* **Logic:** Vanilla JavaScript (modular architecture, no bundler required).
* **Data:** IMF PortWatch ArcGIS REST FeatureServer API.

## 🚀 Quick Start

### Prerequisites

* A modern web browser (Chrome, Firefox, Safari, or Edge).
* Any local static file server (required—browsers block cross-origin API `fetch` from raw `file://` URIs).

### 1. Clone the repository

```bash
git clone https://github.com/solomonnaraine/chokepoint-map.git
cd chokepoint-map
```

### 2. Run a local server

```bash
# Python 3
python -m http.server 8080

# Node.js (npx, no install)
npx serve .

# PHP
php -S localhost:8080
```

Open **http://localhost:8080** in your browser.

### 3. Explore the dashboard

1. Wait for port markers to load on the global map.
2. Click a port marker for economic inference in the left panel.
3. Use **Data Filters** to isolate risk profiles by region.
4. Toggle chokepoints in the **Geopolitical Shock Simulator**.
5. Export a scenario report or open **Economic Methodology** for theory context.

## 🌐 Deploy to GitHub Pages

ChokePoint Map is a **static site**—all files live at the repository root.

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set:
   * **Source:** `Deploy from a branch`
   * **Branch:** `main` · `/ (root)`
4. Save. Your site will be live at:

   ```
   https://solomonnaraine.github.io/chokepoint-map/
   ```

## 📁 Project Structure

```
chokepoint-map/
├── index.html      # Application shell, sidebar layout, methodology drawer
├── app.js          # Map init, API fetch, inference engine, filters, export
├── styles.css      # Custom theme, animations, drawer & simulator UI
└── README.md
```

## ⚠️ Disclaimer

ChokePoint Map is an **open-source educational and scenario-analysis tool**. Economic narratives are algorithmically generated heuristics—not official IMF forecasts, investment advice, or policy guidance. Data © [IMF PortWatch](https://portwatch.imf.org/).

## 🤝 Contributing

Issues and pull requests are welcome. This project intentionally stays dependency-free—please avoid introducing build tooling unless there is a compelling reason.

## 📜 License

Released for open-source use. See repository license file for terms.
