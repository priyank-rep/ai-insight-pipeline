# AI Insight Pipeline

Automated anomaly detection and insight generation pipeline for marketing analytics data.

- Simulates 5 years of daily marketing data with seeded anomalies
- Detects anomalies using Facebook Prophet (95% confidence interval)
- Forecasts 90 days forward using the same fitted model
- Generates plain-English insight narratives using Groq LLM (LLaMA 3.3 70B)
- Builds a styled HTML email report and delivers it via Gmail SMTP
- Runs automatically every Monday via GitHub Actions — fully automated, zero manual intervention

## Pipeline

Data Simulation → Anomaly Detection → Forecasting → LLM Narratives → Email Delivery

## Tech Stack

Python, pandas, Facebook Prophet, Groq API, GitHub Actions, Gmail SMTP

## Status

Complete — Days 1 through 3 finished. All notebooks committed, GitHub Actions workflow verified working.

## Structure

notebooks/   - Jupyter notebooks (data simulation, anomaly detection, narrative generation)
data/        - Generated CSVs and HTML reports
.github/     - GitHub Actions workflow for weekly automated runs
