# 🚢 ChokePoint Map

ChokePoint Map is an open-source macroeconomic monitoring tool that maps global tanker activity, scores port-level strategic risk, and simulates what happens when major maritime chokepoints close.

It pulls live port data from the [IMF PortWatch](https://portwatch.imf.org/) platform and turns vessel traffic into interactive maps, vulnerability scores, and plain-language economic analysis—no install, no account, no setup.

## Try it now

**[https://solomonnaraine.github.io/chokepoint-map/](https://solomonnaraine.github.io/chokepoint-map/)**

Open that link in any modern browser and you are ready to go.

## How to use it

1. **Browse the map** — Each dot is a port. Larger markers mean more tanker traffic.
2. **Click a port** — The left panel shows congestion risk, vulnerability, and a generated economic summary for that location.
3. **Filter the data** — Narrow ports by region or risk level; the map and global stats update instantly.
4. **Run a shock simulation** — Close a chokepoint (e.g. Suez Canal, Strait of Hormuz) and watch dependent ports escalate to **CRITICAL (DISRUPTED)**.
5. **Export a report** — Download a markdown scenario summary of your current filters, closures, and selected port analysis.
6. **Read the methodology** — Open **Economic Methodology** in the sidebar for a short primer on how the analysis works.

## What it does

| Feature | What you get |
| :--- | :--- |
| **Live mapping** | ~2,000+ global ports on an interactive world map |
| **Economic inference** | Tiered analysis by port throughput—Primary Hub, Regional Node, or Feeder Port |
| **Vulnerability index** | Distance-based risk scoring against Suez, Panama, Hormuz, Bab el-Mandeb, and Malacca |
| **Shock simulator** | Model chokepoint closures and see supply-chain disruption cascade across ports |
| **Filters & sorting** | Slice the fleet by region, risk level, tanker volume, and more |
| **Scenario export** | One-click download to `chokepoint-map-scenario.md` |
| **Methodology guide** | Built-in explanation of nowcasting, chokepoint risk, and rerouting economics |

## Data & disclaimer

Port locations and tanker counts come from **IMF PortWatch**. Narratives and risk scores are **algorithmically generated** for education and scenario exploration—they are not official IMF forecasts, investment advice, or policy guidance.

## Open source

Source code is available on GitHub: [github.com/solomonnaraine/chokepoint-map](https://github.com/solomonnaraine/chokepoint-map)

Built with HTML, CSS, JavaScript, Leaflet, and Tailwind—entirely client-side, with no backend.

Questions, bugs, or ideas? Open an issue on the repository.
