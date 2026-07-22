---
title: "Week 11 Worklog"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

{{% notice warning %}}
 **Note:** The following content records the learning and implementation activities completed during the week and is intended for the personal worklog report.
{{% /notice %}}

### Week 11 Objectives:
- Implement system monitoring using Amazon CloudWatch.
- Enhance application security using AWS WAF.
- Perform final testing on the RecruitPro system.

### Tasks carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 06/26/2026 | Explored CloudWatch Metrics and Logs for EC2, RDS, and ALB. | 06/26/2026 | 06/26/2026 | CloudWatch Overview |
| 06/27/2026 – 06/28/2026 | Created a custom CloudWatch Dashboard to monitor EC2 CPU Utilization and DB Connections. | 06/27/2026 | 06/28/2026 | Dashboard configurations |
| 06/29/2026 | Set up CloudWatch Alarms to send email notifications (via SNS) if CPU exceeds 80%. | 06/29/2026 | 06/29/2026 | AWS SNS & CloudWatch |
| 06/30/2026 – 07/01/2026 | Configured an AWS WAF (Web Application Firewall) Web ACL and attached it to CloudFront. | 06/30/2026 | 07/01/2026 | AWS WAF Rules |
| 07/02/2026 | Conducted a system test: uploading files, retrieving data, and checking WAF blocking rules. | 07/02/2026 | 07/02/2026 | Application Testing |

### Week 11 Achievements:
- Built a proactive monitoring solution to keep track of system health automatically.
- Added a crucial layer of security by filtering malicious web requests with AWS WAF.
- Ensured the RecruitPro system was fully functional, stable, and secure.