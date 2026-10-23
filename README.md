# Auto Ticket Classification Using Flow Designer
**Team ID:** `SWTID-2026-8980`  
**Institution:** Jaya Engineering College (JEC)  
**Affiliation:** Anna University, Chennai (Regulation 2021)  
**Department:** Computer Science and Engineering (CSE), Third Year  
**Submission Date:** 23 October 2026  
**Repository:** [github.com/akashprabhu683/NM_23_OCT_2026](https://github.com/akashprabhu683/NM_23_OCT_2026)

---

## 📌 Executive Summary

This repository houses the complete academic and technical documentation, verification audit reports, design artifacts, and implementation evidence for the project **"Auto Ticket Classification Using Flow Designer"** developed under **Anna University Regulation 2021**.

The system automates ticket categorization and subcategorization on the **ServiceNow Now Platform** using **Flow Designer**, eliminating manual triage delays, routing incidents instantly, and delivering immediate confirmation notifications to requesters.

---

## 👥 Project Team Roster

| S.No | Student Name | Register Number | Role |
|:---:|:---|:---:|:---|
| 1 | **Akash Prabhu. P** | 110824104004 | **Team Lead / ServiceNow Developer** |
| 2 | **Gowtham. R** | 110824104020 | Developer / Technical Documentation |
| 3 | **Karthik. K** | 110824104032 | QA Engineer / Test Execution Lead |
| 4 | **Gokul Raj K** | 110824104019 | Systems Analyst / Requirements Engineer |
| 5 | **Douglas Christopher** | 110824104017 | Scrum Master / Project Planning |

---

## ⚙️ Solution Architecture & Implementation Highlights

- **Platform:** ServiceNow Now Platform (Washington DC / Zurich Release)
- **Primary Data Schema:** Custom table `Incident Workflow` (`u_incident_workflow`) with 9 key fields:
  - `Number` (Auto-generated prefix `INCWF`)
  - `Caller` (Reference to `sys_user`)
  - `Category` & `Subcategory` (Choice fields)
  - `Short Description` & `Description` (String / Text)
  - `State`, `Assigned Group`, and `Assigned to`
- **Automation Logic:** No-code ServiceNow Flow Designer
  - **Trigger:** Record Created on `u_incident_workflow` where `Category is Empty`
  - **Decision Rules:** Keyword parsing matching Short Description / Description:
    - *Wi-Fi / Network* $\rightarrow$ Category: **Network**, Subcategory: **Wi-Fi**
    - *Projector / Hardware* $\rightarrow$ Category: **Hardware**, Subcategory: **Projector**
    - *Forgot Password / Login / Password* $\rightarrow$ Category: **Access**, Subcategory: **Forgot Password**
    - *Slow Computer / Performance / Slow* $\rightarrow$ Category: **Performance**, Subcategory: **Slow computer**
  - **Automated Communication:** Send Email notification to `Caller -> Email` on successful creation.
- **Sprint & Agile Planning:** 4 Sprints across 24 working days, 80 total Story Points, 20 Story Points/sprint velocity (20 User Stories: `USN-1` through `USN-20`).
- **Test Integrity:** 6 UAT test scenarios (`TC-001` through `TC-006`). Unmatched keywords (`TC-005`) are documented honestly as known backlog defect `BG-001` (slated for `USN-9`), demonstrating genuine engineering rigour.

---

## 📂 Repository Structure

```plaintext
NM_Final_Documentation_SWTID-2026-8980/
├── 01_Final_Documents/                         # Official Deliverables (DOCX, PDF, PPTX)
│   ├── Phase_1_Ideation/                       # Brainstorming, Problem Statements & Empathy Maps
│   │   ├── Brainstorm_Idea_Prioritization_SWTID-2026-8980.docx
│   │   ├── Completed_Brainstorm_Idea_Prioritization_SWTID-2026-8980.pdf
│   │   ├── Completed_Define_Problem_Statements_SWTID-2026-8980.pdf
│   │   ├── Completed_Empathy_Map_Canvas_SWTID-2026-8980.pdf
│   │   ├── Define_Problem_Statements_SWTID-2026-8980.docx
│   │   └── Empathy_Map_Canvas_SWTID-2026-8980.docx
│   ├── Phase_2_Design/                         # Architecture, Requirements, DFDs & Pitch Decks
│   │   ├── Customer_Journey_Map_SWTID-2026-8980.docx
│   │   ├── Data_Flow_Diagrams_and_User_Stories_SWTID-2026-8980.docx
│   │   ├── Problem_Solution_Fit_Canvas_SWTID-2026-8980.pptx
│   │   ├── Problem_Solution_Fit_Template_SWTID-2026-8980.pptx
│   │   ├── Proposed_Solution_Template_SWTID-2026-8980.pptx
│   │   ├── Solution_Architecture_SWTID-2026-8980.pdf
│   │   ├── Solution_Requirements_SWTID-2026-8980.docx
│   │   └── Technology_Stack_SWTID-2026-8980.docx
│   ├── Phase_3_Planning/                       # Agile Sprints, User Stories & Story Points
│   │   ├── Planning_Logic_SWTID-2026-8980.docx
│   │   ├── Project_Planning_Phase_SWTID-2026-8980.pdf
│   │   └── Project_Planning_Template_SWTID-2026-8980.docx
│   ├── Phase_4_Development_and_Testing/        # UAT Test Cases, Traceability & Bug Log
│   │   ├── UAT_Execution_Report_SWTID-2026-8980.docx
│   │   └── User_Acceptance_Testing_FSD_SWTID-2026-8980.docx
│   └── Phase_5_Documentation/                  # Final Project Report & FSD Specification
│       ├── Final_Project_Report_SWTID-2026-8980.docx
│       └── FSD_Documentation_Format_SWTID-2026-8980.docx
├── 02_Audit_Reports/                           # Verification & Quality Assurance Reports
│   ├── 01_Document_Inventory.md
│   ├── 02_Audit_and_Change_Log.md
│   ├── 03_Cross_Document_Consistency_Report.md
│   ├── 04_Clarification_Checklist.md
│   ├── 05_Final_Quality_Control_Report.md
│   └── 06_Final_Submission_Verification_Report.md
├── 03_Evidence_and_References/                 # Verified Primary Implementation Evidence
│   ├── Primary_Implementation_Guide.docx       # Guide with 42 verified configuration screenshots
│   ├── Team_Implementation_Screenshots/        # Extracted individual implementation proof images
│   └── Reference_Screenshots_NM_03OCT/         # Upstream baseline reference screenshots
├── 04_Items_Requiring_Clarification/           # Evaluator & Guide sign-off checklist
│   └── Clarification_Checklist.md
└── README.md                                   # Project Overview & Index
```

---

## 🧪 Acceptance Testing Summary

| Test ID | Test Scenario | Description Keyword | Expected Result | Actual Result | Status |
|:---:|:---|:---|:---|:---|:---:|
| **TC-001** | Network classification | "Wi-Fi connection down in lab" | Category: `Network`, Subcategory: `Wi-Fi` | Category & Subcategory updated; email sent | **PASS** |
| **TC-002** | Hardware classification | "Projector display flickering" | Category: `Hardware`, Subcategory: `Projector` | Category & Subcategory updated; email sent | **PASS** |
| **TC-003** | Access issue classification | "Forgot password to portal" | Category: `Access`, Subcategory: `Forgot Password` | Category & Subcategory updated; email sent | **PASS** |
| **TC-004** | Performance issue | "Slow computer after restart" | Category: `Performance`, Subcategory: `Slow computer` | Category & Subcategory updated; email sent | **PASS** |
| **TC-005** | Unmatched keyword triage | "AC in server room leaking water" | Category: `General / Other` (Default) | Category remains blank (No `Else` branch) | **DEFECT (BG-001)** |
| **TC-006** | Update trigger restriction | Record updated (Category modified) | Flow should not trigger on update | Flow only triggered on `Record Created` | **PASS** |

---

## 🔗 Project Links

- **GitHub Repository:** [akashprabhu683/NM_23_OCT_2026](https://github.com/akashprabhu683/NM_23_OCT_2026)
- **Video Demonstration Drive Link:** [Google Drive Folder](https://drive.google.com/drive/folders/1NYfD8kHX6Su9VBgkYKpSaBVTYnT1S_Db?usp=drive_link)

---

## 🎓 Academic Compliance & Attribution

Prepared in accordance with the curriculum requirements of **Anna University, Chennai (Regulation 2021)** for the Department of **Computer Science and Engineering**, **Jaya Engineering College (JEC)**. All screenshots, configurations, and verification audits represent genuine implementation evidence.
