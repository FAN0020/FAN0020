# Fan Yupei

I build applied AI products with reviewable outputs, explicit evidence, and clear limits. I am an MSc Enterprise Artificial Intelligence candidate at Nanyang Technological University, with a Computer Science degree and a Data Science specialisation.

## Contents

| Section | What you’ll find |
| --- | --- |
| [Applied AI products](#applied-ai-products) | Local speech, field reporting, and multimodal creation |
| [Agent research and evaluation](#agent-research-and-evaluation) | Reproducible tool-change comparisons |
| [Workflow automation and services](#workflow-automation-and-services) | Human-reviewed automation and backend engineering |
| [Agent skills](#agent-skills) | Reusable workflows for UI, animation selection, history, and academic notes |
| [Experience](#experience) | Applied AI engineering internship |
| [Education](#education) | NTU degrees |
| [Toolkit](#toolkit) | Methods and technologies |
| [Full project notes](PORTFOLIO.md) | Methods, evaluation details, and limitations |

## Applied AI products

| Project | Classification | Outcome and evaluation |
| --- | --- | --- |
| [**Story Compiler Studio**](https://github.com/FAN0020/Smaller_Agentic_Story_Compiler) | Local multimodal creation · Python, React, FLUX, LTX-Video | Text stories become a source-grounded series bible, reviewer-approved visual references, episode plans, and 1–4 minute videos. A **60.02-second local take** completed with 15 generated clips and captions; planning needed reviewer correction, and visual quality remains unapproved. [Verification](https://github.com/FAN0020/Smaller_Agentic_Story_Compiler/blob/main/docs/implementation/VERIFICATION.md). |
| [**Local Lecture Copilot**](https://github.com/FAN0020/local-lecture-copilot) | Local-first speech AI · Electron, whisper.cpp, Ollama · NTU team project; my work is the Version C/C6 branch | **395 tests passed**. A measured 10.5-minute Base run completed 66/66 chunks at 0.620 s average decode time. On 20 fixed C6 slices, proxy WER moved 0.3271 → 0.3243; this compares against an unverified Large-v3 transcript, not human ground truth. [Latest verification](https://github.com/FAN0020/local-lecture-copilot/blob/main/docs/latest-verification.md). |
| [**ServiceScribe**](https://github.com/FAN0020/newway-hvac-report-agent) | Source-grounded field reporting · Node.js, whisper.cpp, retrieval | **7 frozen synthetic cases: 100% expected-field recall, 0 frozen safety-gate failures.** Technician-reviewed report workflow. Field-speech quality and production deployment remain unverified. [Evaluation](https://github.com/FAN0020/newway-hvac-report-agent/blob/main/docs/SBS_EXTRACTION_EVALUATION.md). |

## Agent research and evaluation

| Project | Classification | What the evidence supports |
| --- | --- | --- |
| [**Tool Harness Adaptation**](https://github.com/FAN0020/pe6203-tool-harness-adaptation) | NTU team research · agent tool-change evaluation | A reproducible comparison of No Update, Full Rewrite, and Selective Patch across **27 scored task-method runs**. Later variant results and retry-inclusive summaries are archived separately; differing protocols do not support a simple superiority ranking. [Methods and current results](https://github.com/FAN0020/pe6203-tool-harness-adaptation#readme). |

## Workflow automation and services

| Project | Classification | Reviewer shortcut |
| --- | --- | --- |
| [**Local Outlook Group Mailer**](https://github.com/FAN0020/group_email) | Human-reviewed workflow automation · Python, Playwright, SQLite | **38/38 mocked tests passed.** Roster identity matching → reviewed Outlook BCC draft; sending stays manual. [Test scope](https://github.com/FAN0020/group_email#automated-tests). |
| [**ClassGuruAI Payment Service**](https://github.com/FAN0020/CG_payment_service) | Backend service · TypeScript, Fastify, SQLite, Stripe | **Type-check and build passed.** Subscription billing, credits, JWT authentication, and idempotent webhooks. Live payment behavior was not evaluated. [Verification](https://github.com/FAN0020/CG_payment_service/blob/main/docs/verification-2026-10-07.md). |

## Agent skills

I turn recurring product and research workflows into reusable agent skills with explicit evidence requirements and clear limits.

| Skill | Main capability | Design focus |
| --- | --- | --- |
| [**Product UI QA**](https://github.com/FAN0020/evidence-driven-agent-skills/tree/main/skills/product-ui-qa) | Review and verify product interfaces | Component necessity, meaningful UI states, and an adversarial completion review |
| [**Animated Component Picker**](https://github.com/FAN0020/evidence-driven-agent-skills/tree/main/skills/animated-component-picker) | Choose animation components for a web project | Match task, stack, style, and access; load the comparison catalog only when needed |
| [**Visual Convergence**](https://github.com/FAN0020/evidence-driven-agent-skills/tree/main/skills/visual-convergence) | Refine an existing UI toward an approved reference | Token correctness, perceptual composition, and project-specific visual decisions |
| [**Project History Archivist**](https://github.com/FAN0020/evidence-driven-agent-skills/tree/main/skills/project-history-archivist) | Reconstruct accessible conversations and development into an auditable DOCX | Inventory reconciliation, chronology, and Git corroboration |
| [**Software History Lessons**](https://github.com/FAN0020/evidence-driven-agent-skills/tree/main/skills/software-history-lessons) | Turn repository history into reusable engineering knowledge | Evidence, transfer conditions, target-product recommendations, and validation |
| [**Adaptive Academic Note Architect**](https://github.com/FAN0020/adaptive-academic-note-architect) | Reconstruct comprehensive academic notes from mixed sources | Bilingual explanations, source coverage, underlined takeaways, and navigable documents |

[Collection and installation](https://github.com/FAN0020/evidence-driven-agent-skills) · [Animation selection catalog](https://github.com/FAN0020/evidence-driven-agent-skills/blob/main/skills/animated-component-picker/references/catalog.md) · [Original skill comparisons](https://github.com/FAN0020/evidence-driven-agent-skills/blob/main/docs/comparisons.md). These describe workflow capabilities and task fit; comparative output quality has not been benchmarked.

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
