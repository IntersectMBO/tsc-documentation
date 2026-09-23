# Meeting Minutes September 23, 2026

Sep 23, 2026 | Technical Steering Committee

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
| Alexander Moser    | Yes        | Member/Seat     | Y                 | April 2028   |
| Ryan Wiley         | Yes        | Member/Seat     | Y                 | October 2026 |
| Udai Solanki       | No         | Member/Seat     | Y                 | October 2026 |
| Leandros Holleman  | Yes        | Member/Seat     | Y                 | October 2026 |
| Seungheon Oh       | No         | Member/Seat     | Y                 | October 2026 |

Community/Other Attendees

* None

\
Recording: [Technical Steering Committee - 2026/09/23 - Recording](https://drive.google.com/file/d/1fpAQ9zkrVJgP7XNLR8X5ZoMzAK6gOs7O/view?usp=drive_link)

Transcript: [Technical Steering Committee - 2026/09/23 - Transcript](https://docs.google.com/document/d/1kZzzhG3A3UsXFoMwu76_iqyx7b_PiQCFqeNrj09dqzw/edit?usp=drive_link)

Chat Transcript: [Technical Steering Committee - 2026/09/23 - Chat Transcript](https://drive.google.com/file/d/1ZRol5mZFJf-X-ZD6YZlrMPR6byBSnJ7k/view?usp=drive_link)

## Agenda 23rd September 2026

* Actions from the last meeting
* Dijkstra era hard fork
* Technical Steering Committee Budget
* Parameter Committee
* Node diversity
* TSC review of CAPs
* Q3 Reporting/Q4 Planning
* AOB

## Decisions/Actions

**Decisions**

* **Budget & Milestone Structure:** Decided to retain the proposed 13-milestone structure across the three work packages rather than adding additional granular milestones.
* **CIP Editor Selection Role:** Agreed that the TSC will only ratify final candidate selections based on editor recommendations rather than conducting the initial recruitment screening.
* **Travel Funding Process:** Approved a continuously open application process with rapid turnaround times to accommodate urgent travel needs (e.g., London workshop).
* **Guardrail Scope Split:** Agreed to separate the \~50 guardrails required for Peras from the Dijkstra release to avoid delaying the current cycle.

**Actions**

* **Kevin:** Draft additional technical risk notes (gap analysis) for committee review and submit them to the general delivery risk register.
* **Kevin:** Set up a poll for prioritizing upcoming technical reports to commission.
* **Kevin:** Finalize details with Intersect regarding stablecoin conversion for the TSC budget.
* **Kevin:** Prepare Q3 achievements and Q4 goals reporting inputs.
* **Christian:** Coordinate a meeting time with the research team regarding the post-quantum risk assessment before the end of Q4.
* **Christian:** Assist Kevin with preparing Q3/Q4 reporting inputs for Intersect.
* **Terence:** Create and maintain ClickUp intake forms for CIP editor applicants, travel funding requests, and expert funding applications.
* **Kevin/Terence:** Finalize and publish the travel funding call and application form ahead of the London Node Diversity workshop.
* **Kevin/Bosko:** Define formal review criteria alongside Kevin for allocating expert funding for the Parameter Committee and Hard Fork Working Group.
* **TSC Members:** Review the technical risk register draft provided by Kevin.
* **TSC Members:** Cast votes in the Intersect Board Elections before voting closes in two days.<br>

| Topic                                      | Discussion                                                                                                                                                                                                                                           | Notes                                                                                                                             |
| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Meeting Logistics & Quorum                 | Kevin called the meeting to order at 4 minutes past the hour. Quorum was reached with 8 voting members present.                                                                                                                                      | Meeting was recorded.                                                                                                             |
| Review of Past Actions                     | Bosko reviewed open action items. Progress was noted on the State of the Union draft, post-quantum risk assessments, parameter feedback, and node developer contacts.                                                                                | Post-quantum research team is open to meeting, likely before end of Q4.                                                           |
| Node Updates & Releases (Dijkstra / Peras) | Ryan briefed on Node 11.1.2 release, upcoming 11.1.3 storage patch, and Node 11.2 plans. Discussions covered BLS key support for hardware wallets, neutral naming conventions, and progress on alternative nodes (Haskell, Dingo, Amaru, Yarloomoo). | A node diversity workshop in London is targeted for Nov 12–13.                                                                    |
| Technical Risk Register & Recovery         | Kevin highlighted the transition of technical risks into Intersect's delivery register and noted gaps in identifying all risks, specifically around disaster recovery mechanics and parameter hysteresis under linear layoffs.                       | Kevin will draft additional risk notes for committee review.                                                                      |
| Hardware Wallet Coordination               | Cardano Foundation is taking over hardware wallet coordination from IO to ensure compatibility post-hard fork for new transaction forms (BLS keys, Plutus v4).                                                                                       | Non-blocker for hard fork, but a priority to address.                                                                             |
| TSC Budget & Milestones                    | Kevin drafted integrated Statements of Work with 3 milestones per work package (13 total milestones across the budget). Terence suggested more granular milestones to mitigate reputation risks with large upfront withdrawals.                      | Committee agreed to stick to the 13-milestone structure framed around time/reports.                                               |
| CIP Editors Recruitment                    | Robert provided his CV for one editor position. Recruitment for additional editors was posted on Discord, with follow-ups scheduled for Twitter and the Intersect newsletter.                                                                        | Terence will set up a ClickUp form for applicant tracking; TSC will ratify final candidates.                                      |
| Travel Funding & Workshop Support          | Open application process for travel funding will be established to allow quick turnaround, specifically targeting attendees for the London node diversity workshop in November.                                                                      | Kevin, Bosko, and Terence to finalize minimal-friction application process.                                                       |
| Parameter Committee & Hard Fork Funding    | Funding is available to support additional experts and commission technical/performance reports for the Parameter Committee and Hard Fork Working Group.                                                                                             | Process and criteria will be shared in upcoming meetings.                                                                         |
| Governance Action on Parameter K           | An individual community member prematurely submitted an info governance action on Parameter K, using a 51% threshold where non-votes count as 'No'. Discussed implications for the Parameter Committee's approach.                                   | Parameter Committee will meet Thursday to decide whether to submit a formal competing proposal or focus on educational materials. |
| Node Cost & Memory Submissions             | Ryan's memory cost resubmission currently has \~11.8% SPO support with 18 days remaining. Transaction memory increases will not be resubmitted as-is.                                                                                                | Any future larger parameter increases will require a new Parameter Change Proposal (PCP).                                         |
| Dijkstra Guardrails Review                 | Kevin identified 100–150 new guardrails needed for Dijkstra (mainly linear layoffs and reference scripts). Neil and Bosko raised concerns regarding workload, resource constraints, parameter interactions, and missing vendor performance data.     | Kevin will share analysis after initial Parameter Committee review; node performance data is needed before finalizing settings.   |
| Intersect Reporting & Board Elections      | Q3 achievements and Q4 goals need to be submitted for the upcoming Intersect meeting. Board election voting closes in two days.                                                                                                                      | Members are urged to vote in the Intersect board elections.                                                                       |
