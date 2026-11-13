# VOAP Mission Control

Design-first prototype for the **ValOS Operational Adoption Programme** (VOAP), based on the latest proposal supplied in November 2026.

## Open the prototype

Open `index.html` directly in a browser. No build step, backend, credentials or Netcup deployment is required. The prototype includes an overview, organisation adoption pipeline, separate task Kanban, milestone tracker, outreach & communications panel, evidence register layout, funding tracker, and decision/risk register.

**Important:** This is a prototype, not a production application. Tasks and organisations entered in the browser use `localStorage`. They are not synchronized or backed up. Do not put confidential applications, correspondence, security findings, or personal information into a publicly hosted copy.

## Proposal baseline

- Programme duration: **18 months** (actual start date TBD).
- Funding requested: **USD 108,000** (not an award).
- Target: **12 independently verifiable adoptions**.
- Headline target mix: **6 staking operators + 6 security/assurance providers**.
- Activation: **20 qualified prospects**.
- Activity milestones: **10 operator-specific actions, 10 provider-specific actions, 6 staking proposals, 6 provider proposals**.
- Seven milestone payments: 12k + 21k + 21k + 13.5k + 13.5k + 13.5k + 13.5k = **USD 108k**.
- **Open discrepancy:** The paid adoption milestone breakdown includes **9 staking operators and 3 providers**, in contrast with the 6+6 programme commitment. Resolve this before implementing acceptance logic.

### Verification principle

Pipeline advancement **does not** count as verified adoption. The current prototype's verified counters remain at zero because it has no independent-review or evidence approval workflow. In production, only independently accepted records with the required operational adoption and continuity evidence should increase verified KPIs.

## Important scope distinctions

VOAP drives and coordinates adoption; it **does not** perform security audits, certify operators, operate third-party validators, build partners' security products, perform routine ValOS v2 maintenance, or administer the existing Lido subsidy. Link to the independent subsidy intake without conflating its recipients with verified VOAP adoptions.

## Connected destinations (links only, no API integration)

- [ValOS](https://www.valos.global/)
- [ValOS standard](https://github.com/lidofinance/valos)
- [ValOS on X](https://x.com/validatorOS/)
- [Operator subsidy Tally](https://tally.so/r/jebL0Y)

## Future production architecture

Suggested: React/Next.js or lightweight SPA, PostgreSQL, authenticated server API, role-based access (programme admins, partners, independent reviewers, read-only observers), private evidence object storage, tamper-evident activity log, backup plan and a separately publishable, redacted public adoption register.

Core entities: Organisation, Opportunity, AdoptionAction, Proposal, AssessmentReferral, AdoptionEvidence, IndependentReview, ContinuityPlan, Milestone, Task, Activity, Communication, FundingEntry, Decision, Risk. Include owner, date, status, next action, relevant grant deliverable and audit history where appropriate.

Do not place API tokens or sensitive evidence in a public GitHub repository. Explicit review before any public publication.

## Suggested next phases

1. Approve programme KPI definitions, acceptance criteria and resolve the 6+6 / 9+3 mismatch.
2. Implement multi-user persistence, permissions, organisation/adoption records, evidence review and a public-safe register.
3. Add milestone/reviewer workflow, evidence exports, reporting and budget.
4. Evaluate permitted Tally and X data access and integrations; deploy separately to Netcup when ready.
