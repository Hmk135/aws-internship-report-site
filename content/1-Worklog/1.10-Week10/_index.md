---
title: "Week 10 Worklog"
date: 2026-06-19
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

{{% notice warning %}}
 **Note:** The following content records the learning and implementation activities completed during the week and is intended for the personal worklog report.
{{% /notice %}}

### Week 10 Objectives:
- Make the private application accessible to the public securely.
- Configure an Application Load Balancer (ALB).
- Integrate CloudFront to optimize content delivery globally.

### Tasks carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 06/19/2026 | Created a Target Group pointing to the private Backend EC2 instance (port 8080). | 06/19/2026 | 06/19/2026 | Target Group configuration |
| 06/20/2026 – 06/21/2026 | Deployed an Application Load Balancer in the Public Subnets and attached the Target Group. | 06/20/2026 | 06/21/2026 | ALB Setup |
| 06/22/2026 | Verified that the application APIs could be accessed successfully via the ALB DNS name. | 06/22/2026 | 06/22/2026 | Postman / Browser |
| 06/23/2026 – 06/24/2026 | Created a CloudFront Distribution using the ALB as the origin server. | 06/23/2026 | 06/24/2026 | CloudFront Documentation |
| 06/25/2026 | Adjusted CloudFront cache behaviors and allowed specific HTTP methods (GET, POST). | 06/25/2026 | 06/25/2026 | Caching strategies |

### Week 10 Achievements:
- Completed the public exposure layer of the 3-tier architecture.
- Successfully routed external internet traffic securely down to the private EC2 via ALB.
- Leveraged CloudFront Edge locations (as learned in Community Day) to speed up application delivery.