# Fan Yupei Project Portfolio

I build applied AI products that make generated output inspectable and correctable. My recent work spans field reporting, story production, document question answering, local speech tools, and workflow automation. The projects below distinguish working software and retained evaluations from capabilities that still need real-world validation.

## Featured Projects

### Field Work Reporting Agent

**September 2026 onward · Local field-service reporting · Node.js, JavaScript, whisper.cpp, Ollama, retrieval, deterministic validation**

Field technicians often start with incomplete, noisy voice notes. This application records or accepts a statement, preserves the raw transcript, proposes terminology corrections for technician review, extracts source-bound service facts, asks for missing information, builds a domain-specific report, validates its claims, and requires confirmation of the exact final draft before export. The first vertical was HVAC; later knowledge scopes and report schemas cover bus, rail, power-grid, and oilfield scenarios.

**Problems and improvements.** Speech recognition can alter an asset identifier or a critical part name. In a retained rail voice example, `C751A` was transcribed as `Z751A`, and “door control module faulty” became “door control model 40.” The application presents corrections as unchecked suggestions; after the technician accepted both, the example yielded six extracted facts rather than two. Knowledge retrieval is isolated by domain, and retrieved manuals cannot by themselves become claims that a technician performed work or obtained a test result. Missing report modules lead to targeted questions, with answers recorded as technician-confirmed facts. Correction, fact, validation, and final report receipts are bound to their source artifacts and hashes so an altered or stale report cannot inherit an old approval.

**Engineering choices and scope.** The report is assembled from confirmed facts through a fixed workflow with an independent validator and a human confirmation gate. This avoids giving a language model authority to silently rewrite critical transcript values, infer service actions from reference material, or publish an unreviewed report. The accepted MVP workflow and an English Whisper provider smoke test are documented; Chinese HVAC accuracy, live two-device microphone use, and production deployment remain unverified.

### Agentic Story Compiler / Story Director V4

**September–October 2026 · Story-to-video planning and production · FastAPI, Python, SQLite, Ollama/Qwen, MFLUX, LTX/MLX, FFmpeg**

Story Director converts prose into a reviewable production plan: grounded source events and story facts, Director and design bibles, Episodes, Scenes, Shots, provider-specific prompts, generated Clips, and assembled Episode video. A creator can inspect and approve an exact plan before media production, then review the output in Create, Director Plan, Production, Watch, and Evaluate.

**Problems and improvements.** Long or ambiguous source material makes it easy for generated plans to invent facts, lose event order, or change character and prop state between Shots. The system asks models to select numbered source units, reconstructs exact quotations from original offsets, and rejects invalid or overlapping evidence before persistence. Scene and Shot contracts separate narrative purpose from camera and action instructions, while canonical identities and start/end states support continuity checks. Provider capability records and a prompt compiler test duration, geometry, references, and prompt size before expensive generation. Persisted versions, optimistic revisions, lineage, budgets, and bounded repair allow the smallest affected artifact to be retried while accepted work survives interruption.

**What changed or was set aside.** V3.1 produced an illustrated interactive reader; V4 deliberately uses linear Episode video as its final viewing unit and keeps V3.1 as a legacy baseline. Free-text provider prompts no longer serve as the canonical directing state. Model-written quotations are checked against source spans rather than accepted as evidence. Technical media validity is kept separate from creative quality review. Automatic regeneration has a bounded budget and hands uncertain outcomes to a reviewer. An interim removal of the local Episode cap was reversed in the active design: local video defaults to one Episode per project as a resource safeguard, while complete planning remains available and a bounded acceptance override is possible.

**Reached result and limits.** A retained real local *Lion and Mouse* run produced 21 valid Clips and a 42.9-second assembled Episode that played after a backend restart. The run remains `REVIEW_REQUIRED` for visual and directing quality. Controlled real-video superiority, time saved, and multi-Episode real acceptance have not been established. PDF story input, multi-user hosting, standalone keyframe authoring, style search, and advanced audio polish are outside the demonstrated scope. V4 is still under active development.

### WizAI Demo — Voice Book QA

**September 2026 · Single-PDF voice question answering · React, TypeScript, FastAPI, PostgreSQL, pgvector, Whisper, Ollama**

Voice Book QA accepts one text-based PDF, builds durable page-aware lexical and vector indexes, takes a spoken or typed question, returns an answer with server-validated citations, and can read the answer aloud. Retrieval combines PostgreSQL full-text search and vectors through reciprocal rank fusion, followed by deduplication, bounded context expansion, and evidence packing. Local voice and answer providers are available on macOS; OpenAI adapters are separately configurable.

**Problems and improvements.** PostgreSQL's conjunctive question parsing missed two cases in a frozen synthetic retrieval set. A bounded parser using submitted query terms raised fixture Recall@6 from 0.939 to 1.000. A four-anchor expansion displaced a gold result, so the final policy preserves six fused anchors before adding at most one context item. Stable source order removed UUID-dependent tie behavior; two fresh ingestions then produced identical fixture metrics. Later fixes improved microphone cancellation, API responsiveness during local transcription, and display of grounded generated answers.

**Scope and evidence.** The retained 36-case score—Recall@6 1.000 and MRR 0.851—comes from a generated PDF with deterministic offline embeddings, not a production-model or real-book quality claim. A newer real-document benchmark still requires approved cases. OCR, a multi-book library, query rewriting, reranking, and streaming speech were left out of this assessment build. Public deployment and production provider quality remain unverified.

### Local Lecture Copilot

**2026 · Local lecture workspace · Electron, Node.js, whisper.cpp, Ollama, retrieval**

A privacy-oriented desktop product for lecture recording or upload, preserved transcripts, conservative course-material correction, bilingual translation, notes, and structured outlines. The pipeline separates provisional transcription, user-controlled improvement, and derived documents. It persists sessions and revisions, bounds native Whisper and Ollama work, and distinguishes missing or stale outputs from accepted ones.

## Other Selected Work

- **Forgeboard:** a local content-operations application covering media understanding, planning, FFmpeg rendering, review, test publishing, metric import, and evidence-grounded insights. The verified publication adapter is synthetic; official platform publishing remains unverified.
- **EventNook Prospecting Agent:** an auditable UiPath workflow for company discovery, research, ICP qualification, contact checks, and structured JSON/Excel output. Retained unattended test runs and upload checks document the workflow; production deployment is separate.
- **Story Forge:** a separate interactive-reading production system with story planning, generation, QA, bounded batch queues, and portable finalized Story Library packages.
- **Local Outlook Group Mailer:** visible browser automation that reads an authorised NTULearn roster, verifies Outlook identities, and prepares a BCC draft. Ambiguous recipients stay out of the draft; the user sends it manually.
- **Agentic Rental Appointment Automation:** an NTU Applied AI workflow for property filtering, calendar availability, response interpretation, appointment creation, and lifecycle tracking.
- **ClassGuruAI Payment Service:** a TypeScript/Fastify subscription and credit-management microservice with authentication, SQLite WAL, health checks, and API documentation.
