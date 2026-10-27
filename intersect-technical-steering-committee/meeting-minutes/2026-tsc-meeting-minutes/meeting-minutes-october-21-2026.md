# Meeting Minutes October 21, 2026

## Attendees:&#x20;

| Name               | Attendance | Role            | Voting Seat (Y/N) | Term         |
| ------------------ | ---------- | --------------- | ----------------- | ------------ |
| Kevin Hammond      | Yes        | Chair           | Y                 | October 2026 |
| Christian Taylor   | No         | Vice Chair      | Y                 | October 2026 |
| Tex McCutcheon     | Yes        | Secretary       | N                 | N/A          |
| Bosko Majdanac     | Yes        | Alt - Secretary | N                 | N/A          |
| Marcin Szamotulski | Yes        | Member/Seat     | Y                 | April 2028   |
| Alonzo Benavides   | Yes        | Member/Seat     | Y                 | April 2028   |
| Alexander Moser    | Yes        | Member/Seat     | Y                 | April 2028   |
| Ryan Wiley         | No         | Member/Seat     | Y                 | October 2026 |
| Udai Solanki       | No         | Member/Seat     | Y                 | October 2026 |
| Leandros Holleman  | No         | Member/Seat     | Y                 | October 2026 |

Community/Other Attendees

* Agustin Mista
* Aleksandr Vershilov
* Jesus Diaz Vico
* Kristijan Kowalsky
* Nicolas Bacquey
* Sandro Coretti-Drayton
* Thomas Bagrel



**Recording:** [Technical Steering Committee - 2026/10/21 - Recording](https://drive.google.com/file/d/1uQWhkMlJvqMfEfYzhSXtgajdMfk1Wdhy/view?usp=sharing)

**Transcript:** [Technical Steering Committee - 2026/10/21 - Transcript](https://docs.google.com/document/d/1huWuYz_YYjR5J4brzGHdrxZ84YcTZdyq9r0gij14qoM/edit?usp=sharing)

**Chat Transcript:** [Technical Steering Committee - 2026/10/21 - Chat Transcript](https://docs.google.com/document/d/1huWuYz_YYjR5J4brzGHdrxZ84YcTZdyq9r0gij14qoM/edit?usp=sharing)

## Agenda 21st October 2026

* Cryptography Schemes for Peras - Tweag/IOR
* Actions from the last meeting
* Djikstra Hard Fork Status
* TSC Budget
* Feedback on TSC PR on KPI’s
* Dijkstra Rollout - Constitutional update & guardrails
* Proposed changes to Intersect scope
* AOB

## Decisions/Actions

**Decisions**

* **Provisional Standing of All Votes:** Any formal determinations reached during the meeting are classified as provisional and require ratification out of band due to lacking a voting quorum.
* **Batch Voting and Abstention Policy:** Committee members must cast out-of-band votes on the six outstanding issues by tomorrow afternoon; any uncast votes will formally be counted as abstentions.
* **Milestone Zero Baseline Documentation:** The committee agreed to adopt previously approved lists for upcoming events and report topics (removing outdated items) to fulfill Milestone 0 criteria rather than running a new formal voting cycle.
* **Peras Cryptography Next Steps:** Rather than deciding on a cryptographic scheme immediately, the committee agreed to review Aleksandr’s background material and invite the team back for a 15-minute follow-up session at the next meeting.

**Actions**

* **Kevin** and **Bosko** to collect names of interested attendees and coordinate with Damian before the end of next week to finalize accommodation and catering numbers.
* **Terence** to coordinate with Damian to obtain links and publish the workshop announcements.
* **Bosko** and **Kevin** to contact Ziyang directly to confirm whether any parameter changes, cost model updates, or new primitives are required for Plutus V4.
* **Kevin** to submit detailed technical feedback to Carlos addressing structural inconsistencies in the proposed constitutional amendment.
* **Kevin** to coordinate with the Parameter Committee regarding guardrail range limits and initial parameter settings for Min Margin and Min Pool Cost.
* **Terence** to contact the identified lead to determine maintenance and ownership of the Cardano Serialization Library while Nick is away.
* **TSC Voting Members** to submit out-of-band votes on the six pending committee issues prior to the deadline tomorrow afternoon.
* **Terence** to gather and record Conflict of Interest (COI) disclosures for onboarded CIP editors.
* **Terence** to compile and publish the rosters for the Parameter Committee and the Hard Fork Working Group, along with approved events and report topics, to the GitBook.
* **Alexander** to identify and assist Parameter Committee members who require financial/travel support and report back at the next meeting.
* **Kevin** to identify Hard Fork Working Group members who need support.

| Topic                                             | Discussion                                                                                                                                                                                                                                                                                                                                                                                           | Notes                                                                                                                                                    |
| ------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Meeting Opening & Quorum Status                   | Kevin welcomed attendees and guest Aleksandr. Quorum was not met due to Leandros's absence, meaning all decisions made during the call remain provisional until ratified out of band.                                                                                                                                                                                                                | Formal votes and official decisions must be confirmed via out-of-band ratification.                                                                      |
| Cryptography Schemes for Peras (Problem Overview) | Aleksandr presented the trade-offs around cryptography schemes for Peras, focusing on historical certificates, catching-up/syncing nodes, and vulnerability to stake shift across epochs. Jesus clarified that stake shift measures stake moving from honest to dishonest participants (estimated at \~10% over 19 epochs).                                                                          | Aleksandr shared a background document with Terence and offered to share it with the broader team.                                                       |
| Attack Vectors on Syncing Nodes                   | Thomas explained how an adversary could exploit historical stake shifts to corrupt previously honest nodes for a low budget and forge past certificates. Sandro noted that while the implementation rollback limits confine the immediate issue to syncing nodes, it technically results in active nodes sitting on an objectively non-preferable chain.                                             | Genesis synchronization and chain selection mechanics remain key security concerns.                                                                      |
| Evaluation of Pixel vs. BLS Schemes               | Aleksandr outlined the Pixel key-evolution scheme, which offers fast rotation (e.g., every 36 hours) and aggregation, but lacks mature, production-grade implementations. An alternative is using BLS with an increased safety threshold, though this could negatively affect liveliness and force fallback to Praos. Alexander and Alonzo expressed hesitation over adopting unproven cryptography. | Consensus leaned toward pragmatically using BLS with an increased safety threshold for the near term while continuing to test Pixel for future releases. |
| Threshold Adjustments & Fallback Protocol         | Nicolas clarified that raising the voting threshold (e.g., from 75% to 85%) absorbs up to 10% of stake shift without actively detecting it. If a quorum is missed due to adversarial absence, the protocol safely drops into Praos cooldown mode until the stake redistributes, trading liveliness for security without risking permanent damage.                                                    | A temporary fallback to Praos is considered acceptable operational behavior during major stake shifts.                                                   |
| Research on Quantum Resistance                    | Kevin noted that future protocol updates must keep quantum resistance on the radar, highlighting an upcoming session where an external partner will present on the topic and the committee will commission a dedicated study.                                                                                                                                                                        | A dedicated report on quantum resistance is scheduled to be presented in two weeks.                                                                      |
| Review of Outstanding Action Items                | Terence led a rapid review of previous action items: Bosko completed the CIP-23 call coordination; Kevin updated the feature impact analysis; and work package 3 reviews were completed in a private session.                                                                                                                                                                                        | Outstanding items include finalizing the risk register owners and distributing Node Diversity Workshop materials.                                        |
| Node Diversity Workshop (London)                  | Terence and Kevin addressed announcements for the upcoming Node Diversity Workshop at the Canary Wharf Marriott in London. Bosko shared available links in the chat, noting that while venue attendance is open, complimentary accommodation spots are strictly limited.                                                                                                                             | Attendees must submit their interest to Kevin or Bosko by the end of next week so catering and logistics can be finalized with Damian.                   |
| Plutus V4 & Node Releases Update                  | Bosko reported that version 11.2 (entering the Conway to Dijkstra transition) is expected this week, with 11.3 arriving several weeks later. Kevin confirmed there is currently no formal update on Plutus V4 parameter changes or cost models from Midgard Labs.                                                                                                                                    | Bosko and Kevin will follow up directly with Ziyang to obtain expected Plutus V4 specifications.                                                         |
| CIP-23 (Min Margin) Inclusion in Dijkstra         | Bosko shared that the dev team agreed to include CIP-23 in the full Dijkstra release. Alexander strongly objected to adding features at the last minute outside standard governance processes. Kevin explained that the decision addresses urgent SPO community concerns without altering release schedules or imposing extra costs.                                                                 | Min Margin will roll out initially set to zero, with guardrails and ranges to be deliberated by the Parameter Committee.                                 |
| Constitutional Amendment & Guardrails Feedback    | Bosko announced an upcoming open session with Carlos covering guardrail structures. Kevin raised concerns regarding inconsistencies between Carlos's proposed amendment and the existing constitution, specifically warning against efforts to omit necessary guardrails.                                                                                                                            | Kevin will submit technical feedback to Carlos and review parameter settings with the Parameter Committee.                                               |
| TSC Budget & Milestone Zero Requirements          | Terence outlined the deliverables required to unblock Milestone 0 funding, including agreed event lists for Q4/Q1, report delivery topics for Q1/Q2, committee rosters (Parameter Committee, Hard Fork Working Group), and Conflict of Interest (COI) disclosures for onboarded CIP editors.                                                                                                         | Kevin advised utilizing previously agreed lists to satisfy requirements without waiting for formal re-votes.                                             |
| Outstanding Committee Voting                      | Kevin urged all members to cast out-of-band votes on the six issues brought forward during the prior week's call. Voting will formally close tomorrow afternoon, with missing submissions recorded as abstentions.                                                                                                                                                                                   | Members must submit out-of-band votes before the deadline tomorrow afternoon.                                                                            |
