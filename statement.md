# 📋 Project Problem Statement & Scope

## 1. Problem Statement
Meteorological data tracking at regional or agricultural levels often suffers from localized fragmentation. Small-scale data collection centers, individual researchers, and modern farms need a straightforward, localized way to document climate shifts without dealing with overly complex cloud enterprise configurations. 

Manual weather tracking sheet logs are prone to human input errors, lack immediate threshold classifications, and do not compile immediate data analytics. This makes it difficult to quickly spot dangerous environmental shifts like sudden flash heavy rains or prolonged heatwaves. 

To solve this, this project introduces a standalone, highly modular desktop application. It acts as an immediate processing script to safely capture, validate, classify, and mathematically summarize core weather inputs right at the collection source.

---

## 2. Project Scope
The application operates as an interactive command-line evaluation tool that processes weather logs over a single-month window. 

### What is Included:
* **Time-Bound Framework Automation:** Dynamic day count mappings across standard calendar cycles, incorporating automated loop logic corrections for leap-year Februaries.
* **Dual-Stream Input Verification:** Strict terminal boundaries protecting inputs by forcing re-prompts for misspelled tracking parameters.
* **Algorithmic Classification Triggers:** Logical data sorting structures that parse raw measurements against set threshold tiers for rainfall, temperatures, and cloud density tracking.
* **Aggregated Statistical Computation:** Immediate array analytics mapping monthly accumulation patterns alongside peak value spikes.

### What is Excluded (Out of Scope):
* API integrations with real-time live satellite feeds or public hardware trackers.
* Relational database engine persistence (data resets fresh upon session termination).
* Historical multivariable forecasting or machine learning predictions.

---

## 3. Target Users
This localized tool is built tailored to the operational needs of:
* **Agricultural Coordinators & Modern Farmers:** Who rely on fast, offline micro-climate statistics to time crop irrigation schedules.
* **Environmental Field Researchers:** Who need a lightweight validation system to check collected field variables before importing them into heavy data analysis frameworks.
* **Academic Labs & Students:** Seeking a clear, production-grade example of modular code separation, basic error handling, and object-oriented testing design.

---

## 4. High-Level Core Features
* **Interactive Data Entry System:** Interactive date-labeled input steps (`i / month / year`) that guide the user predictably.
* **Rainfall Severity Monitor:** Instantly maps daily precipitation volumes to clear alert labels (ranging from *"no rain"* up to *"extremely heavy rain"* alerts).
* **Thermal Range Classifier:** Categorizes temperature thresholds to spot heat stress conditions (e.g., *"extremely hot day"*, *"very cold day"*).
* **Daylight Efficiency Tracker:** Audits aggregate daylight visibility balances to track clear sunny conditions vs heavy cloud layers.
* **End-of-Session Analytics Dashboard:** Consolidates daily data arrays into clear statistical summaries showing totals and monthly maximums.
