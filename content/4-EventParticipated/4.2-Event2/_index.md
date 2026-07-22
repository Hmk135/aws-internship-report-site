---
title: "Event 11/7/2026 - Security, Monitoring & Certification"
date: 2026-07-11
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Insights from the July 11 Event

On July 11, 2026, I attended another insightful event focusing on cloud certification, system monitoring, and AI-driven security. This session provided practical strategies for passing AWS exams and deep dives into securing modern web applications using autonomous agents.

## Overview of Presentations

- Speaker (Huy): **Inside The Exam: AWS Cloud Practitioner**.
- Nguyễn Huỳnh Sơn: **SLA and Monitoring - From SLA to Monitoring what really matters**.
- Thinh Nguyen: **Securing Your Web Apps With AWS Security Agent**.

## Key Insights and Learnings

### Cracking the AWS Cloud Practitioner Exam
The session provided valuable "Tips & Tricks" for the exam:
- **Elimination technique:** Questions often provide four answer choices, in which two are "made-up" services or completely irrelevant; eliminating those first increases your chances of getting the correct answer to 50%.
- **Don't overthink:** The Cloud Practitioner exam focuses on fundamental knowledge. If a question seems to require overly complex configuration, you're likely overthinking it, so choose the simplest answer.
- **Language pitfalls:** The English exam can be tricky, so it is recommended to highlight decisive terms immediately when reading questions, such as "Not", "Least cost", or "Most scalable".

### Meaningful Monitoring
Nguyễn Huỳnh Sơn emphasized shifting the focus from standard SLA numbers to monitoring metrics that actually matter to the system and business.

### Overcoming the Security Bottleneck
Thinh Nguyen highlighted that traditional manual penetration testing is time-consuming (taking weeks) and expensive (with high daily rates for specialized hackers). It is also inconsistent because coverage depends on the tester's mood or skill, resulting in high operational costs of around $20k for third-party assessments.

### AI-Powered Security with Frontier Agent
To solve this bottleneck, the "Frontier Agent" was introduced. It features:
- **Autonomous Reasoning:** Powered by Amazon Bedrock, it plans and executes security tasks without human intervention.
- **Full Lifecycle Coverage:** It handles Design Review, Code Security, and Active Penetration Testing.
- **Verifiable Findings:** Unlike LLM chatbots, it verifies vulnerabilities by attempting real exploitation.
- **Design Security Review:** You can upload Markdown docs or Terraform code to verify against Managed Packs (like PCI DSS, NIST CSF, AWS Well-Architected) to check if the design meets security "Requirements". This feature includes a Free Tier of 200 reviews/month.

### Limitations of AI Security Agents
Despite their capabilities, AI agents have critical limitations:
- **Auth Blocks:** Implementations like MFA, Biometrics, and mTLS will stop the agent in its tracks.
- **Logic Flaws:** Agents find it difficult to detect business-logic fraud without deep context.
- **Task-Hour Accumulation:** Complex apps burn hours fast, making monitoring mandatory.

## Actionable Takeaways
- Always highlight key constraints like "Least cost" or "Most scalable" when analyzing cloud problems or exam questions.
- Move beyond basic SLAs to monitor what truly matters for system health.
- Leverage automated Design Security Reviews against frameworks like AWS Well-Architected.
- Implement strong authentication blocks like MFA and Biometrics, as they are highly effective roadblocks against autonomous agents.

## How This Applies to RecruitPro
The exam strategies directly support my goal of achieving AWS certification. For RecruitPro, I will rethink our CloudWatch dashboards to monitor what truly matters rather than just checking basic uptime metrics. Furthermore, learning that MFA stops AI agents reinforces my decision to implement strict authentication for our administrative backend.

## Proof of Attendance
![My photo at FCAJ Community Day](</images/4-EventParticipated/4.2-Event2/Picture3.jpg>)

![Photo taken during the event](</images/4-EventParticipated/4.2-Event2/picture4.jpg>)

## Conclusion
This event perfectly balanced career development with advanced technical knowledge. It opened my eyes to the future of automated penetration testing and the enduring importance of foundational security practices like MFA.