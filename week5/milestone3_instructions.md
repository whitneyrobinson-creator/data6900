# Milestone 3 – Business Case & Final Design (V3.0) Instructions

**Due:** Before Week 6 Live Session
**Format:** Updated PDD (Markdown/PDF) + ROI One-Pager
**Weight:** 15% of Course Grade

### **The Mission: From Experiment to Asset**
In Milestone 2 (MVW), you proved that your "Assembly Line" *could* work. But in the real world, "could work" isn't enough. It must be **Safe** (protected from risk) and **Profitable** (worth the cost).

Your goal is to upgrade your workflow to **Version 3.0**. You will install the "Control Room" components (Auditor, HITL) and calculate the "Iceberg" costs to prove the business value to your client.

---

### **The Steps**

#### **1. Upgrade to V3.0 (Advanced Logic)**
*   **The Architecture:** Update your Mermaid flowchart from Week 2.
*   **The Requirement:** You must move beyond a linear chain. Your V3.0 map must include:
    *   **The Auditor Node:** A specific step where the AI evaluates its own output *before* final action.
    *   **Routing Logic:** A "Diamond" decision point (e.g., `IF Risk > High THEN...`).
    *   **The Resurrection Point (HITL):** A clear path where the process stops and routes to a human if the Auditor flags a risk.

#### **2. Define the Safety Spec (The Auditor)**
*   Define the **Spec (SDD)** for your new Auditor Node.
*   **The Rules:** List the 3-5 "Fatal Errors" your Auditor is checking for (e.g., Hallucinations, Bias, Financial Limits).
*   **The Prompt:** Write the System Prompt for the Auditor (using the R.A.F.T. framework). It must output **JSON** (Score/Flag), not chat.

#### **3. Stress Test (Red Teaming)**
*   You cannot assume your bot is safe; you must prove it.
*   **The Attack:** Attempt to break your own workflow using **Prompt Injection** or **Edge Cases** (as practiced in the Week 5 Live Session).
*   **The Evidence:** Include your **"Attack Log"** in the PDD. Show at least 3 attempts:
    *   *Attack Input* $\to$ *Auditor Response* $\to$ *Outcome (Blocked/Failed)*.

#### **4. The Business Case (ROI & KPIs)**
*   **The Pain Audit:** Identify the **one** SMART KPI that matters. (e.g., "Reduce processing time from 4 hours to 15 minutes").
*   **The Math:** Use the **ROI Excel Template** provided in class to calculate:
    *   **TCO (Total Cost of Ownership):** Development time + Maintenance + API costs.
    *   **Value:** Human hours saved $\times$ Hourly rate.
    *   **Break-Even Point:** How many runs does it take to pay back the investment?
*   *Output:* Export the "Verdict" section of your Excel sheet (Net Profit & Break-Even) into your report.

---

### **Deliverable Checklist**

Please submit a **Single PDF** (The Updated Process Design Document) containing:

1.  **V3.0 Logic Map:** The updated Mermaid diagram with Auditor & HITL.
2.  **Auditor Spec:** The Input/Output Schema and System Prompt for your Safety Node.
3.  **Validation Log (The Attack Log):** Evidence that your Auditor catches "Bad Inputs."
4.  **The Business Case:**
    *   Your SMART KPI definition.
    *   The ROI Summary (Cost vs. Value vs. Break-Even).

---

### **Grading Rubric (Milestone 3)**

| Criteria | Excellent (4 pts) | Satisfactory (2 pts) | Needs Improvement (1 pt) |
| :--- | :--- | :--- | :--- |
| **Advanced Workflow Design (V3.0)** | The workflow includes a functional **Auditor Node** and a strategically placed **HITL** point. The logic handles failure gracefully (Loops/Routing). | The workflow is enhanced with an Auditor/HITL, but the placement feels illogical or "tacked on." | The workflow remains linear or lacks safety mechanisms. |
| **Business Case & KPI Analysis** | **SMART KPIs** are clearly defined. Financial assumptions (TCO/ROI) are realistic and defensible based on the "Iceberg" concept. | Business case is present, but KPIs are vague (e.g., "Improve efficiency") or financial math is missing. | Business case is missing or superficial. |
| **Safety Validation (Red Teaming)** | **Attack Log** proves the system was stress-tested. The Auditor successfully blocks specific risks defined in the spec. | Validation is present but only tests "Easy" cases. No evidence of resisting Injection Attacks. | No evidence of testing provided. |
| **Documentation Quality** | PDD is professional, updated clearly from V2.0, and "Client-Ready." | PDD is updated but messy or difficult to follow. | Document is incomplete or formatting is broken. |
