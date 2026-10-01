# Meeting Minutes October 01, 2026

## Attendees:&#x20;

| Name               | Attendance | Role            | Voting Seat (Y/N) | Term         |
| ------------------ | ---------- | --------------- | ----------------- | ------------ |
| Kevin Hammond      | Yes        | Chair           | Y                 | October 2026 |
| Christian Taylor   | No         | Vice Chair      | Y                 | October 2026 |
| Bosko Majdanac     | Yes        | Secretary       | N                 | N/A          |
| Tex McCutcheon     | Yes        | Alt - Secretary | N                 | N/A          |
| Marcin Szamotulski | Yes        | Member/Seat     | Y                 | April 2028   |
| Alonzo Benavides   | Yes        | Member/Seat     | Y                 | April 2028   |
| Neil Davies        | Yes        | Member/Seat     | Y                 | April 2028   |
| Alexander Moser    | No         | Member/Seat     | Y                 | April 2028   |
| Ryan Wiley         | No         | Member/Seat     | Y                 | October 2026 |
| Udai Solanki       | No         | Member/Seat     | Y                 | October 2026 |
| Leandros Holleman  | Yes        | Member/Seat     | Y                 | October 2026 |
| Seungheon Oh       | No         | Member/Seat     | Y                 | October 2026 |

Community/Other Attendees

* James Meidinger

\
Recording: [Technical Steering Committee - 2026/09/30 16:00 CEST - Recording](https://drive.google.com/file/d/1mubPDI7HS14VXFaRL2kAhKpU6p323bLH/view?usp=drive_link)

Transcript: [Technical Steering Committee - 2026/09/30 16:00 CEST - Transcript](https://docs.google.com/document/d/1hcqUH-Y5EVYluPnln1FrEVnJ8A1mW93dLMxkppr9Joo/edit?usp=drive_link)

Chat Transcript: [Technical Steering Committee - 2026/09/30 - Chat Transcript](https://drive.google.com/file/d/1QQD6_nnP3bz6LRGtZO8WJAvuntYHyWV7/view?usp=drive_link)

## Agenda 23rd September 2026

* Actions from the last meeting
* Dijkstra era hard fork
* Planning for euler era hard fork
* CIP on managing different node versions
* Parameter Committee
* Technical Steering Committee Budget
* TSC review of CAPs
* TSC Members Terms
* Q3 Reporting/Q4 Planning
* AOB

## Decisions/Actions

**Decisions**

* **Quorum Adjustment:** Approved excluding Ryan from the quorum calculation threshold during his multi-month absence.
* **Budget Contract Currency Structure:** Approved drafting the primary Statement of Work in ADA while executing stablecoin conversions upon drawing down tranches as needed for fiat commitments.
* **Technical Work Priorities:** Approved the priority sequence for technical work reports: (1) Post-Quantum Cryptography, (2) Impact of Node Implementations, and (3) Security Readiness.
* **Plutus Memory Unit Limits:** Decided against pursuing minor (9%) incremental increases to Plutus transaction memory unit limits, requiring a formal PCP and benchmark analysis prior to any major adjustment.
* **Protocol Guardrails Scope:** Decided to limit current guardrail revisions strictly to Protocol Version 12 parameters, delaying Protocol Version 13 guardrail drafting.

**Actions**

* **Leandros's Risk Notes:**
  * TSC members to review and submit feedback on Leandros's technical risk notes within 48 hours.
  * Leandros to re-share the document link in the Slack channel for team visibility.
* **Risk Register Integration:** Bosko to transition current hard fork risk logs into a dedicated Dystra technical risk register, assign risk owners, and share with the TSC once complete.
* **CIP Draft:** Marcin to push his draft branch and share the link to the Node-to-Node Versioning CIP with the committee next week.
* **Contract Execution:** Tex to track final signatures from Jack and Mark on the Statement of Work and Master Services Agreement.
* **Guardrails Review:** Committee members to review Kevin’s draft guardrail updates for Protocol Version 12 by the end of the week.
* **Euler Scoping Coordination:** Kevin to coordinate with the Product Committee regarding technical input for Euler release scoping (potentially forming a joint working group).



| Topic                                   | Discussion                                                                                                                                                                                                                                                                          | Notes                                                                                                                                                               |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Agenda & Quorum Adjustments             | Kevin opened the meeting and set the agenda. The committee addressed Ryan's extended multi-month absence and agreed by consensus to temporarily exclude him from quorum calculations without removing him as a TSC member.                                                          | Ryan removed from quorum count during his absence. Bosko noted he had to drop off early.                                                                            |
| Resignation Announcement                | Neil announced his resignation from both the TSC and the Parameters Committee, effective after next week's meeting. He cited frustration with community engagement, vendor practices, and a lack of proper review/control mechanisms within Intersect.                              | Neil's final TSC meeting will be next week. Committee members expressed regret over his departure.                                                                  |
| Action Items & Technical Risk Register  | The committee reviewed open action items. Leandros drafted a technical risk analysis regarding potential vendor layoffs and the Dystra release. Neil highlighted big red flags (high risk, likelihood, and impact) in the report.                                                   | Members have 48 hours to provide feedback on Leandros's risk analysis before it is shared more broadly.                                                             |
| TSC Budget & Stablecoin Conversions     | Kevin and Tex finalized the Statement of Work (SOW). James and Tex discussed conversion mechanics between ADA and stablecoins (USDM). To prevent delays, the main contract is written in ADA, with conversions to stablecoins occurring at tranche drawdowns when fiat is required. | Statement of Work and Master Services Agreement (MSA) sent out for signatures (signed by Tex; awaiting Jack and Mark).                                              |
| Dijkstra Hard Fork & Node Releases      | Node 11.1.3 was released to address a ledger rule bug that affected networking/peer connectivity (big ledger peers). Node 11.2 is 2–3 weeks from pre-release. Node 11.3 will integrate linear Leios features over approximately 5 major PRs.                                        | Node 11.1.3 is the recommended version for mainnet. Delivery of linear Leios is potentially pushed to March–April 2027 (seems mathematically impossible for Dec 5). |
| Node-to-Node Versioning SIP             | Marcin discussed a forthcoming CIP aimed at establishing a communication protocol for node-to-node versions across multiple implementations, allowing feature tracking without necessarily changing wire-level encodings.                                                           | Marcin will share the draft CIP link with the committee next week.                                                                                                  |
| CIP Editor Positions                    | Openings for CIP Editors have been advertised on Discord and Twitter, with newsletter inclusion prioritized. The committee discussed establishing a baseline "sanity check" criteria for candidates to prevent Sybil/collusion risks.                                               | Robert Phair will retain his current position. Payment processes to be set up upon SOW execution.                                                                   |
| Technical Work Reports Prioritization   | Kevin outlined priority order for upcoming technical reports: (1) Post-quantum cryptography requirements for Cardano, (2) Impact of old/diverse node implementations on-chain, and (3) Security readiness.                                                                          | Commissioning process to proceed using unlocked smart contract funds.                                                                                               |
| Parameters Committee & On-Chain Polling | The committee discussed an unauthorized on-chain poll regarding K=1000 (K parameter). The premature poll damaged the opportunity for a structured community/DRep dialogue. Kevin and Ryan published a "case for and against" to inform voters.                                      | Ryan submitted an on-chain proposal to reduce minPoolCost to 75.                                                                                                    |
| Plutus Execution Units & V4 Cost Model  | Discussions around increasing Plutus transaction memory unit limits concluded that minor increments are unnecessary; larger increases require a sponsored Parameter Change Proposal (PCP) and benchmarking. Protocol v12 will introduce Plutus V4, requiring updated cost models.   | A formal PCP is required before memory limit increases are considered. Benchmarking must evaluate impact on linear Leios.                                           |
| Guardrails & Governance Updates         | Kevin prepared draft guardrail updates and additions for protocol v12 parameters. Protocol v13 guardrails are deferred for now.                                                                                                                                                     | Committee members to review draft guardrails by the end of the week before public release.                                                                          |
| TSC Governance & Term Extensions        | Terms for TSC members elected in October 2026 have been extended to April 2027, aligning with the next planned election cycle.                                                                                                                                                      | Alex is tracking CAP reviews on his task list.                                                                                                                      |
