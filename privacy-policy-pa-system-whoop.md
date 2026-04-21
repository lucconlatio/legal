# Privacy Policy — Conlatio PA (Whoop Integration)

**Last updated:** April 2026
**Application name:** Conlatio PA
**Developer:** Luc Wynne / Conlatio FZ-LLC

---

## Overview

Conlatio PA is a private personal assistant integration built for internal use by the developer only. It connects to the WHOOP API to retrieve health and fitness data for the purpose of generating a personalised daily briefing. This application is not available to the public and has no external users.

---

## Data Collected

This application accesses the following data from the WHOOP API, with the explicit authorisation of the account holder:

- Recovery data (recovery score, heart rate variability, resting heart rate)
- Sleep data (sleep performance, sleep duration, sleep stages)
- Strain data (daily strain score)
- Cycle data (cycle timing and timezone offset)

---

## How Data Is Used

WHOOP data is used solely to generate a personalised morning briefing delivered via private Slack message to the account holder. Specifically:

- Recovery score, HRV, and sleep data are used to provide a daily physical readiness summary
- Timezone offset from cycle data is used to correctly assign each record to the appropriate local date
- No data is used for commercial purposes, advertising, or any purpose beyond the personal morning briefing

---

## Data Storage

WHOOP data is stored in a private Supabase database accessible only to the developer. Data is retained indefinitely for personal trend analysis. No data is stored on third-party servers beyond Supabase and the self-hosted n8n instance used for workflow automation, both of which are privately controlled.

---

## Data Sharing

WHOOP data is never shared with third parties. It is not sold, licensed, distributed, or disclosed to any external party for any reason.

---

## Data Access

Only the developer (Luc Wynne) has access to the stored WHOOP data. No other individuals, employees, or systems have access to this data.

---

## Data Deletion

The account holder (who is also the developer) may delete all stored WHOOP data at any time by removing the relevant records from the Supabase database. Access to the WHOOP API can be revoked at any time via the WHOOP developer dashboard.

---

## Security

Data is transmitted over HTTPS at all times. The Supabase database is protected by access controls. OAuth tokens are stored securely in the n8n credentials store and are never exposed in logs or application code.

---

## Contact

For any questions regarding this privacy policy or data handling:

**Luc Wynne**
Conlatio FZ-LLC
luc@conlatio.eu
