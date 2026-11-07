# GatePulse • Rate Limiting API Gateway & Telemetry Dashboard

[![Tech: HTML + Tailwind + JS](https://img.shields.io/badge/Tech-HTML5_·_Tailwind_CSS_·_JavaScript-0ea5e9.svg)]()
[![Single Folder: Zero Build](https://img.shields.io/badge/Architecture-Single_Folder_·_Zero_Build-success.svg)]()

> High-performance API Gateway implementing **Token Bucket** and **Sliding Window Log** rate limiting algorithms to control request traffic and prevent excessive requests, featuring 5+ RESTful endpoints and a real-time monitoring dashboard in a **single folder with zero complex dependencies**.

---

## ⚡ Highlights

- **Single Folder Architecture**: No nested `src/` or complex folder trees. Everything runs seamlessly from `index.html`.
- **Works 100% on GitHub & GitHub Pages**: Built using standard **HTML5**, **Tailwind CSS** (via CDN), and modern **JavaScript**. Zero missing features, zero broken imports, and zero build commands required.
- **Algorithms Implemented**:
  - **Token Bucket**: $O(1)$ time and memory with capacity $B$, refill rate $r$, and burst allowance.
  - **Sliding Window Log**: Rolling $W$-second timestamp tracking eliminating boundary spikes.
- **5+ RESTful API Endpoints**:
  1. `GET /api/v1/products` - Product catalog & inventory
  2. `GET /api/v1/users` - User directory & account roles
  3. `POST /api/v1/payments` - Transaction checkout (2x Token Cost multiplier)
  4. `GET /api/v1/analytics` - System metrics & latency percentiles
  5. `POST /api/v1/messages` - Outbound webhook & notification dispatch
  6. `GET /api/v1/health` - Health probe (Cost: 0, Exempt)
- **Monitoring Dashboard**:
  - Live KPI metrics (Total Requests, Allowed, Blocked 429, Throughput RPS, Overhead Latency)
  - Real-time animated Canvas Traffic Velocity Chart
  - Filterable Live Log Stream Table (All, Passed, Blocked)
  - Interactive Algorithm Lab with Token Bucket fluid fill gauge and Sliding Window timeline
  - Interactive API Playground with 15x traffic burst tester

---

## 🚀 How to Upload to GitHub in 3 Steps

1. In your project folder, run:
```bash
git init
git add .
git commit -m "feat: Single-folder Rate Limiter Gateway"
```

2. Link to your GitHub repository:
```bash
git branch -M main
git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO_NAME>.git
git push -u origin main
```

3. **(Optional) Enable Free 1-Click Hosting on GitHub Pages**:
   - Go to your repository on GitHub.
   - Click **Settings** &rarr; **Pages**.
   - Under **Build and deployment**, select **Deploy from a branch**.
   - Choose `main` branch and `/ (root)` folder, then click **Save**.
   - Your gateway dashboard will be live at `https://<YOUR_GITHUB_USERNAME>.github.io/<YOUR_REPO_NAME>/` with all features working!
