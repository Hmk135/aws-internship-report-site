---
title: "Week 8 Worklog"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---



### Week 8 Objectives:
- Deploy the database tier securely within the custom VPC.
- Launch the backend EC2 server in the private subnet.
- Establish a connection between the backend and the database.

### Tasks carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 06/05/2026 | Created a DB Subnet Group combining the two private DB subnets inside RecruitPro-VPC. | 06/05/2026 | 06/05/2026 | RDS Console |
| 06/06/2026 – 06/07/2026 | Launched the production RDS MySQL instance attached to the private DB subnets. | 06/06/2026 | 06/07/2026 | AWS Management Console |
| 06/08/2026 | Deployed a Bastion Host in the Public Subnet to access the private network. | 06/08/2026 | 06/08/2026 | SSH Agent forwarding |
| 06/09/2026 – 06/10/2026 | Launched the Backend EC2 instance in the Private App Subnet and connected via the Bastion Host. | 06/09/2026 | 06/10/2026 | Network routing |
| 06/11/2026 | Installed MySQL Client on the Backend EC2 and successfully tested the connection to the RDS endpoint. | 06/11/2026 | 06/11/2026 | Linux CLI |

### Week 8 Achievements:
- Successfully deployed a fully private database that is inaccessible from the outside world.
- Mastered the concept of a Bastion Host (Jump Box) for secure internal management.
- Verified the internal connectivity between the Application tier and the Database tier.