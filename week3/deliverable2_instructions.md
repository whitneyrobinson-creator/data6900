# Week 3 Assignment Instructions

**Assignment:** Milestone 2 – MVW Design & Prototyping
**Due:** Before Week 4 Live Session
**Format:** Updated PDD (Markdown/PDF)
**Weight:** 10% of Course Grade

### **The Mission: From Diagnosis to Blueprint**
In Week 2, you diagnosed the "Spaghetti" (The Manual Process). Now, you must design the **Assembly Line** (The Automated Solution).

Your goal is to design a **Linear Minimum Viable Workflow (MVW)** that replaces the manual bottleneck. You will not write Python or n8n code yet; instead, you will use **Spec-Driven Development** to prove your logic works in a manual simulation.

### **The Mission: From Diagnosis to Blueprint**
In Week 2, you diagnosed the "Spaghetti" (The Manual Process). Now, you must design the **Assembly Line** (The Automated Solution).

Your goal is to design a **Linear Minimum Viable Workflow (MVW)** that replaces the manual bottleneck. You will not write Python or n8n code yet; instead, you will use **Spec-Driven Development** to prove your logic works in a manual simulation.

### **The Steps**

**1. Design the "To-Be" Architecture**
*   Take your "As-Is" Map from Week 2.
*   Create a new **Mermaid Flowchart** representing the automated "To-Be" state.
*   It must follow the **Universal Dispatcher** pattern:
    *   **Input** $\to$ **Gatekeeper** (Extraction) $\to$ **Judge** (Reasoning) $\to$ **Worker** (Drafting) $\to$ **Output**.

**2. Draft the R.A.F.T. Prompts**
*   Write the **System Prompts** for your 3 Nodes (Gatekeeper, Judge, Worker).
*   Use the **R.A.F.T. Framework** to define the Role, Audience, Format, and Task.
*   *Tip:* Start with natural language instructions.

**3. Audit with Tool Specs (SDD)**
*   Now, act as an Engineer. Look at the prompts you just wrote.
*   Fill out the **Tool Specification Canvas** (Section 2.3 of the PDD) based on your prompts.
*   **The Check:** Does your prompt *actually* guarantee the Output Schema you defined in the Spec? If not, go back and tighten the prompt (e.g., add "Output RAW JSON ONLY").

**4. The "Proof of Life" (Simulation)**
*   Use the `Workflow_Engine_Simulator.txt` method (or the Auto-Simulator prompt).
*   Run a real example (e.g., a real email or job description) through your chain.
*   **Paste the Chat Log** into your PDD as proof that the logic holds together.

**5. Define the ROI (KPIs)**
*   Estimate the value using the 4 Metrics (Efficiency, Quality, Cost, Satisfaction).

---

### **Grading Rubric (Milestone 2)**

| Criteria | Excellent (4 pts) | Satisfactory (2 pts) | Needs Improvement (1 pt) |
| :--- | :--- | :--- | :--- |
| **Tool Specification (SDD)** | Inputs/Outputs are rigorously defined (e.g., specific JSON keys). Failure modes (Grounding) are addressed. | Inputs/Outputs are defined but vague. Missing failure modes. | No clear specification; jumps straight to prompting. |
| **Prompt Engineering (R.A.F.T.)** | Prompts strictly follow R.A.F.T. Gatekeeper enforces JSON; Judge enforces Reasoning. No "chatty" pollution. | Prompts use R.A.F.T. but allow some "pollution" or unstructured output. | Prompts are conversational ("Please help me") rather than structural. |
| **Validation (Simulation)** | Chat log proves the chain works end-to-end on a real example. Logic is sound. | Chat log included but shows minor hallucinations or format errors. | No evidence of testing provided. |
| **Business Value (KPIs)** | At least one "Hard Metric" (Time/Cost) is quantified with realistic estimates. | Only "Soft Metrics" (Satisfaction) or vague estimates provided. | Value section missing or trivial. |
