## Project Summary

**Payment Journey Improvement** is a Lean Six Sigma Green Belt project focused on improving the payment experience in an e-commerce application. The project addressed customer complaints, lost sales, payment delays, failed or pending transactions, and checkout cancellations caused by friction in the payment journey.

The project followed the DMAIC methodology: Define, Measure, Analyze, Improve, and Control. It used Voice of Customer analysis, SIPOC, swimlane diagrams, data collection planning, measurement validation, fishbone analysis, 5 Whys, value-add/cycle-time analysis, risk management, and control planning to identify and resolve root causes.

### Problem

Customers were experiencing long payment sessions, unclear payment status communication, payment cancellations, and cases where payments were completed but transaction responses were not received during the active session. This led to customer frustration, lost sales, and lower application ratings.

### Root Causes Identified

- Web-hosted checkout loaded through iframe, increasing UI rendering time
- Payment sessions were initiated through the backend server, increasing dependency and latency
- Multiple client-server-gateway network round trips created delays
- Payment response timing was not clearly communicated to customers
- Weak retry/error handling caused pending payment states and customer uncertainty
- Web-based card entry and redirect-based authentication created additional friction

### Solution Implemented

- Migrated from web-hosted checkout to native SDK checkout integration
- Added payment gateway callback/webhook handling for transaction confirmation
- Reduced server dependency by allowing the device/application to initiate payment while keeping the server informed
- Improved payment-status communication and customer-facing visuals during checkout
- Added monitoring, alerting, and control plans to track payment journey health

### Results

- Improved payment acceptance from **77% to 92%**
- Reduced payment pending/failure rate from **12% to 1%**
- Reduced average payment session time from **4.3 minutes to 2.52 minutes**
- Reduced average payment response time from **5.30 minutes to 2.79 minutes**
- Improved app satisfaction from **3.1/5 to 4.2/5**
- Improved NPS from **4/10 to 7/10**
- Delivered a reported **7% monthly sales increase**
- Reduced payment-related customer complaints by **67%**

### Value of the Project

This project demonstrates practical experience in process improvement, payment journey optimization, KPI tracking, root-cause analysis, cross-functional collaboration, and customer experience improvement. It highlights the ability to convert operational data into measurable business impact through structured Lean Six Sigma methodology.
