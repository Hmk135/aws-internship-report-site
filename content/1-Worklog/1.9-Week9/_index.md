---
title: "Week 9 Worklog"
date: 2026-06-12
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Week 9 Objectives:
- Prepare the Backend EC2 for the application runtime.
- Deploy the RecruitPro source code and dependencies.
- Grant the EC2 instance secure access to upload files to S3 via IAM Roles.

### Tasks carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 06/12/2026 | Created an IAM Role with S3 permissions and attached it to the Backend EC2 instance. | 06/12/2026 | 06/12/2026 | IAM Roles for EC2 |
| 06/13/2026 – 06/14/2026 | Installed Java (JDK) and necessary runtime dependencies on the Backend EC2. | 06/13/2026 | 06/14/2026 | Linux package manager |
| 06/15/2026 | Transferred the `.jar` build file and initial SQL scripts to the private EC2. | 06/15/2026 | 06/15/2026 | SCP / WinSCP |
| 06/16/2026 – 06/17/2026 | Imported the database schema into RDS and configured the app's `application.properties`. | 06/16/2026 | 06/17/2026 | Project Source Code |
| 06/18/2026 | Created a `systemd` service to run the Spring Boot application securely in the background. | 06/18/2026 | 06/18/2026 | systemd documentation |

### Week 9 Achievements:
- Eliminated the need for hardcoded AWS credentials by using secure IAM Roles for S3 access.
- Successfully started the backend application and verified it was running smoothly.
- Learned how to manage Linux background processes using `systemd`.