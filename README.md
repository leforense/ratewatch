# RATEWATCH - Burp® Intruder Rate Limiting Analysis

A visual dashboard for analyzing Burp Suite Intruder CSV exports — detect Rate Limiting behavior, WAF blocks, and response anomalies at a glance.

<img width="1687" height="1216" alt="image" src="https://github.com/user-attachments/assets/130e381e-f665-4f18-ab95-c01ebda9d5a1" />


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


## How to use:

1. Export the results table from Burp Intruder: Right-click the results and save them as a CSV, following this example:

<img width="1318" height="922" alt="ratewatch" src="https://github.com/user-attachments/assets/8aabc337-47b0-4238-b06a-eb8d9965e12f" />

2. Import the CSV file into the dashboard: Once the attack is complete, upload your file to visualize the data:
<img width="1722" height="1334" alt="mainscreen" src="https://github.com/user-attachments/assets/85765016-afb3-4678-b535-ce9489916c54" />

3. Rename your analysis (Optional): If you need to change the project name, just click here:
<img width="328" height="119" alt="image" src="https://github.com/user-attachments/assets/9d8340c9-5704-4282-b692-382fa1509244" />

4. Download the report: Click "Exportar Imagem" to save a snapshot of your dashboard:
<img width="203" height="76" alt="image" src="https://github.com/user-attachments/assets/11049f33-1f04-4839-accf-8f42ae1414ea" />

## License

This project is released into the public domain under the [Unlicense](LICENSE).  
No attribution required — copy, modify, and use freely.
