# Meeting Minutes September 09, 2026

## Attendees:&#x20;

| Name               | Attendance | Role            | Voting Seat (Y/N) | Term         |
| ------------------ | ---------- | --------------- | ----------------- | ------------ |
| Kevin Hammond      | Yes        | Chair           | Y                 | October 2026 |
| Christian Taylor   | Yes        | Vice Chair      | Y                 | October 2026 |
| Bosko Majdanac     | Yes        | Secretary       | N                 | N/A          |
| Tex McCutcheon     | Yes        | Alt - Secretary | N                 | N/A          |
| Marcin Szamotulski | Yes        | Member/Seat     | Y                 | April 2028   |
| Alonzo Benavides   | No         | Member/Seat     | Y                 | April 2028   |
| Neil Davies        | Yes        | Member/Seat     | Y                 | April 2028   |
| Alexander Moser    | Yes        | Member/Seat     | Y                 | April 2028   |
| Ryan Wiley         | Yes        | Member/Seat     | Y                 | October 2026 |
| Udai Solanki       | No         | Member/Seat     | Y                 | October 2026 |
| Leandros Holleman  | Yes        | Member/Seat     | Y                 | October 2026 |
| Seungheon Oh       | No         | Member/Seat     | Y                 | October 2026 |

Community/Other Attendees

* Nick Clarke
* Ken-Erik Ølmheim

\
Recording: [Technical Steering Committee - 2026/09/09 - Recording](https://drive.google.com/file/d/1-KIh7gueWaoX5203kKYL7tLcDetCVWxC/view?usp=drive_link)

Transcript: [Technical Steering Committee - 2026/09/09 - Transcript](https://docs.google.com/document/d/1MAxm-Zj3KkzoXB7ni0YNEEijegkQNn3EKHWKt54vVb8/edit?usp=drive_link)

Chat Transcript: [Technical Steering Committee - 2026/09/09 - Chat Transcript](https://drive.google.com/file/d/1T-9RVizUUL5_5qgn7PLbjvJqu8tvRIAv/view?usp=drive_link)

## Agenda 2nd September 2026

* Actions from the last meeting
* Dijkstra era hard fork
* Technical Steering Committee Budget
* Parameter Committee
* TSC review of CAPs
* Post Quantum Cryptography
* Q3 Reporting/Q4 Planning
* AOB

## Decisions/Actions

**Decisions**

* **Parameter Proposals:** The TSC decided not to re-submit the rejected Plutus memory limit or minimum fee parameter change proposals on its own initiative, respecting the community vote outcome.
* **Hard Fork Naming:** Agreed to proceed with an Info Action to name the hard fork after Alexander Esgen following family consent.
* **CAP Reviews:** Referred CAPs regarding SPO approval for economic parameters and net change limits to the Parameters Committee for evaluation.
* **Funding Approval Process:** Adopted the use of a public ClickUp form (managed by Terence) to process travel and event support requests, setting a limit of $2,000 per funded event.
* **K1000 Strategy:** Agreed to proceed with a two-step approach for K1000: first issuing a stake-weighted SPO Info Action, followed by a formal DRep parameter vote if approved.

**Actions**

* **Bosko:** Connect Leandros, Lorenzo, and himself in a group chat to finalize the PR for the 2030 Vision KPIs.
* **Kevin:** Continue refining the dependency tracker spreadsheet with Jeff and capture feedback from the Hard Fork Working Group.
* **Kevin:** Circulate the updated HackMD document containing the complete set of Dijkstra parameters once received from Carlos.
* **Neil:** Finalize responses to Alex's comments regarding the K1000 rationale document.
* **Alex:** Finalize the consolidated K1000 rationale document and circulate it within the Parameters Committee for review.
* **Christian:** Formulate a plan for a post-quantum cryptography report coordinating with IOG research.
* **All TSC Members:** Complete the 10-minute Intersect questionnaire linked in ClickUp/Slack.

<br>

| Topic                                        | Discussion                                                                                                                              | Notes                                                                                                                        |
| -------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Quorum Clarification                         | The committee discussed quorum calculations regarding the 9 elected members versus the 10-person establishment count.                   | Clarification needed on whether majority is calculated against elected members (9) or establishment (10).                    |
| Agenda Review                                | Checking for additional agenda items; Bosko raised a point from Lorenzo regarding PR2 KPIs.                                             | Intersect's Lorenzo requested a PR for KPI updates; Bosko to connect Leandros, Lorenzo, and himself.                         |
| Action Items Review                          | Review of pending actions from the prior meeting, including the Centralized Technical Risk Register and CIP research updates.           | Technical Risk Register exists at IOG but is private due to security concerns; excerpts will be required.                    |
| Parameter Changes (Min Cost & Plutus Memory) | Discussion on the rejected parameter changes (min cost & Plutus memory limits) due to low SPO voting turnout.                           | Committee agreed not to re-submit the rejected changes directly; community members can submit new proposals if desired.      |
| Dijkstra Hard Fork Scope                     | Status update on Node versions (11.1 mainnet ready, 11.2 in progress) and target scope for Protocol Versions 12 and 13.                 | Dolos and Palace are on the critical path. Cardano RPC and Serve are deferred to 2027.                                       |
| Dependency Tracker & Gates                   | Kevin introduced a detailed dependency chart/spreadsheet capturing 27 essential community and release gates.                            | IoG plan listed 9 gates; Kevin's version includes broader ecosystem dependencies (e.g., hardware wallets, security reviews). |
| Hard Fork Naming                             | Update on naming the upcoming hard fork info action.                                                                                    | Family approval was received to name the hard fork after Alexander Esgen.                                                    |
| TSC Budget & Support Calls                   | Update on drafting policies, SOWs, and lightweight mechanisms for funding community support requests.                                   | Terence created a ClickUp form for travel funding requests; funding per event capped at $2,000.                              |
| K1000 Parameter Proposal                     | Alex, Neil, and Ryan discussed the strategy to gauge SPO support for increasing K to 1000 using an Info Action.                         | SPO vote will be stake-weighted. If SPOs approve, a formal parameter change will be submitted for DRep voting.               |
| Constitutional Actions (CAPs)                | Review of two Constitutional Actions (CAPs) submitted by Thomas regarding SPO economic parameter approval and net change limits.        | Both CAPs referred to the Parameters Committee for formal review and operational feedback.                                   |
| Post-Quantum Cryptography                    | Christian and Kevin provided an update on post-quantum crypto research and potential impacts on keys, wallets, and on-chain signatures. | Changing on-chain keys would require a hard fork; seed phrases would remain unaffected. Independent assessment requested.    |
| Intersect Survey                             | Bosko and Kevin reminded members to complete the Intersect questionnaire.                                                               | Link distributed; members requested to fill out the \~10-minute form.                                                        |
