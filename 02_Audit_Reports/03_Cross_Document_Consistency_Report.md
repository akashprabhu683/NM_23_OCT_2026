# Deliverable D: Cross-Document Consistency Report
**Project Title:** Auto Ticket Classification Using Flow Designer  
**Team ID:** SWTID-2026-8980  
**Institution:** Jaya Engineering College (JEC) | Anna University Regulation 2021  
**Audit Date:** 23 October 2026  

---

## 1. Audit Scope & Consistency Matrix

| Parameter / Data Item | Expected Value / Baseline | Consistency Status Across Final Documents | Discrepancies Found in Source Material & Resolution |
|:---|:---|:---:|:---|
| **Project Title** | Auto Ticket Classification Using Flow Designer | **CONSISTENT** | Unified capitalization across all headers and templates. |
| **Team ID** | SWTID-2026-8980 | **CONSISTENT** | Replaced `[Enter Team ID]` placeholders from reference templates with verified ID. |
| **Submission Date** | 23 October 2026 | **CONSISTENT** | Converted varied formats (`23/10/2026`, `03 October 2026`) to standardized `23 October 2026`. Historical sprint dates preserved. |
| **Institution** | Jaya Engineering College (JEC) | **CONSISTENT** | Added to metadata tables across all Word documents. |
| **University & Reg.** | Anna University (Regulation 2021) | **CONSISTENT** | Stated on all major phase documents and final report cover. |
| **Department** | Computer Science and Engineering (CSE) | **CONSISTENT** | Stated on final report and FSD document. |
| **Team Members** | 5 Members (Akash Prabhu. P, Gowtham. R, Karthik. K, Gokul Raj K, Douglas Christopher) | **CONSISTENT** | Source `frds` lacked explicit member tables. Full 5-member roster with register numbers and roles embedded in Final Report and FSD. |
| **Faculty Guide** | To be confirmed | **CONSISTENT** | Preserved as `[Faculty Guide / Supervisor Name - To be confirmed]`. No name fabricated. |
| **ServiceNow Table** | `Incident Workflow` (`u_incident_workflow`) | **CONSISTENT** | Consistently referenced across DFD, Tech Stack, FSD, UAT, and Final Report. |
| **Table Fields** | Number, Caller, Category, Subcategory, Short Description, Description, State, Assigned Group, Assigned To | **CONSISTENT** | Exactly matches Table 0 in `Primary_Implementation_Guide.docx`. |
| **Trigger Logic** | Record Created on `Incident Workflow`, Condition: `Category is Empty` | **CONSISTENT** | Consistent in Flow Designer description, DFD, FSD, and UAT. |
| **Keyword Mappings** | Wi-Fi/Network -> Network/Wi-Fi<br>Projector -> Hardware/Projector<br>Password/Login -> Access/Forgot Password<br>Slow/Hanging -> Performance/Slow computer | **CONSISTENT** | Fully verified against Flow Designer condition branches in `Primary_Implementation_Guide.docx`. |
| **Email Action** | Send Email to `Caller -> Email`, Subject: `Your Request for the issue has been submitted.` | **CONSISTENT** | Consistent across Customer Journey Map, Tech Stack, FSD, and UAT. |
| **Sprint Model** | 4 Sprints, 80 Story Points (20 pts/sprint) | **RESOLVED & ALIGNED** | **Major Discrepancy:** Reference team planned 2 sprints (23 pts), while friends planned 4 sprints (80 pts). Prioritized friends' verified work (`Project_Planning_Phase_SWTID-2026-8980.pdf`) and aligned Final Report Section 5 and `Project_Planning_Template.docx`. |
| **Test Scenarios** | TC-001 to TC-004 Pass; TC-005 Fail (Unmatched); TC-006 Pass | **CONSISTENT** | Maintained defect BG-001 (unmatched ticket leaves Category empty) across UAT FSD, UAT Report, and Final Report. No test results fabricated. |

---

## 2. Unresolved Contradictions & Audit Findings
1. **Sprint Planning Discrepancy Resolved:** The reference team used a 2-sprint (23-story-point) timeline. My teammates created a 4-sprint (80-story-point) schedule in `Project_Planning_Phase_SWTID-2026-8980.pdf`. In accordance with prompt rules, our teammates' plan takes precedence. All final documents now consistently report 4 sprints and 80 story points.
2. **Defect BG-001 (No Default Else Branch):** In ServiceNow Flow Designer, the flow only checks the four configured keyword conditions. When an incident short description does not contain any of those keywords, the flow finishes without setting Category or Subcategory. Both the reference UAT and our team's logic confirm this behavior. It is correctly categorized as a known limitation / backlog story USN-9.
