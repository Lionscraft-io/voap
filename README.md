# VOAP Adoption Dashboard

Interactive design prototype for the ValOS Operational Adoption Programme, based on the latest proposal.

## Scope

Exactly five sections:
1. **Overview:** adoption progress, four operational adoption milestones, quick access to other workspaces, and pipeline / Kanban snapshots.
2. **Adoption Pipeline:** track staking operators and security/assurance providers through Identified → Engaged → Integrating → Evidence ready.
3. **Task Kanban:** To do → In progress → Blocked → Done, including starter tasks and user-created tasks.
4. **Adoption Milestones:** track **only** four operational adoption milestones from the proposal:
   - First 3 Ethereum staking operators (at least 1 with 20,000+ ETH staked).
   - Second group of 3 (6 cumulative; composition requirements apply).
   - Third group of 3 (9 cumulative; composition requirements apply).
   - First 3 security and assurance providers (at least 2 integration application areas).
5. **Outreach & Comms:** campaign and stakeholder tracking concept, with direct links to [ValOS X](https://x.com/validatorOS/) and the [validator/NOP subsidy application](https://tally.so/r/jebL0Y).

There is intentionally **no** funding KPI, budget tracker, evidence-register page, decisions/risk page, or activity-based grant milestones.

## Adoption counting

The proposal's broad 12-organisation commitment specifies 6 staking + 6 assurance, while the adoption milestones specify 9 staking + 3 assurance. The prototype displays the milestone path **9+3** explicitly, with a note about this inconsistency. Do not silently interpret the proposal as changing its commitment.

The preview does not count a pipeline card as independently verified, even when moved to 'Evidence ready'. Adoption figures remain at 0 until a proper independent-review confirmation workflow is implemented.

## How to view

Open `index.html` in a browser, or access its GitHub Pages URL **after** Pages is separately configured. Browsing the GitHub source file itself will show code, not an interactive dashboard.

The prototype stores added tasks and organisation pipeline entries in local browser storage; nothing syncs to GitHub or a server. Never put confidential applicant data or validator security details into a publicly deployed prototype.

Future production work: authenticated multi-user persistence, organisation records with owner/next action, independently confirmed adoption criteria, outreach campaign management, task assignments, and a backend for safe hosting on Netcup. No deployment has been performed.
