# Tableau_Network_Dashboard

This project is a simple, offline tool built to help small businesses analyze their past network activity. It focuses on identifying patterns in failures, security incidents, and performance issues—without needing complex setups or expensive real-time monitoring tools. Everything runs on your local machine, so your data stays secure and in your control.

## Project Overview

Many small businesses don’t have access to advanced network monitoring systems. These tools are often costly, require technical expertise, or rely on constant internet access. That makes it hard for teams to understand what went wrong and how to prevent it in the future.

This dashboard bridges that gap. It gives users an easy way to upload network log files, process the data, and get clear insights through charts and summaries. It’s simple, secure, and doesn’t need a tech team to run.

### What it offers:
	•	Offline access for full data privacy
	•	Easy setup, no advanced skills required
	•	Automatic issue classification (Failure, Security, Performance)
	•	Clean visuals and summaries anyone can understand

## How It Works
To use the system, just upload a CSV file with your network logs. It should include things like timestamps, device names, and event types.

The system will:
	•	Clean the data and fix formatting issues
	•	Classify events into relevant categories
	•	Save everything to a local SQLite database
	•	Analyze trends across time and devices
	•	Show you results through easy-to-read dashboards
	•	Let you export a summary report if needed

## Dashboard Highlights

The tool includes two main dashboard views:

1. Severity & Resolution Dashboard
Focuses on how many issues occurred, how long they lasted, and how severe they were.
Includes:
	•	3,150 total cases
	•	48.8% resolved
	•	92.6 minutes average duration
	•	19.5% marked critical
With scatter plots, IP-level breakdowns, and severity maps.

2. Network Health Dashboard
Shows when and where problems happened.
Features:
	•	Hourly heatmaps to spot peak problem times
	•	Trends by date and device
	•	Top 10 problematic devices
	•	Event severity breakdown

These views make it easy to understand what’s happening in your network at a glance.

## Technology Used

This system is built using simple but powerful tools:
	•	Python 3.11 for scripts and automation
	•	pandas for data processing
	•	SQLite for storing data locally
	•	Matplotlib for visuals
	•	Tableau (optional) for enhanced dashboards

## Privacy & Security

All your data stays local. The system doesn’t connect to the internet or upload anything to the cloud. This makes it perfect for businesses that care about privacy or operate in offline environments.

It’s reliable, secure, and easy to manage—even without a dedicated IT team.
