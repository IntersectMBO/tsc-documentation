# Meeting Minutes October 07, 2026

Oct 7, 2026 | Technical Steering Committee

## Attendees:&#x20;

| Name               | Attendance | Role            | Voting Seat (Y/N) | Term         |
| ------------------ | ---------- | --------------- | ----------------- | ------------ |
| Kevin Hammond      | Yes        | Chair           | Y                 | October 2026 |
| Christian Taylor   | Yes        | Vice Chair      | Y                 | October 2026 |
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

* Abid
* Duncan Soutar
* Enrique Fernandez
* Luke Mahoney
* Nick Clarke

\
Recording: [Technical Steering Committee - 2026/10/07 - Recording](https://drive.google.com/file/d/1Jub8wo2faMrfSmbwe3kkJu7Crcxk9ir6/view?usp=drive_link)

Transcript: [Technical Steering Committee - 2026/10/07 - Transcript](https://docs.google.com/document/d/1uMlNoBrWkyY9inDHiYCgp4nY4bDOrQSHnUU7lweiHPY/edit?usp=drive_link)

Chat Transcript: [Technical Steering Committee - 2026/10/07 - Chat Transcript](https://drive.google.com/file/d/1O4yEMAxPhebiBnc8WDNKlufX2IhxUw0s/view?usp=drive_link)

## Agenda 7th October 2026

* Actions from the last meeting
* Dijkstra era hard fork
* Parameter Committee
* Technical Steering Committee Budget
* Post-Quantum Cryptography
* TSC Members Terms
* AOB

## Decisions/Actions

**Decisions**

* **Administrative Lead Assignment:** Administrative, payment, and onboarding communications with Intersect Delivery Assurance will be managed directly by Bosko, Terence, and Kevin on behalf of the TSC.
* **Interim Work Package Leads:** Kevin (Chair) and Christian (Vice Chair) will serve as default Work Package Leads until formal leads are officially designated.
* **Milestone Approval Process:** Terence will prepare the Milestone Acceptance Forms (MAFs), which will then be signed off by Kevin prior to submission to Intersect.
* **Extension of TSC Member Terms:** The TSC will extend current member terms until April 2027 without holding elections (pending individual confirmations).

**Actions**

* **Bosko:** Post technical risk notes/updates in the Hard Fork Working Group Slack channel and ensure they are officially documented in the central Dijkstra risk log.
* **Bosko:** Conduct private/direct outreach to each TSC member to confirm their willingness to extend their term through April 2027.
* **Tex/Kevin/Bosko:** Coordinate in regards to the USDM conversion feedback provided by James.
* **Kevin:** Facilitate a review of the full Dijkstra Risk Register with the TSC during the next meeting.
* **Ken-Erik:** Organize a working/Q\&A session on parameter guardrails and technical dependencies for Constitutional Committee (CC) members, involving IOG engineers.

\
<br>

| Topic                                   | Discussion                                                                                                                                                                                                                               | Notes                                                                                                                                                                              |
| --------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Welcome & Agenda Reordering             | Kevin called the Technical Steering Committee (TSC) meeting to order and proposed prioritizing Duncan's update to optimize his remaining time at Intersect.                                                                              | Quorum was initially not met (4 voting members present; Alex was absent in Singapore). Quorum was reached later when Christian and Alonzo joined.                                  |
| Intersect Handover & Onboarding         | Duncan announced this is his last month in Delivery Assurance at Intersect and introduced Luke and Enrique, who will assume his responsibilities starting November 1st.                                                                  | Onboarding/administrative tasks will be handled by Bosko, Terence, and Kevin rather than taking up general TSC meeting time.                                                       |
| Smart Contract & Milestone Submissions  | Intersect raised the TSC's smart contract online (\~15 mins prior). Approval will take 36+ hours, with expectations of going live by the end of the week to release first milestone funding.                                             | Submissions require a completed Milestone Acceptance Form (MAF) linking acceptance criteria to public evidence. Terence will prepare MAFs, and Kevin will sign off.                |
| Work Package Leads                      | Duncan inquired about designated work package leads referenced in the Statement of Work (SOW).                                                                                                                                           | Work package leads have not yet been formally agreed upon. Kevin and Christian will serve as default leads in the interim.                                                         |
| Review of Action Items                  | Bosko reviewed previous action items: Leandros's technical risk notes for layers were completed and shared with Carlos; Marcin's draft branch push was delayed due to time constraints; Parameter Committee guardrail notes were shared. | Technical risk log items from IOG have been incorporated into the main Dijkstra risk log. Bosko will post the updates in the Hard Fork Working Group channel.                      |
| Scoping Next Era Hard Fork              | Bosko and Kevin discussed coordinating scoping for the upcoming hard fork era (Euler/Ouroboros Leios).                                                                                                                                   | Progress was delayed with Sam in Singapore. The Node Diversity Workshop in London will serve as the next key opportunity to progress scoping.                                      |
| Node Release Uptake (11.1.3 & 11.2)     | Node 11.1.3 has around 30–40% adoption among Stake Pool Operators (SPOs). SPOs need to upgrade to avoid potential ledger bug connectivity issues and improve block distribution.                                                         | Node 11.2 is 1–2 weeks away from pre-release. Node 11.3 development will begin around mid-October.                                                                                 |
| Hard Fork Timeline & Integration Risks  | Neil expressed strong concern over integration delays, noting that missing code integrations and necessary PR merges make a 2026 hard fork timeline highly unrealistic.                                                                  | Kevin acknowledged the unpredictability of integration timelines (ranging from 1 to 4 months), stating a Node v12 candidate would be needed very soon to achieve a 2026 hard fork. |
| Dijkstra Risk Register                  | The committee discussed treating the risk register as a primary driver, prioritizing technical risk resolution over arbitrary delivery deadlines.                                                                                        | Bosko shared the risk register link with the group. The TSC will review the register in detail during next week's meeting.                                                         |
| Dijkstra Guardrails Review              | Kevin analyzed protocol v12 parameters, identifying \~100 new guardrails (45 checkable by scripts, 38 related to reference scripts, 9 for pledge, and 48 for Leios).                                                                     | Carlos proposed a constitutional amendment with 83 guardrails, showing strong overlap with Kevin's independent analysis.                                                           |
| Constitutional Amendment & Benchmarking | Ken-Erik noted December as a target for constitutional discussions with Constitutional Committee (CC) members. Neil emphasized that parameter settings cannot be finalized without a fully integrated node running benchmarks.           | Kevin proposed that if a hard fork occurs before constitutional changes are ready, Leios could initially be deployed in a disabled parameter state.                                |
| Plutus V4 & Parameter Committee         | Kevin noted the Parameter Committee will need to review Plutus V4 settings.                                                                                                                                                              | Decision on new primitives requiring benchmarking is expected from the Plutus team later in October.                                                                               |
| TSC Budget & Operational Updates        | Kevin referenced feedback from James regarding converting funds to USDM, to be coordinated with Terence and Bosko.                                                                                                                       | Applications for CIP Editor positions close this week, with 9 applications received so far.                                                                                        |
| TSC Member Terms & Farewell             | Bosko noted plans to extend current TSC member terms through April 2027 without holding new elections.                                                                                                                                   | The committee bade farewell to Neil, thanking him for his extensive contributions to the TSC and the Cardano ecosystem.                                                            |
