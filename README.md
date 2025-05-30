# 🛡️ PhishAnalyzer

**PhishAnalyzer** is an open-source email phishing analysis tool that lets you upload `.eml` files and receive a full breakdown of potential threats — including header inspection, link analysis, attachment scanning, and phishing risk scoring — all locally with no cloud upload or login required.

> Built with **FastAPI** (Python) and **React + Tailwind** (TypeScript), this app empowers security researchers, analysts, and developers to inspect emails in a self-hosted, privacy-first manner.

---

## 🚀 Features

- 📬 **Upload `.eml` Files** via browser interface
- 🔎 **Header & Metadata Analysis** (From, To, Subject, Received paths, etc.)
- 🔗 **Extract URLs** and embedded links
- 🧪 **Check Attachments** for macro-based threats (via `oletools`)
- 🧠 **Risk Scoring Engine**: Flags Safe / Suspicious / Malicious emails
- 🧬 **IOC Extraction**: IPs, domains, emails, and hashes
- 🔐 **Optional Enrichment** via VirusTotal & Abuse.ch (via `.env`)
- 💾 **Analysis History**: View and manage past scans
- 🌐 Works **fully offline** — no cloud, no login, no data leak

---

## 🧱 Tech Stack

| Layer     | Tech                          |
|-----------|-------------------------------|
| Frontend  | React, TypeScript, TailwindCSS |
| Backend   | Python, FastAPI, Uvicorn       |
| Parsing   | `mailparser`, `email`, `oletools`, `beautifulsoup4` |
| Storage   | Local JSON files (`/data/analyses/`) |
| Optional  | VirusTotal / Abuse.ch API for threat enrichment |

---

## ⚙️ Getting Started

### 📦 Prerequisites
- Python 3.10+
- Node.js 18+
- Git

---

### 🖥️ Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/phish-analyzer.git
cd phish-analyzer

🧠 Related Tools & Landscape
PhishAnalyzer is developed independently. It draws inspiration from other email analysis tools in the open-source ecosystem, including PhishInspect, emlAnalyzer, InQuest Labs, and other such tools focused on phishing detection and email threat analysis.
