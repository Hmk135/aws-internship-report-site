---
title: "Event 23/5/2026 - FCAJ Community Day"
date: 2026-05-23
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# My Experience at FCAJ Community Day

On May 23, 2026, I joined the FCAJ Community Day alongside a friend. The event featured a diverse lineup of presentations, touching on everything from AWS infrastructure (like CloudFront) to practical AI implementations (such as LLM determinism, context optimization, and enterprise multi-agent architectures). In this report, I will highlight the most valuable insights I gained and how I plan to apply them to my own work.

## Overview of Presentations

- Tịnh: **Context Is Everything**.
- Phạm Ngô Hải Anh: **Friendly AI Assistant with Amazon Quick**.
- Nguyễn Tuấn Thịnh: **From Edge to Origin**.
- Team VIB: **36 Hours with LotusHacks**.
- Đào Đức: **Non-Determinism of Deterministic LLM Settings**.
- Cát Vy: **Enterprise-Grade Multi-Agent System**.

## Key Insights and Learnings

### Prompting: Quality Trumps Quantity
I used to think that providing an AI with as much text as possible would yield the best results. However, this session highlighted that precision is far more important. A well-crafted context should only contain the specific goals, constraints, and necessary data. Overloading the prompt with irrelevant information not only wastes tokens but also distracts the model. The concept of a "Second AI Brain"—a retrieval system that fetches only highly relevant notes or docs before feeding them to the AI—was particularly inspiring for managing large-scale project documentation.

### The Importance of Data Access Controls in AI
The presentation on Amazon Quick showcased the power of enterprise AI assistants in handling tasks like scheduling, drafting emails, and summarizing meetings. However, the biggest takeaway for me was the critical need for security. An internal company AI must be strictly governed by role-based access controls to ensure users can only query information they are explicitly authorized to view.

### CloudFront as a Security and Performance Tool
This session was highly relevant to my work on RecruitPro. While I knew CloudFront was used for caching content at edge locations, I learned it is equally vital for security and cost optimization. By integrating with AWS WAF and AWS Shield, and by enforcing HTTPS, CloudFront acts as a robust shield, ensuring that the origin server is rarely exposed to direct internet traffic.

### Hackathon Strategy: Less is More
Team VIB shared their journey of building "UTMorpho" during the 36-hour LotusHacks event. They struggled with token limits, exhaustion, and unreliable AI outputs. Their breakthrough came when they stopped trying to build a massive feature set and instead zeroed in on perfecting one core editing feature. This taught me that delivering a single, polished, and working function is far better than presenting a buggy, over-complicated application.

### Unpredictability Even at Temperature Zero
One of the most surprising facts I learned is that setting an LLM's temperature to zero does not guarantee 100% identical responses every time. Factors like GPU architecture, parallel computing, and batching can introduce slight variations. Therefore, for production systems, we must rely on rigid constraints (like JSON formatting) and robust output validation rather than assuming the model's behavior is perfectly deterministic.

### Managing Enterprise Multi-Agent Workflows
Using a startup credit evaluation as a case study, this session demonstrated how different AI agents (handling finance, risk, team analysis, etc.) can collaborate under a "manager" agent. While this specialization speeds up complex tasks, deploying such a system in a real enterprise requires strict guardrails. You need comprehensive audit logs, data privacy measures, and human oversight—highlighting the massive gap between a simple AI demo and a production-ready system.

## Actionable Takeaways

- Feed AI models only highly targeted context, avoiding data dumps.
- Be explicit about desired outputs, formats, and constraints when prompting.
- Leverage CloudFront not just for speed, but to mask and protect the origin server.
- In time-constrained projects, prioritize building one rock-solid feature over many incomplete ones.
- Never assume an LLM's output is fixed; always validate the results programmatically.
- Ensure strict permission boundaries and auditing when deploying AI Agent tools.

## How This Applies to RecruitPro

The insights on CloudFront are immediately applicable to my RecruitPro project. I plan to reconfigure our caching strategies, restrict direct access to the backend origin, and explore AWS WAF integration. Additionally, when implementing AI features, I will adopt a much stricter approach to prompt structuring and output validation to ensure reliability.

## Proof of Attendance

![My photo at FCAJ Community Day](</images/4-EventParticipated/4.1-Event1/Picture1.png>)

![Photo taken during the event](</images/4-EventParticipated/4.1-Event1/picture2.jpg>)

## Conclusion

Attending the FCAJ Community Day was incredibly rewarding. It provided a perfect mix of cloud infrastructure best practices (CloudFront) and realistic AI development strategies (LLM behaviors and Multi-Agent governance). I now have a much clearer understanding that real-world AI requires rigorous control and validation, concepts I am eager to apply in my ongoing and future work.