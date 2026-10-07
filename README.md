# Fan Yupei

I build applied AI products with reviewable outputs, explicit evidence, and clear limits. I am an MSc Enterprise Artificial Intelligence candidate at Nanyang Technological University, with a Computer Science degree and a Data Science specialisation.

## Contents

| Section | What you’ll find |
| --- | --- |
| [Applied AI products](#applied-ai-products) | Local AI systems and measured results |
| [Workflow automation and services](#workflow-automation-and-services) | Human-reviewed automation and backend engineering |
| [Experience](#experience) | Applied AI engineering internship |
| [Education](#education) | NTU degrees |
| [Toolkit](#toolkit) | Methods and technologies |
| [Full project notes](PORTFOLIO.md) | Methods, evaluation details, and limitations |

## Applied AI products

| Project | Classification | Outcome and evaluation |
| --- | --- | --- |
| [**Local Lecture Copilot**](https://github.com/FAN0020/local-lecture-copilot) | Local-first speech AI · Electron, whisper.cpp, Ollama · NTU team project; my work is the Version C/C6 branch | **395 tests passed**. A measured 10.5-minute Base run completed 66/66 chunks at 0.620 s average decode time. On 20 fixed C6 slices, proxy WER moved 0.3271 → 0.3243; this compares against an unverified Large-v3 transcript, not human ground truth. [Latest verification](https://github.com/FAN0020/local-lecture-copilot/blob/main/docs/latest-verification.md). |
| [**ServiceScribe**](https://github.com/FAN0020/newway-hvac-report-agent) | Source-grounded field reporting · Node.js, whisper.cpp, retrieval | **7 frozen synthetic cases: 100% expected-field recall, 0 frozen safety-gate failures.** Technician-reviewed report workflow. Field-speech quality and production deployment remain unverified. [Evaluation](https://github.com/FAN0020/newway-hvac-report-agent/blob/main/docs/SBS_EXTRACTION_EVALUATION.md). |

## Workflow automation and services

| Project | Classification | Reviewer shortcut |
| --- | --- | --- |
| [**Local Outlook Group Mailer**](https://github.com/FAN0020/group_email) | Human-reviewed workflow automation · Python, Playwright, SQLite | **38/38 mocked tests passed.** Roster identity matching → reviewed Outlook BCC draft; sending stays manual. [Test scope](https://github.com/FAN0020/group_email#automated-tests). |
| [**ClassGuruAI Payment Service**](https://github.com/FAN0020/CG_payment_service) | Backend service · TypeScript, Fastify, SQLite, Stripe | **Type-check and build passed.** Subscription billing, credits, JWT authentication, and idempotent webhooks. Live payment behavior was not evaluated. [Verification](https://github.com/FAN0020/CG_payment_service/blob/main/docs/verification-2026-10-07.md). |

## Experience

**AI Software Engineer Intern — Fling AI** · January–July 2025  
Improved warehouse counting accuracy from approximately 70% to 94%+ through YOLOv7/YOLOv11 fine-tuning and dataset-quality improvements. Built reproducible Docker/SageMaker workflows and live counting interfaces.

## Education

**Nanyang Technological University**  
MSc in Enterprise Artificial Intelligence · August 2026–Present  
Bachelor of Computing in Computer Science, Honours · August 2021–March 2026  
Data Science specialisation

## Toolkit

- **AI:** LLM integration, RAG, prompt design, Whisper/ASR, PyTorch, computer vision, model evaluation
- **Engineering:** Python, JavaScript/TypeScript, React, Node.js, Electron, REST APIs, SQL
- **Automation and delivery:** UiPath, Playwright, Docker, GitHub Actions, AWS SageMaker
- **Product:** Discovery, requirements, roadmaps, Figma, user flows, MVP iteration

Interested in AI product engineering, applied AI, agentic automation, and technical product opportunities in Singapore.

[LinkedIn](https://www.linkedin.com/in/fan-yupei-0522---)
