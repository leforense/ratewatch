# BURPINTRUDER DATA ANALYST

A visual dashboard for analyzing Burp Suite Intruder CSV exports — detect Rate Limiting behavior, WAF blocks, and response anomalies at a glance.

## Features

- **Automatic CSV parsing** — supports Burp Suite Intruder tab-separated exports
- **Real-time stats** — total requests, duration, average RPS (requests per second)
- **Error & Timeout detection** — counts HTTP 5xx errors and 504 timeouts automatically
- **Response Integrity chart** — breakdown of all status codes (2xx, 3xx, 4xx, 5xx)
- **Latency time-series chart** — per-request response time colored by status code
- **RPS Gauge** — visual throughput meter
- **Dashboard export** — download the full dashboard as a PNG image
- **Editable project name** — rename the analysis before exporting

## Stack

- React 19 + TypeScript
- Vite
- Tailwind CSS
- Recharts
- html2canvas
- Lucide React

## Prerequisites

- Node.js 18+

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/burp-intruder-analyst.git
   cd burp-intruder-analyst
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser at `http://localhost:3000`.

## How to Export from Burp Suite

1. Run an **Intruder** attack in Burp Suite.
2. After the attack finishes, right-click the results table → **Save results** → choose **CSV**.
3. Upload the `.csv` file to the dashboard.

## Building for Production

```bash
npm run build
```

The output will be in the `dist/` folder.

## License

This project is released into the public domain under the [Unlicense](LICENSE).  
No attribution required — copy, modify, and use freely.
