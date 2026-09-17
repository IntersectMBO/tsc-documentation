# Meeting Minutes September 16, 2026

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
* James Meidinger
* Elena Bardo

\
Recording: [Technical Steering Committee - 2026/09/16 - Recording](https://drive.google.com/file/d/1zsZJQYiojYfbL-pmG3KFFQYXkYiU1UoW/view?usp=drive_link)

Transcript: [Technical Steering Committee - 2026/09/16 - Transcript](https://docs.google.com/document/d/1T5QTYBa6sqhleGadq_TJW8T5i7Wu0KJ7zkTnRoOwC_w/edit?usp=drive_link)

Chat Transcript: [Technical Steering Committee - 2026/09/16 - Chat Transcript](https://drive.google.com/file/d/1Z1NfpV8mF8IVRqydGc2xj7YALR4A-8BD/view?usp=drive_link)

## Agenda 16th September 2026

* Actions from the last meeting
* Dingo Node has Minted Mainnet Block
* Dijkstra era hard fork
* Technical Steering Committee Budget
* Parameter Committee
* TSC review of CAPs
* Q3 Reporting/Q4 Planning
* AOB

## Decisions/Actions

**Decisions**

* **Testnet Parameter Reversion:** Voted by majority (5 in favor, 0 opposed, 0 abstentions) to revert the Plutus memory limit parameters on testnets back in line with mainnet limits.
* **CIP Editor Recruitment Process:** Agreed to proceed with publishing the recruitment notice for CIP editors once minor text adjustments regarding TSC oversight are applied.

**Actions**

* **Nick:** Share the draft of the Cardano "State of the Union" report with Kevin and Christian.
* Neil: Send feedback regarding K=1000 to Ryan by the end of the week.
* **Alex:** Consolidate parameter feedback once Neil and Ryan submit their inputs; adjust the wording of the CIP editor recruitment notice.
* **Christian:** Forward Kevin's notes on post-quantum crypto risk assessments to the IO Research team.
* **Kevin:** Feed back concerns regarding the operational burden of fixed committee size parameters to the node developers.
* **Elena:** Work with Mike to test potential contract breakage on Sanchonet/Preview prior to reverting testnet memory limits.
* **Bosko:** Schedule an off-line meeting with Kevin, Christian, Terence, James and Intersects delivery assurance to resolve the smart contract asset allocation issue.

<br>

| Topic                                       | Discussion                                                                                                                                                                                                                                                                                                           | Notes                                                                                                                                    |
| ------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| State of the Union Report                   | Nick raised that Intersect is assembling a "State of the Union" technical report for Cardano and requested input. Kevin suggested keeping comments private rather than discussing them in public, asking members to submit feedback directly to Nick or Kevin.                                                       | Nick to share the draft with Kevin and Christian.                                                                                        |
| Dependency Tracker & 2030 Vision            | Kevin updated the committee that he extracted dependencies into a spreadsheet for Jeff to assist with planning. Leandros confirmed opening a PR for the 2030 Vision KPIs recommendations without altering core recommendations.                                                                                      | Bosco to turn the dependency tracker into a Miro chart.                                                                                  |
| Parameter Committee / K=1000                | Neil and Ryan discussed feedback regarding parameter updates (K=1000). Neil noted that Alec is synthesizing input. Ryan mentioned he will be away starting a week from tomorrow, making early input essential.                                                                                                       | Neil to send responses to Ryan by the end of the week. Alec's consolidated document action remains carried forward.                      |
| Post-Quantum Crypto Report                  | Christian reported progress on the post-quantum crypto report outline, having reached out to Fergie. Kevin noted an IO Research two-page document on consensus and ledger requirements, emphasizing the need for a proper risk assessment regarding keys and voting.                                                 | Christian to forward Kevin's notes to the IO Research team.                                                                              |
| Intersect Governance Working Group          | Terence highlighted that the Intersect Governance Working Group meets Thursdays at 2:00 PM to review committees, election processes, and related governance tasks. He encouraged interested members to join.                                                                                                         | Committee members to monitor the working group's progress.                                                                               |
| Dingo Node Mainnet Milestone                | Kevin announced that the Dingo node minted its first block on mainnet. Nick detailed their live conformance testing, which validates UTXO sets, protocol parameters, and Plutus model vectors against a standard node.                                                                                               | The team noted a need to engage Dingo developers via the Hard Fork Working Group and Security Council.                                   |
| Node 11.1 / 11.2 & Committee Size Parameter | Ryan noted Node 11.1 mainnet release and 11.2 progress for Dystra testing. Neil raised concerns over changing the committee size from a percentage to a fixed number, arguing it converts an automated closed-loop system into an open-loop operational management burden that requires parameter updates to adjust. | Kevin to capture these operational concerns and feed them directly back to the node vendor team.                                         |
| Dijkstra Hard Fork & Naming Proposal        | Bosko confirmed the Hard Fork Working Group proposed naming the hard fork after Alex Esgen, alongside an In Memoriam section for other community members.                                                                                                                                                            | The proposal requires further communication planning to navigate the social/governance aspects effectively.                              |
| Plutus Memory Limits (Testnet Reversion)    | Elena questioned whether testnets (Preview/Preprod) should revert their Plutus memory limits to match mainnet, avoiding disparities for contract developers. Following a vote, the decision was carried by majority (5 in favor, 0 opposed, 0 abstentions) to revert the settings.                                   | Elena to coordinate with Mike to test script behavior on Sanctionet/Preview before full reversion.                                       |
| CIP Editors Funding & Recruitment           | Kevin presented Robert's recruitment proposal and CV for expanding CIP editors. Alec cautioned against the TSC overstepping by appearing to select or whitelist CIP editors, while Neil and Kevin clarified that the TSC's role is strictly fiduciary oversight regarding who gets remunerated from community funds. | Members to submit text tweaks by the end of the day; Alec to adjust the advert text to clarify the CIP team is recruiting independently. |
| TSC Budget & Smart Contract Asset Types     | Terence noted Intersect's current constraint restricting smart contracts to a single asset type (ADA vs. USD), preventing the planned split allocation without separate contracts.                                                                                                                                   | A dedicated meeting will be scheduled with Kevin, Bosko, Christian, Terence, and James to resolve the administrative setup.              |
| Q3 Reporting & Q4 Planning                  | Kevin noted that Q3/Q4 administrative planning needs to be structured similarly to the previous quarter.                                                                                                                                                                                                             | Kevin and Bosko to structure the existing data for reporting.                                                                            |
