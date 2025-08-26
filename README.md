# DFIR Splunk App

**Version:** 0.1 (Initial Release)
**Status:** :white_check_mark: Released
**App Name:** `DFIR`

## Overview

The **DFIR Splunk App** is now officially released as **v0.1**. This initial version provides a streamlined, easy-to-install package containing all essential dashboards for Digital Forensics and Incident Response (DFIR) operations.

This app is designed to simplify deployment and ensure consistency across your Splunk environments by bundling everything into a single, installable unit.

1.  Download the latest `DFIR.spl` file from https://github.com/dfirvault/Splunk-DFIR-Dashboards/releases/tag/v0.1.
2.  In your Splunk Web interface, navigate to **Apps > Manage Apps**.
3.  Click on **Install app from file**.
4.  Click **Choose File** and select the downloaded `dfir-X.X.X.spl` file.
5.  Click **Upload**.
6.  Restart Splunk if prompted.

# 🕵️‍♂️ Splunk DFIR Dashboard Collection

This repository contains a curated set of tested and production-ready **Splunk dashboard XML files** designed specifically for **Digital Forensics and Incident Response (DFIR)** investigations.

![image](https://github.com/user-attachments/assets/80c86773-44cd-4f7c-b2f5-beedd1790a24)
![image](https://github.com/user-attachments/assets/2117681e-99aa-4556-b759-81f2a0247956)


## 📦 What’s Inside

Over the years, during numerous real-world DFIR cases, these dashboards were developed, refined, and tested extensively. Each XML file represents a complete Splunk dashboard that provides insights into log data commonly collected during investigations.
Credit: https://github.com/Truvis/SplunkDashboards

### ✅ Features

- **Case-Based Drop-down Selector**: Analysts can select the case-specific index from a drop-down menu.
- **Plug-and-Play Dashboards**: Upload logs (`evtx`, `csv`, `json`, `plaso`, etc.) into a designated index, and the dashboards will automatically parse and analyze them.
- **Automated Analysis**: Built-in searches and panels provide immediate visualizations and actionable insights.
- **Flexible Data Ingestion**: Works with a wide range of log types and formats.
- **Optimized for Local Splunk Enterprise** deployments (no Splunk Cloud dependencies).

---

## 🧠 Use Case

These dashboards are intended for **DFIR analysts** who need quick, repeatable, and insightful visibility into forensic data. Typical workflow:

1. Spin up a **local instance** of Splunk Enterprise.
2. Ingest logs collected from the case:  
   - Windows Event Logs (`.evtx`)  
   - Plaso storage files  
   - CSVs from triage tools or EDRs  
   - JSON/NDJSON logs
3. Assign them to a unique **index** (e.g., `case_july2025_ransomware`).
4. Open the corresponding dashboard in Splunk.
5. Use the **index selector** to switch between cases.
6. Begin analysis using built-in visualizations, correlations, and automated insights.

---

## 📁 Dashboard Structure

Each `.xml` file in this repo is a complete dashboard definition. You can:

- Copy/paste the XML into Splunk’s **"Import Dashboard"** interface.
- Or place it into `$SPLUNK_HOME/etc/apps/YOUR_APP_NAME/default/data/ui/views/`.

---

## 🚀 Getting Started

### 1. Install Splunk Enterprise (if not already)
Download and install from: [https://www.splunk.com](https://www.splunk.com)

### 2. Ingest Your Data
Use the **Add Data** interface or CLI to import your logs into a defined index.

### 3. Import Dashboards
- Go to **Dashboards > Create New Dashboard**
- Choose **"Import XML"**, then paste contents of a `.xml` file from this repo.

### 4. Use It!
- Open the dashboard.
- Select your case index from the dropdown.
- Review logs, timelines, process trees, event IDs, artifacts, and much more.

---

## 🛠 Dashboard Types

This repository includes dashboards for:

- 🔍 Event Log Triage
- 📊 Process Timeline Visualization
- 🧾 Logon Activity Summaries
- 🖥️ Host Artifact Mapping
- 💾 Plaso Timeline Analysis
- 🛡️ Detection Hits by Rule/Tool
- … and more

> Each dashboard is annotated in comments for ease of understanding and modification.

---

## 📚 Resources

- Splunk Documentation: [https://docs.splunk.com](https://docs.splunk.com)
- DFIR Playbooks: Coming soon to the Wiki section.

---

## 🤝 Contributions & Feedback

This project is continuously improved. If you have:
- Suggestions for enhancements,
- Found a bug or false-positive,
- Or want to contribute your own dashboard,

---

## 👤 Author

**Jacob Wilson**  
📧 dfirvault@gmail.com
[https://www.linkedin.com/in/jacob--wilson/](https://www.linkedin.com/in/jacob--wilson/)

**More information:**
[https://dfirvault.com](https://dfirvault.com)
---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
