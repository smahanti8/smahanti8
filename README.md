# Subha Mahanti

**I build the product and engineering organizations that take AI across the trust bar where errors cost bodies, not dashboards — surgical robotics through FDA, enterprise AI at scale, agentic systems shipped in the open.**

Twenty years, one problem at increasing stakes: making powerful systems trustworthy enough to act on the physical world. Twelve years in real-time distributed systems (MathWorks) — the substrate agent orchestration now runs on. Multi-team embedded engineering on a Class III robotic-surgery platform through design transfer and FDA/CE authorization (Medtronic Hugo™ — IEC 62304, ISO 13485/14971), where I built the SOUP governance function from scratch: automation and intelligence replacing manual vulnerability review of COTS, OTS, and open-source components — and owned it end to end, including weekly sessions with General Counsel on EULA compliance, reselling terms, and IP review. Engineering risk and legal-regulatory risk, held in one seat. Then concept-to-commercialization leadership of new AI/analytics service offerings on a $175M IoT SaaS portfolio (Fortive) — new monetization models built on customer analytics and master data management, $1M incremental revenue in year one. Now: a 200+ person global product and engineering org at Schneider Electric, and the vision and macro-architecture for a production GenAI platform spanning ideation to engineering to post-release support.

Along the way I kept volunteering across the walls: cadaver studies with clinical-trial and human-factors engineers, market research and user surveys for long-horizon roadmaps, partnerships with marketing and business development. Engineering, clinical, commercial, and regulatory — I've worked inside all four, which is the only way I know to build systems that survive contact with all four.

I come from a family of surgeons, and I've seen up close what it costs when the right information isn't at the point of care. This work is personal.

## What's here

Every repo ships with a `DECISIONS.md` — because architecture judgment is the job — and reports its own failures, because a pipeline that claims 100% is either being fed clean data or lying to you.

🏥 **[surgical-fhir-pipeline](../surgical-fhir-pipeline)** — *shipped.* Maps synthetic robotic-surgery telemetry to FHIR R4B behind a conformant REST API, and refuses to hide what the crossing destroys: 80% of cases exchangeable, every lossy mapping logged, terminology bindings marked `PROVISIONAL` with a test that fails if anyone promotes them without doing the work. Interoperability as a governance problem, treated like one.

⚖️ **[prior-auth-agent](../prior-auth-agent)** — *building in the open.* An agent that drafts prior-authorization determinations under two hard rules: no citation → no claim (every criterion links to the exact policy passage *and* the exact patient-record element), and it is never allowed to deny — approvals can be automated; denials get humans. LangGraph state machine, hash-chained audit log, golden-set evals in CI, cost-per-determination published. Follow the commits; the `Known Limitations` section is load-bearing.

🛡️ **regulated-ai-evals** — *next.* The trust layer extracted and generalized: requirement→prompt→test traceability, versioned golden sets, regression gates, auto-generated audit packets. What IEC 62304 taught me, expressed in pytest.

**Stack:** Python · Anthropic API (Sonnet/Haiku tiered) · LangGraph · ChromaDB · MCP · FastAPI · Synthea/FHIR R4B · GitHub Actions. Synthetic data only, always.

## The standing invitation

If you're evaluating whether the AI depth is real: don't ask me — open the eval harness, the binding-status tests, the audit trail, and go as deep as you like. The stack took me months. The part that took twenty years is knowing what must never ship.

📍 Boston · [LinkedIn](https://linkedin.com/in/smahanti) · Building toward: product & engineering leadership in regulated AI · Open to: founder conversations, technical diligence, advisory
