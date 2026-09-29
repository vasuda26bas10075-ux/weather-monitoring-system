# 🌦️ Weather Analytics System

A structured, modular Python application designed to collect, classify, and analyze daily localized weather indicators—including **rainfall metrics**, **temperatures**, and **sunshine durations**—over a monthly tracking window. 

---

## 📁 System Architecture & Directory Structure

To meet clean architectural standards and codebase decoupling requirements, the software is organized into distinct, modular functional layers:

```text
├── main.py                # Main orchestration layer & execution entry point
├── weather_input.py       # Calendar parameters, validation, and leap year checks
├── rainfall_mod.py        # Rainfall capture, threshold processing, and alerts
├── sunshine_mod.py        # Temperature and sunshine duration classifications
├── analytics_mod.py       # Math operations (totaling, finding peak max values)
├── test_suite.py          # Automated verification script for unit validations
```

---

## 🛠️ Technologies & Tools Used

* **Programming Language:** Python 3.x
* **Version Control:** Git & GitHub
* **Development Environment:** Google Colab / Standard IDE

---

## ✨ Features & Functional Modules

1. **Date & Calendar Automation (`weather_input.py`):** Automatically maps monthly calendar sizes and dynamically handles leap-year corrections for February. 
2. **Climate Classification Engines (`rainfall_mod.py` & `sunshine_mod.py`):** Instantly sorts raw metrics into distinct warning tiers (e.g., *"extremely heavy rain"*, *"moderately hot day"*, *"partially cloudy"*) using logical switch hierarchies.
3. **Data Summarization Core (`analytics_mod.py`):** Computes monthly statistics including aggregate volume totals and maximum peak event detection.

---

## ⚙️ Non-Functional Requirements (Architectural Standards)

As per project parameters, this architecture implements four core non-functional requirements:
* **Maintainability:** Separation of inputs, analysis, and execution scripts ensures single-responsibility updates.
* **Error Handling Strategy:** Built-in loop validation traps incorrect string inputs (like misspelled months) to prevent application crashes.
* **Usability:** Clear interactive shell prompts with date labels (`i / month / year`) guide predictable user workflows.
* **Resource Efficiency:** Avoids heavy third-party dependencies by relying strictly on core Python libraries, optimizing execution speed and runtime efficiency.

---

## 🚀 Installation & Running Guide

### Prerequisites
Ensure you have **Python 3.x** installed on your workstation.

### Step 1: Clone the Repository
```bash
git clone https://github.com
cd weather-analytics-system
```

### Step 2: Run the Application
Execute the central entry script to start the interactive wizard:
```bash
python main.py
```

---

## 🧪 Testing Instructions

To confirm the accuracy of data flows and boundary thresholds, trigger the automated verification file:

```bash
python test_suite.py
```
* **Input Validation Test:** Verifies that out-of-bounds strings or typos inside month prompts are caught gracefully.
* **Logic Calculation Test:** Validates that standard leap year equations evaluate February constraints exactly.

