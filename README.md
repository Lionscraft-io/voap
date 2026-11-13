# VOAP — Workforce-style Adoption Board

A design-first VOAP dashboard adapted from the **warm, quiet, paper-planner Kanban UI** in the private [Lionscraft-io/workforce](https://github.com/Lionscraft-io/workforce) repository.

## Visual language
- Cream canvas and sidebar, dark olive text and green primary actions.
- Open, horizontally scrollable Kanban lanes with coloured status dots and rounded white cards.
- Small tinted labels, owner initials, dates, sidebar navigation and slide-out card editing.
- Drag cards between columns on desktop; tap to edit status on mobile.

## Five sections
1. **Overview:** adoption KPI targets, workstream snapshots, quick links.
2. **Adoption pipeline:** Identified → Contacted → Engaged → Implementing → Verification pending. Filter by staking or security/assurance.
3. **Task Kanban:** Backlog → Weekly → Focus → Review → Done. Workstream filters.
4. **Adoption milestones:** only four operational adoption outcomes (staking 3 / 6 / 9 and assurance providers 3).
5. **Outreach & comms:** manually managed contacts plus links to [ValOS X](https://x.com/validatorOS/) and [NOP subsidy intake](https://tally.so/r/jebL0Y).

No funding KPI, funding/budget module, evidence register, or decisions/risk module. No outreach activity milestones.

## How to run
Download or clone this repo and open `index.html` in a browser. It is a self-contained, static prototype with no build step. GitHub's source code view does **not** render the application.

Changes are stored in browser `localStorage` using the key `voap_workforce_design_v1`, not in GitHub or on a server. They are not synchronised with other users or devices. Do not enter private operator security findings or sensitive contact/applicant data into a publicly hosted copy.

**KPI counting:** The prototype intentionally displays zero independently verified adoptions. Merely moving an organisation to "Verification pending" does not count it as verified. The eventual production version needs a validated confirmation workflow.

**Proposal discrepancy:** The updated grant proposal states an overall 6 staking + 6 assurance commitment, whereas the four adoption milestones total 9 staking + 3 assurance. For visualisation the dashboard uses the milestone-specific 9+3 breakdown without purporting to change the commitment.

## What was reused vs adapted
This is a **visual and interaction adaptation**, not a copy of Workforce's infrastructure. It does not reuse Workforce's backend, authentication, Markdown task storage, agents or API. The final Netcup deployment and any real persistence are separate future work.


## ValOS branding assets

- `assets/valos-logo.svg` — original full ValOS vector logo (orange symbol and black wordmark), supplied by the project.
- `assets/valos-icon.svg` — cropped SVG symbol for sidebar, page header and favicon, preserving the supplied vector path and original orange `#FC5F2B`.

The VOAP interface uses ValOS branding while retaining the warm paper-planner Kanban design. Assets are referenced via relative paths for static hosting.
