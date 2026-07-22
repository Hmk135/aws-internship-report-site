---
title: "Week 7 Worklog"
date: 2026-05-29
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---


### Week 7 Objectives:
- Design a secure, custom VPC network for the RecruitPro project.
- Implement the 3-tier architecture with Public, Private App, and Private DB subnets.
- Establish correct routing using Internet and NAT Gateways.

### Tasks carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 05/29/2026 | Created `RecruitPro-VPC` with CIDR `10.10.0.0/16` in the `ap-southeast-1` region. | 05/29/2026 | 05/29/2026 | AWS VPC settings |
| 05/30/2026 | Provisioned 2 Public Subnets, 2 Private App Subnets, and 2 Private DB Subnets across two AZs. | 05/30/2026 | 05/30/2026 | Subnet planning sheet |
| 05/31/2026 | Attached an Internet Gateway (IGW) to the VPC and created a NAT Gateway with an Elastic IP. | 05/31/2026 | 05/31/2026 | AWS Networking Guide |
| 06/01/2026 – 06/02/2026 | Configured the Public Route Table (to IGW) and Private Route Tables (to NAT Gateway). | 06/01/2026 | 06/02/2026 | Route Table configurations |
| 06/03/2026 | Created the core Security Groups for ALB (Public), EC2 (Private), and RDS (Private). | 06/03/2026 | 06/03/2026 | Security Group policies |
| 06/04/2026 | Verified subnet associations and ensured DB subnets had no outbound internet access. | 06/04/2026 | 06/04/2026 | VPC reachability analyzer |

### Week 7 Achievements:
- Successfully built a resilient, isolated network foundation for RecruitPro.
- Understood how to shield internal application servers and databases from direct public access.
- Correctly chained Security Groups so that RDS only accepts traffic from the EC2 backend.