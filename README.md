# Network Health Dashboard – Offline Log Analyzer

This project was built to help anyone—from small teams to solo operators—make sense of their past network issues using the log files they already have. It’s a simple, offline tool that runs locally, combining Python (via Google Colab) for data processing and Tableau for visualizing the results in a way that’s actually useful.

No complex setup. No cloud dependency. Just upload your logs and get insights.

---

## Why This Project Exists

Not every business has the budget or bandwidth for a full-fledged network monitoring system. But that doesn’t mean they should be left in the dark when it comes to understanding why their network failed—or which devices keep causing trouble.

This project was created to fill that gap. It’s designed to be lightweight, practical, and easy enough for non-technical users. Just bring your CSV logs, and the system handles the rest—cleaning the data, categorizing issues, and turning everything into a clean, readable dashboard.

---

## What It Does

- Upload your network log file (CSV format)
- Automatically clean and organize the data
- Classify each event as a **Failure**, **Security Issue**, or **Performance Warning**
- Save the processed results in a local SQLite database
- Analyze patterns across time, device, and severity
- Visualize insights through a Tableau dashboard
- Export a simple CSV summary report for future reference

---

## How It Works

1. Open the Google Colab notebook (link below)
2. Upload your CSV log file
3. The Python script:
   - Cleans missing data and fixes formatting
   - Tags each log by issue type
   - Stores everything locally in SQLite
4. Tableau reads that data and shows:
   - Which devices had the most trouble
   - When most issues occurred
   - What kinds of problems were most common

You can explore trends by hour, day, device, or severity—all in just a few clicks.

---

## What You'll See in the Dashboard

### Severity & Resolution View
- Total number of logged issues
- How many were resolved
- Average time to resolution
- Share of critical events
- Visuals like scatter plots and IP-level breakdowns

### Network Health View
- Heatmaps showing issue frequency by hour
- Trends over days and weeks
- Breakdown of issue types and affected devices
- Top 10 most problematic endpoints

---

## Built With

- **Python 3.11** in Google Colab  
- **pandas** for data cleaning  
- **SQLite** for lightweight, local data storage  
- **Matplotlib** for quick visuals  
- **Tableau** for final dashboard design  

---

## Keeping It Local

The whole system runs offline. Your log files, processed data, and reports stay on your machine. This makes it a good fit for teams with sensitive data or limited internet access.

---

## Try It Yourself

Want to see how it works?  
Just open the notebook, upload your logs, and follow the steps.

👉 [Run the Google Colab Notebook](https://colab.research.google.com/drive/1D8A4IF_H1do1qK6bs6CyE594et4tuxdA?usp=share_link)

---

## Project Status

The tool is fully working and tested with sample log data. That said, there’s always room to grow. A few potential next steps include:
- Adding user roles or login features
- Making the dashboard even more interactive
- Introducing smart event classification using machine learning

---

Feel free to clone it, improve it, or use it as a base for your own internal projects. Feedback and suggestions are always welcome.
