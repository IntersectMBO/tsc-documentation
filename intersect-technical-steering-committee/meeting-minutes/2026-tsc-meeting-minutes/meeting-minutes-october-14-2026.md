# Meeting Minutes October 14, 2026

## Attendees:&#x20;

| Name               | Attendance | Role            | Voting Seat (Y/N) | Term         |
| ------------------ | ---------- | --------------- | ----------------- | ------------ |
| Kevin Hammond      | Yes        | Chair           | Y                 | October 2026 |
| Christian Taylor   | Yes        | Vice Chair      | Y                 | October 2026 |
| Tex McCutcheon     | Yes        | Secretary       | N                 | N/A          |
| Bosko Majdanac     | Yes        | Alt - Secretary | N                 | N/A          |
| Marcin Szamotulski | No         | Member/Seat     | Y                 | April 2028   |
| Alonzo Benavides   | Yes        | Member/Seat     | Y                 | April 2028   |
| Alexander Moser    | Yes        | Member/Seat     | Y                 | April 2028   |
| Ryan Wiley         | Yes        | Member/Seat     | Y                 | October 2026 |
| Udai Solanki       | No         | Member/Seat     | Y                 | October 2026 |
| Leandros Holleman  | Yes        | Member/Seat     | Y                 | October 2026 |

Community/Other Attendees

* Abid
* Nick Clarke<br>

**Recording:** [Technical Steering Committee - 2026/10/14 - Recording](https://drive.google.com/file/d/1tgf_rLx5IWB5i5wphBdzDSRXLlbckLJK/view?usp=sharing)

**Transcript:** [Technical Steering Committee - 2026/10/14 - Transcript](https://docs.google.com/document/d/1as4Qr6aeuprNJenrWvTjidS9moH1DagtteTbnVSAog8/edit?usp=sharing)

**Chat Transcript:** [Technical Steering Committee - 2026/10/14 - Chat Transcript](https://drive.google.com/file/d/18cYdNzZq0JmV0ZaKMUwQfNeZH6kkyfSv/view?usp=sharing)

## Agenda 14th October 2026

* Actions from the last meeting
* Dijkstra Hard Fork Updates
* TSC Budget To-Do’s
* Parameter Committee
* Post-quantum Crypto
* Node Diversity Workshop, London 12-13 November
* Baseline Readiness Report
* AOB

## Decisions/Actions

**Decisions**

* **Secretarial Role Shift:** Confirmed Tex as the primary TSC Secretary, with Bosko transitioning to an alternate Secretary role to focus on the Hard Fork Working Group.
* **Term Extensions:** Agreed to automatically extend committee terms expiring in October 2026 to April 2027, with Kevin explicitly confirming his term extension as Chair.
* **CIP Editors Funding & Appointments:** Ratified the decision to proceed with funding and appointing the two selected candidate candidates for the CIP Editor positions.
* **Work Package Leadership Appointments:** Provisionally appointed Christian as the lead for Work Package 1 (Events & Reports) and Leandros as the lead for Work Package 3 (Review).
* **Budget Vote Plan:** Decided to defer the formal vote on the proposed budget reallocation guidelines, audit rules, and capacity limits to an out-of-band Slack vote, to be finalized at the next meeting.
* **Post-Quantum Crypto Meeting Allocation:** Decided to allocate a dedicated 30-minute block at the beginning of the October 28 meeting for the post-quantum cryptography discussion.

**Actions**

* **Bosko:** Coordinate with Carlos regarding the shared Technical Risk Note updates (which were already posted to the Hard Fork Working Group channel last week).
* **Bosko:** Coordinate and host the dedicated CIP-23 call tomorrow afternoon (10/15) at 15:00 UTC (3:00 PM UTC).
* **All TSC Members:** Review the updated Dijkstra Risk Register (shared in chat/Slack) and the draft feature impact analyses prior to next week's meeting.
* **Bosko:** Review and update the initial feature impact analyses based on feedback and Claude/human gap reviews.
* **Kevin & Leandros:** Schedule an out-of-band meeting to set up and coordinate Work Package 3 (Review) framework and processes.
* **Christian:** Draft and post communications/announcements for the Node Diversity Workshop (Nov 12–13, Canary Wharf, London) once final event links are received.
* **Nick:** Share/provide the venue details link for the Node Diversity Workshop to Christian and Tex.
* **Nick:** Take ownership of following up on the status of transferring or forking the Emurgo serialization library repository to Intersect as a neutral host.

| Topic                               | Discussion                                                                                                                                                                                                                                                                                                                                                                                                           | Notes                                                                                                                           |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| Committee Roles & Administration    | Bosko announced a shift in TSC secretary duties, with Tex assuming the primary Secretary role and Bosko stepping into an alternate role to focus on the Hard Fork Working Group and Dijkstra. Members discussed term expirations occurring in October 2026; standard practice extends active terms to April 2027 automatically unless raised.                                                                        | Kevin agreed to extend his term; Christian was jokingly noted as next in line for Chair if terms expired.                       |
| Action Items & Budget               | The team confirmed technical risk note updates were posted in the Hard Fork Working Group channel. On the USDM conversion action item, the budget remains operational in ADA for now, with USDM options to be explored where conversion is required. Tracked actions regarding private guardrails with the Constitution Committee were confirmed as aligned across meetings.                                         | The risk notes review will be carried forward to the next meeting for detailed discussion.                                      |
| Dijkstra Hard Fork Updates          | Node version 11.2 (containing all features except Linear Leios) is expected this/next week, with DystraNet respawning on PV11 and hard forking to PV12. Node 11.3 is the candidate including Linear Leios, targeting PV12/12.0 capability subject to performance tests. Discussions touched on simplifying PV12 constitutional guardrails and a push by SPOs to pull CIP-23 up to PV12 with a possible 1-week delay. | A dedicated call on CIP-23 is scheduled for tomorrow at 15:00 UTC. Node diversity workshop confirmed for Nov 12–13 in London.   |
| Dijkstra Risk Register              | Kevin updated the risk register incorporating Leandros's items and adding new entries, bringing the total to \~40 tracked risks. The register includes severity and likelihood scoring that will require ongoing evaluation and owner assignments as the technical review progresses.                                                                                                                                | Members were asked to review the register via the shared Slack/chat link ahead of focused time next week.                       |
| Feature Impact Analysis             | Bosko and Ryan drafted impact analyses for PV12 features (including CIP-23 and CIP-50). Initial Claude-assisted reviews identified minor gaps for correction. Kevin summarized the Linear Leios engineering impact, noting hardware requirements (SSDs mandatory, memory-only insufficient) and realistic throughput expectations (\~5x on Nisashi net vs. theoretical 50x limits).                                  | DApps, DREPs, and exchanges must adjust workflows and hardware early due to changed buffering behavior under Linear Leios.      |
| Organization & Staff Changes        | ICAN staff have been uncoupled from IOT services as part of an ongoing decentralization process. Some staff have transferred organizations, which may affect connectivity or contact pathways for teams such as performance tracing and the Security Council.                                                                                                                                                        | Members should ensure updated contact paths are established via new organizational structures where needed.                     |
| TSC Budget & Smart Contracts        | Tex confirmed the Statement of Work was signed and the TSC smart contract is live on the Sundae dashboard. Milestone 0 requirements are being finalized to draw down upfront funding. Reallocation procedures within and between work packages were outlined (e.g., 10% intra-package flexibility without extra consultation).                                                                                       | Out-of-band Slack vote to be organized to formalize budget reallocations, audit remediation rules, and capacity limits.         |
| Work Package Allocation             | Christian was provisionally appointed as lead for Work Package 1 (Events & Reports), and Leandros for Work Package 3 (Review). Draft program description pages have been posted to ClickUp for team review and editing.                                                                                                                                                                                              | Kevin and Leandros scheduled an out-of-band discussion to set up WP3 processes.                                                 |
| Parameter Committee                 | The Parameter Committee will meet later in the week to continue reviewing Dystra guardrails (est. \~100 guardrails for PV12, \~50 for PV13/Peras) and evaluating the Plutus V4 cost model. The min pool cost proposal failed to pass the required threshold (\~45% out of 63% needed), shifting focus toward the min pool margin parameter via CIP-23.                                                               | Contact needs to be re-established with the Plutus team (now under Midgard Labs) regarding potential V4 parameter additions.    |
| Post-Quantum Crypto & Workshops     | Christian is coordinating with Paul and Fergie's team regarding post-quantum cryptography, with a meeting penciled in for October 28th. Details for the Node Diversity Workshop (Nov 12–13 at London Marriott Hotel Canary Wharf) were shared, with travel funding support available through the TSC budget.                                                                                                         | Christian to draft event communications once final detail links are provided by Nick.                                           |
| Baseline Readiness Report           | Nick presented the draft Baseline Readiness Report evaluating \~11 alternate nodes and their testing coverage. Key recommendations include establishing "Governance as a Service" to streamline complex proposal reviews/hard forks, as well as a cross-ecosystem consolidated security framework.                                                                                                                   | The report remains in draft for internal review prior to public release to address potential political or operational concerns. |
| Product Committee & Euler Hard Fork | The Product Committee will review the TSC Pull Request (covering vision and KPIs) next week at 13:30 UTC. A new outline discussion group is being kicked off to begin initial planning for the Euler hard fork to feed into 2027 work plans.                                                                                                                                                                         | Leandros and Kevin to attend the Product Committee review session if schedules permit.                                          |
| Repository Hosting                  | The committee revisited the status of the Emurgo serialization library repository, which was previously requested to be transferred to Intersect as a neutral host.                                                                                                                                                                                                                                                  | Nick accepted an action item to follow up on the status and resolution of the repository transfer.                              |
