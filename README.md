# missed-call-analysis

Missed Call Follow Up Analysis for a Sample Auto Shop

## Project Overview

This project explores patterns in missed calls and customer follow-up metrics for a sample automotive repair shop. Using synthetic data, the analysis evaluates communication efficiency, response times, and customer conversion (appointment confirmation) rates following missed calls.

## Business Question

* What patterns appear in missed calls and subsequent customer follow-ups?
* How quickly are follow-up messages sent, and what impact does response time have on appointment confirmations?
* What proportion of missed calls lead to successful conversions?

## Dataset Schema

The project utilizes a synthetic dataset (`missed_call_data.csv`) structured with the following attributes:

| Field Name | Description |
| :--- | :--- |
| `call_id` | Unique identifier for each call record |
| `business_id` | Unique identifier for the shop location |
| `call_time` | Timestamp when the call occurred |
| `call_status` | Status of the call (`missed`, `answered`) |
| `message_delivered` | Boolean flag indicating if an automated or manual follow-up was sent |
| `customer_replied` | Boolean flag indicating if the customer replied |
| `reply_minutes` | Time in minutes elapsed before the customer replied |
| `appointment_confirmed` | Boolean flag indicating if an appointment was successfully booked |

## Tools & Environment

* **Language:** Python
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`
* **Databases / Querying:** SQL / SQLite
* **Environment:** Kaggle Notebooks / Jupyter Notebooks
* **Version Control:** Git & GitHub

## Data Preparation & Cleaning

* Handled missing values (e.g., null values in `reply_minutes` for customers who did not reply).
* Audited records for duplicate `call_id` entries.
* Validated formatting types and distributions across categorical and numeric fields.

## Methodology & Analysis

* **Audit Workflow:** Evaluated existing missed-call follow-up processes to identify broken or unfinished logic paths.
* **Exploratory Data Analysis (EDA):** Aggregated call volumes by time of day and day of week to identify peak missed-call hours.
* **Response Dynamics:** Evaluated conversion rates based on follow-up speed (`reply_minutes`).

## Progress & Study Log

Tracked via internal daily log files:
* [`STUDY_LOG.md`](./STUDY_LOG.md) — Daily learning objectives, tasks implemented, and unresolved challenges during development.
* [`WEEKLY_TRACKER.md`](./WEEKLY_TRACKER.md) — High-level weekly progress summaries.