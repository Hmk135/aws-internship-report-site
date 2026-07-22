---
title: "Week 5 Worklog"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---



### Week 5 Objectives:
- Understand high availability concepts in cloud computing.
- Learn to distribute incoming traffic using an Application Load Balancer (ALB).
- Configure a Target Group for multiple EC2 instances.

### Tasks carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 05/15/2026 | Studied the Elastic Load Balancing (ELB) types and Target Groups. | 05/15/2026 | 05/15/2026 | AWS ELB Guide |
| 05/16/2026 – 05/17/2026 | Launched two separate EC2 instances in different Availability Zones for testing. | 05/16/2026 | 05/17/2026 | AWS EC2 Console |
| 05/18/2026 | Configured user-data scripts to display the unique hostname on each EC2 web server. | 05/18/2026 | 05/18/2026 | Shell scripting |
| 05/19/2026 – 05/20/2026 | Created a Target Group, registered the two EC2 instances, and verified health checks. | 05/19/2026 | 05/20/2026 | AWS Console |
| 05/21/2026 | Provisioned an Application Load Balancer and tested traffic distribution via its DNS name. | 05/21/2026 | 05/21/2026 | Web Browser checks |

### Week 5 Achievements:
- Grasped the importance of distributing workloads across Availability Zones.
- Successfully configured an ALB to route HTTP traffic evenly across multiple backend servers.
- Learned how Health Checks automatically prevent traffic from going to failed instances.