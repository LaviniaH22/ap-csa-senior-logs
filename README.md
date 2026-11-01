# Senior Logs — AP Computer Science A Senior Project

A senior connection website created by **Lavinia Hawkins** for **NHHS AP Computer Science A, May 2024**.

The project helps graduating classmates share profiles, future plans, words of encouragement, and useful resources.

## Features

- Welcome page and navigation between the site's sections.
- Account activation and profile-submission interfaces.
- A home page displaying senior profiles and contact information.
- Resource browsing and submission pages.
- An Express backend that reads and updates CSV records.

## Technology

**Frontend:** HTML, CSS, JavaScript, Fetch API.  
**Backend:** Node.js, Express, CORS, csv-parse, csv-stringify.  
**Storage:** CSV file. The original project used Render-hosted services.

## Project structure

| Folder | Purpose |
| --- | --- |
| `intro/` | Welcome page |
| `home/` | Senior profile display |
| `new/` | Account activation interface |
| `newpf/` | Profile submission interface |
| `res/` | Shared resources |
| `resa/` | Resource submission |
| `data/` | Express API, dependencies, and fictional example data |

## Run locally

Requires Node.js and npm. From the `data` directory:

```bash
npm ci
```

Create a local CSV from the fictional example. On Windows PowerShell:

```powershell
Copy-Item data.example.csv data.csv
```

On macOS or Linux:

```bash
cp data.example.csv data.csv
```

Start the API:

```bash
npm start
```

In a second terminal, also in `data`, start the frontend:

```bash
npm run preview
```

Open **http://localhost:8080**. The publishing copy points frontend requests to **http://localhost:3000/data** rather than the historical hosted API.

The fictional `Demo Student` record starts with the literal value `password`, matching the original activation flow. Use invented information and a disposable demo password only.

## Historical project scope

This preserves the original school project's design. Its account flow uses client-side credential checks and a CSV API; it is a coursework prototype, not production authentication. Run it locally with fictional data.

The original student CSV, installed dependencies, and Git history are excluded. The repository includes only fictional sample records. Portfolio preparation adds documentation, a root landing-page redirect, local startup scripts, and local API URLs, and fixes a missing closing brace in the resource-submission script.

## Validation

JavaScript syntax and local HTML/CSS/script/image references were checked during preparation. Historical deployment availability and complete interactive behavior have not been verified.
