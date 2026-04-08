### EdTech-Support-Responce-Metrics

- Domain: EdTech Analytics
- Objective: Evaluate the dynamics of the number of support requests, and how quickly the requests were handled
- Result: A Google Sheets report with metrics and visualisations
- Tech Stack: Google Sheets, Applied Statistics
- Link to Report: https://docs.google.com/spreadsheets/d/1zKcL79_O2u18Vc0h7FU5dbo54_ESlscu2WpENU8bTVQ/edit?usp=sharing 

Contents:
- [Context Overview](#1-context-overview)
- [Description of Data](#2-description-of-data)
- [Analysis Results (detailed, conclusions, and recommendtations)](#3-analysis-results)

#### 1. Context Overview
In this project I worked with data on requests received by the support team of Yandex Practicum's English language course for April and May 2024. The main objectives were to evaluate the dynamics of the number of support requests, and find out how quickly the requests were handled. Also there were some specific points that should appear in the report:
- total number of requests;
- median response time per request;
- median resolution time per request;
- difference in median response time between periods;
- difference in median resolution time between periods;
- distribution of requests by channel for each period and the difference between periods;
- first response time by channel for each period and the difference between periods.

#### 2. Description of Data:
- `ticket_id` — Unique identifier of the request
- `received_at` — Date and time when the request was registered in the system
- `request_channel` — Channel through which the request was submitted
- `attachments` — Number of attached files added to the request
- `status_change_date` — Date and time when the request was taken into processing
- `assigned_agent` — ID number of the support staff member who handled the request
- `first_response_time` — Time elapsed before the request received a response. The response could be automated and instant, in which case the field value is 0
- `first_response_date` — Date and time when the request received a response
- `resolution_time` — Time elapsed from the moment the request was submitted until it was resolved
- `resolved_on_first_response` — "Yes" if the request was resolved after the first response from the support team. "No" if additional messages were required
- `agent_reply_count` — Number of messages sent by the support staff member to resolve the request
- `customer_reply_count` — Number of messages sent by the author of the request
- `flow` — Tag for the request's topic

#### 3. Analysis results

Analysis showed that:
- The total number of support requests decreased by 9% in May comparing to April
- The median response time per request in May changed minorly (by 10 seconds)
- The median resolution time per request in May changed minorly (by ~20 seconds)
- The distribution of requests by channel in April and May are basically the same (The most popular channel is Telegram — 68% of requests; The least popular channel is VK — <1% of requests)
- First response time via Email increased by 30%
- First response time via VK decreased by 45%

Conclusions:
- decreased number of requests in May is normal, since there are long holidays in May in Russia
- response and resolution time stayed the same even during holidays, which is a win
- roughly 15% of requests come through Email, so increase in first response time might be a problem
  
Recommendations:
- convey additional analysis and look into response time via Emain (e.g., were there any technical problems, was there a shortage of agents, etc.)
