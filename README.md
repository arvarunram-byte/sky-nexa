# 🛰️ SKY NEXA — Space Debris Tracking & Collision Prediction Platform

**Live Interactive Orbital Surveillance & AI Collision Risk Assessment System**

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

---

## 🚀 1-Line Pitch
> *"SKY NEXA tracks space debris and satellites in real time, predicts possible collision risks using AI and orbital dynamics models, and provides early visual alerts so satellite operators can execute safe collision-avoidance maneuvers."*

---

## 🌟 Features & Architecture

### Mode 1: 🛰️ Live Orbital Tracker (Real-Time LEO Surveillance)
- **Live Catalog Tracking**: Hundreds of active spacecraft (ISRO Cartosat/Risat/Oceansat, NASA, SpaceX Starlink, ESA Sentinel, Tiangong Station, ISS) and cataloged space debris fragments (Cosmos, Fengyun-1C, spent rocket bodies).
- **Search & Filtering**: Search by spacecraft name, owner country, or NORAD catalog ID. Filter by Active Satellites vs Tracked Debris shards.
- **Interactive 3D Raycasting**: Click any satellite or debris in 3D space to lock on, focus the camera, and inspect full orbital parameters (Velocity, Altitude, Inclination, Period, Agency).
- **AI Trajectory Telemetry**: Displays atmospheric drag loss rates, solar radiation pressure drift, and covariance confidence.

### Mode 2: 💥 Collision Simulator Lab
- **Incident Scenarios**:
  - **💥 2009 Iridium 33 vs Cosmos 2251:** Historic hypervelocity intersection with interactive 7-Day to 0-Hour timeline drag slider, collision physics, and debris cloud dispersal.
  - **🛰️ ISS vs Cosmos 1408 ASAT Debris:** High-proximity space station avoidance burn scenario (36-hour TCA at 4.2 km).
  - **⚡ Starlink Autonomous Proximity:** Autonomous Krypton ion thruster micro-burn avoidance protocol.
- **$\Delta V$ Thrust Optimizer (Hohmann Transfer)**:
  - Computes $\Delta v_1$ perigee boost, $\Delta v_2$ circularization, total $\Delta v_{tot}$, and Hydrazine ($N_2H_4$) propellant mass using the **Tsiolkovsky Rocket Equation**.
  - Renders the safe higher orbital plane (dashed green line) and transfer ellipse (yellow line) directly in 3D.
- **Official Conjunction Report Export**: 1-click download of standardized JSON telemetry reports.

---

## 🌐 Deployments

### Option 1: GitHub Pages
Host statically with 0 configuration.
- Go to repository **Settings** -> **Pages** -> Deploy from branch: `main` / `root`.

### Option 2: Render.com
1. Go to [dashboard.render.com](https://dashboard.render.com)
2. Click **New +** -> **Web Service** (or **Static Site**)
3. Connect your GitHub repository: `sky-nexa`
4. For **Web Service**:
   - Build Command: `npm install`
   - Start Command: `npm start`
5. For **Static Site**:
   - Build Command: *(leave blank)*
   - Publish directory: `.`

---

## 💻 Local Execution
```bash
git clone https://github.com/arvarunram-byte/sky-nexa.git
cd sky-nexa
npm start
```
Then open `http://localhost:3000/` in your browser.
