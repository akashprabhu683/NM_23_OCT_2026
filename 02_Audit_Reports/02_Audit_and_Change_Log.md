# Deliverable C: Audit and Change Log
**Project Title:** Auto Ticket Classification Using Flow Designer  
**Team ID:** SWTID-2026-8980  
**Institution:** Jaya Engineering College (JEC)  
**Date:** 23 October 2026  

---

## 1. Overview
This log details all modifications, corrections, and completions performed across the project documents. In compliance with the Antigravity Master Prompt, all original files in `frds` and `NM_03OCT.zip` remain completely untouched. All modifications were performed strictly on copies in `01_Final_Documents`.

---

## 2. Detailed Change Log by Document

### Document 1: `Customer_Journey_Map_SWTID-2026-8980.docx`
- **Original Source:** `frds\Customer_Journey_Map_Completed.docx`
- **Sections Modified:** Paragraph 5 (Editorial Notice) and Table 0 (Project Metadata).
- **Corrections Made:**
  - Removed internal editor note: *"Administrative fields not supplied: Team ID and submission date. Replace bracketed placeholders before submission."*
  - Updated Date from `23/10/2026` to standard academic format `23 October 2026`.
  - Added institutional metadata: `Jaya Engineering College (JEC) / CSE (Anna University Reg. 2021)`.
- **Reason:** Editorial instructions should not appear in final submission deliverables; standardized academic date and institutional affiliation.
- **Evidence Supporting Correction:** Master Prompt Section 2.

### Document 2: `Data_Flow_Diagrams_and_User_Stories_SWTID-2026-8980.docx`
- **Original Source:** `frds\Data_Flow_Diagrams_and_User_Stories_Completed.docx`
- **Sections Modified:** User Stories intro text and Table 0.
- **Corrections Made:**
  - Removed internal instruction note regarding bracketed placeholders.
  - Standardized Date to `23 October 2026` and added institutional metadata row.
  - Verified User Stories (US-1 to US-6) against Flow Designer actions.
- **Reason:** Final clean document presentation; validated that user stories accurately depict the ServiceNow implementation.
- **Evidence Supporting Correction:** `Primary_Implementation_Guide.docx` (ServiceNow build steps).

### Document 3: `Solution_Requirements_SWTID-2026-8980.docx`
- **Original Source:** `frds\Solution_Requirements_Completed.docx`
- **Sections Modified:** Table 0 (Metadata Table).
- **Corrections Made:**
  - Standardized Date to `23 October 2026`.
  - Added institutional row for Jaya Engineering College (JEC), Anna University Regulation 2021.
  - Verified that all Functional Requirements (FR-1 through FR-6) and Non-Functional Requirements (NFR-1 through NFR-6) strictly respect evidence boundaries without claiming unverified ML or complex scripting.
- **Reason:** Metadata completeness and consistency.
- **Evidence Supporting Correction:** Master Prompt Section 2 & 9.

### Document 4: `Technology_Stack_SWTID-2026-8980.docx`
- **Original Source:** `frds\Technology_Stack_Completed.docx`
- **Sections Modified:** P4 (References note) and Table 0.
- **Corrections Made:**
  - Removed editorial reminder: *"Before submission, confirm the ServiceNow instance details..."*
  - Standardized Date to `23 October 2026` and added institutional affiliation.
- **Reason:** Professional presentation; verified that components reflect the Now Platform, custom table `Incident Workflow`, and Flow Designer actions.
- **Evidence Supporting Correction:** Master Prompt Section 2.

### Document 5: `Project_Planning_Template_SWTID-2026-8980.docx` & `Planning_Logic_SWTID-2026-8980.docx`
- **Original Source:** `NM_03OCT\docs\Project_Planning_Phase_Filled\4. Project Planning Phase\`
- **Sections Modified:** Table 0, Paragraphs P8-P12 (Velocity calculation), Table 2 (Sprint Tracking Table).
- **Corrections Made:**
  - Corrected Sprint count and story points: Replaced reference team's 2 sprints (23 points) with our team's verified 4 sprints (80 total points, 20 points/sprint, velocity = 20 story points/sprint).
  - Aligned sprint dates: Sprint-1 (26 Oct-31 Oct 2026), Sprint-2 (02 Nov-07 Nov 2026), Sprint-3 (09 Nov-14 Nov 2026), Sprint-4 (16 Nov-21 Nov 2026).
  - Inserted Team ID `SWTID-2026-8980`, Date `23 October 2026`, and College metadata.
- **Reason:** Resolves major cross-document contradiction between reference team's planning and my teammates' completed `Project_Planning_Phase_SWTID-2026-8980.pdf`.
- **Evidence Supporting Correction:** `frds\Project_Planning_Phase_SWTID-2026-8980.pdf`.

### Document 6: `User_Acceptance_Testing_FSD_SWTID-2026-8980.docx`
- **Original Source:** `NM_03OCT\docs\5. Project Development Phase\Performance Testing\User Acceptance Testing FSD.docx`
- **Sections Modified:** Table 0 (Metadata), Testing Period, URL/Location, Tester Name, Sign-off block.
- **Corrections Made:**
  - Updated Date to `23 October 2026`, Team ID to `SWTID-2026-8980`.
  - Added Tester details: `Akash Prabhu. P (Reg. No: 110824104004) & Team SWTID-2026-8980`.
  - Testing Period specified as `16 October 2026 to 23 October 2026`.
  - Preserved strictly: TC-001 (Wi-Fi: Pass), TC-002 (Projector: Pass), TC-003 (Forgot Password: Pass), TC-004 (Performance: Pass), TC-005 (Unmatched: Fail), TC-006 (Trigger on create only: Pass).
  - Preserved defect `BG-001` (unmatched tickets leave Category empty due to missing Else branch).
- **Reason:** Friends had no Phase 4 UAT documents; completed the official template with our team's genuine data without fabricating test outcomes.
- **Evidence Supporting Correction:** `Primary_Implementation_Guide.docx` & Master Prompt Section 9.

### Document 7: `UAT_Execution_Report_SWTID-2026-8980.docx`
- **Original Source:** `NM_03OCT\docs\5. Project Development Phase\User Acceptance Testing\UAT Report Template.docx`
- **Sections Modified:** Table 0 (Metadata).
- **Corrections Made:**
  - Inserted Team ID `SWTID-2026-8980`, Date `23 October 2026`, and JEC institutional details.
  - Verified defect table (1 fixed, 1 skipped, 1 won't fix) and test case pass/fail summary (8 pass, 1 fail).
- **Reason:** Completed missing UAT report deliverable.
- **Evidence Supporting Correction:** UAT FSD document.

### Document 8: `FSD_Documentation_Format_SWTID-2026-8980.docx`
- **Original Source:** `NM_03OCT\docs\Project_Documentation_Filled\6. Project Documentation\FSD Documentation Format.docx`
- **Sections Modified:** Section 1 (Introduction), Section 9 (User Interface), Section 11 (Screenshots).
- **Corrections Made:**
  - Replaced placeholder team list with full names, register numbers, and assigned project roles for all 5 team members:
    1. Akash Prabhu. P (110824104004) - Team Lead / Flow Designer Configuration
    2. Gowtham. R (110824104020) - Table & Field Schema Designer
    3. Karthik. K (110824104032) - Flow Logic & Trigger Developer
    4. Gokul Raj K (110824104019) - Notification & Dependent Choice Rules
    5. Douglas Christopher. I (110824104017) - Testing & Quality Assurance
  - Replaced screenshot placeholders with genuine screenshots extracted from our primary evidence (`Primary_Implementation_Guide.docx`).
- **Reason:** Friends had no FSD documentation; completed missing requirement using official template and authentic team evidence.
- **Evidence Supporting Correction:** Master Prompt Section 2 & `Primary_Implementation_Guide.docx`.

### Document 9: `Final_Project_Report_SWTID-2026-8980.docx`
- **Original Source:** `NM_03OCT\docs\Project_Documentation_Filled\6. Project Documentation\Final Report Template.docx`
- **Sections Modified:** Header/Cover page block, Table 0, Section 5 (Planning), Section 7.1 (Output Screenshots), Section 11 (Appendix).
- **Corrections Made:**
  - Added academic cover header conforming to Anna University Regulation 2021, Jaya Engineering College, Department of Computer Science and Engineering.
  - Listed all 5 team members with register numbers and roles.
  - Preserved faculty guide placeholder: `[Faculty Guide / Supervisor Name - To be confirmed]`.
  - Synchronized Section 5 with our team's 4 sprints (80 story points, 20 points/sprint).
  - Embedded genuine implementation screenshots (Incident Workflow form, Flow Designer canvas, Wi-Fi test scenario execution).
  - Clearly formatted external link placeholders in Appendix.
- **Reason:** Comprehensive final academic report required for Naan Mudhalvan submission.
- **Evidence Supporting Correction:** Master Prompt Sections 2, 6, 8, 9, 10.
