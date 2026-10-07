# Fan Yupei — Project Portfolio

Public projects are grouped by the problem they solve. Each result distinguishes measured behavior from open quality questions.

## Applied AI products

### Local Lecture Copilot

**Local speech AI · Electron, whisper.cpp, Ollama · NTU team project** · [Source](https://github.com/FAN0020/local-lecture-copilot)

This lecture workspace records or imports audio, keeps a reviewable transcript, supports bilingual reading, and creates course-grounded study artifacts. My featured contribution is the Version C/C6 branch: conservative, source-bounded terminology repairs that preserve the existing transcript baseline and reject unsupported edits.

**Evidence.** The current source passes 395 automated tests. A local 10.5-minute Base Whisper run completed 66/66 chunks at 0.620 seconds average decode time per chunk. A fresh real-speech smoke completed three provisional and three user-requested revised segments, then drained all inference work. See [latest verification](https://github.com/FAN0020/local-lecture-copilot/blob/main/docs/latest-verification.md) and [measured performance](https://github.com/FAN0020/local-lecture-copilot/blob/main/docs/performance-validation-2026-09-08.md).

**Limits.** The live speech runs use pinned English fixtures on one Apple Silicon Mac. They do not certify broad transcription accuracy. On 20 fixed C6 slices, proxy WER moved from 0.3271 to 0.3243 against a saved Whisper Large-v3 transcript that is not human-verified ground truth. This is a modest proxy result, not an accuracy claim. The project is a team assignment and the public README identifies that context.

### ServiceScribe — Field Reporting Agent

**Source-grounded field reporting · Node.js, whisper.cpp, retrieval, deterministic validation** · [Source](https://github.com/FAN0020/newway-hvac-report-agent)

Built a technician-reviewed workflow from voice statement to confirmed service report: preserve raw speech, suggest domain terminology corrections, extract source-bound facts, ask about missing fields, validate report claims, then bind confirmation to the exact report version. The MVP workflow is verified; field-speech quality and production deployment remain unverified.

**Evidence.** A fresh rerun of the seven frozen synthetic Bus/Rail extraction cases achieved 100% expected-field recall with zero frozen safety-gate failures. This measures deterministic text-to-field extraction, not field ASR accuracy. See the [method and results](https://github.com/FAN0020/newway-hvac-report-agent/blob/main/docs/SBS_EXTRACTION_EVALUATION.md).

## Workflow automation and services

| Project | Classification | Outcome |
| --- | --- | --- |
| [**Local Outlook Group Mailer**](https://github.com/FAN0020/group_email) | Human-reviewed workflow automation | **38/38 mocked tests passed.** Resolves authorised roster identities and prepares an Outlook BCC draft. Ambiguous matches stay for review; sending remains manual. |
| [**ClassGuruAI Payment Service**](https://github.com/FAN0020/CG_payment_service) | Backend service · TypeScript, Fastify, SQLite, Stripe | **Type-check and build passed.** Subscription billing and credit APIs with JWT authentication, idempotent webhooks, Docker, and OpenAPI docs. Live Stripe and native database behavior were not exercised by these checks. |

## Experience

**AI Software Engineer Intern — Fling AI** · January–July 2025
Improved warehouse counting accuracy from approximately 70% to 94%+ through YOLOv7/YOLOv11 fine-tuning and dataset-quality improvements. Built reproducible Docker/SageMaker workflows and live counting interfaces.

[LinkedIn](https://www.linkedin.com/in/fan-yupei-0522---)
