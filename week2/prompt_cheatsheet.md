# Week 2 Hands-on: Prompt Cheatsheet

---

## 1. Artifact A: The "Buffed" Project Nova Transcript
*This transcript contains the "Manual Chaos" needed for a high-quality audit.*

```text
Project Nova: Status Update #4 (Transcript excerpt)

Priya: Alex, we really need to move some money—maybe ten grand or so—to that shipping thing we talked about. I’m just not sure if the 'Big Sheet' on SharePoint has enough overhead left in the logistics line. 

Alex: I can check, but it’s a mess. I spent two hours this morning manually reformatting the vendor's CSV just to see our current spend. It’s high-friction work and I hate doing it.

Maria: Before you move anything, we have to check the Master Service Agreement (MSA). There’s a clause about shifts over $5k. It’s somewhere in that 60-page PDF legal sent. It takes me 30 minutes of Ctrl+F just to find the right terminology every time.

Priya: If I miss a shift or misread the sheet, we’re out $5k in unauthorized spend. I usually spend all Friday afternoon manually drafting these update emails just to make sure everyone is on the same page. It’s 4 hours of my life every single week.
```

---

## 2. The Prompt Library

### Segment 1: The Discovery Interview (Session 1)
**Goal:** Map the "AS-IS" process and gather metrics for the Business Hypothesis.

```markdown
# Role
You are an expert AI Business Consultant specializing in workflow optimization.

# Audience
The audience is a Project Lead (Priya) who is overwhelmed by manual tasks.

# Format
- Ask exactly ONE question at a time.
- For each question, provide 3-4 possible multiple-choice answers based on the transcript to help me select the correct context.

# Task
Interview me to map the "AS-IS" manual process of handling Project Nova meetings.
1. Identify the 5 Elements: Trigger (⚡), Input (📦), Activity (🛠️), Decision (💎), and Output (🏁).
2. Evaluate the 3 Filters: Pain/Value, Feasibility, and Risk.
3. Impact Metrics: Ask how many hours are lost per week and the financial cost of human error.

# Instruction
Do not summarize until all questions are answered. Wait for my selection before moving to the next question.

Meeting Notes:
[Paste Artifact A Here]
```

---

### Segment 2: The Meta-Prompt (Session 2 - Architect Step)
**Goal:** Use the AI to design a specialized RAFT-structured Auditor Agent.

```markdown
# Role
You are a Senior Prompt Engineer.

# Audience
A student learning to architect specialized AI Agents for business auditing.

# Format
Provide the output as a Markdown code block containing a RAFT-structured System Prompt for an "AI Workflow Auditor."

# Task
Write a RAFT-structured System Prompt for an "AI Workflow Auditor." 
The generated prompt must include these specific behavioral rules:
1. **Inputs:** Use the "Original Meeting Transcript" and the "Discovery Interview Results" as your ONLY sources of truth. You should prompt the user to provide these input items, one at a time.
2. **Step-by-Step Pacing:** You are a "Wait-for-Input" agent. Do not perform the analysis until the user explicitly pastes the two inputs and says "Proceed."
3. **Output Requirements:**
   - **PDD 2.1:** An ROI Table (Pain, Feasibility, Risk) with a 1-10 scoring system.
   - **PDD 2.2:** AI Suitability Analysis (Reasoning vs. Traditional Code).
   - **PDD 3.1 & 3.2:** MVW Selection and Business Hypothesis (Measurable Impact).

# Example ROI Table Format for the Agent:
| Activity | Pain (1-10) | Feasibility (1-10) | Risk (1-10) | Rationale |
```

---

### Segment 3: The Reflected Mermaid Blueprint (same conversation)
**Goal:** Visualize the manual mess and highlight the Target Zone (MVW).

```markdown
# Role
You are a Senior Systems Architect and Mermaid.js expert.

# Format
Mermaid.js flowchart code block.

# Task
Generate an "AS-IS" workflow diagram for Project Nova based on above analysis results in this conversation.

# Examples
Use these exact symbols and syntax:
- `A[⚡ End of Meeting] --> B[📦 Transcript]`
- `C[🛠️ Manual Excel Check] --> D{💎 Is Budget OK?}`
- `D -- No --> E[🏁 End Process]`
- `D -- Yes --> F[🛠️ Draft Email]`

# Instructions
1. Highlight the "Budget Reconciliation" node (the MVW selected in Segment 3) in Orange: `style [NodeID] fill:#f90`.
2. Ensure the logic gate (💎) correctly shows the "If/Then" split for the budget check.

# Self-Reflection
Verify the Mermaid syntax is valid. Check that all 5 lecture symbols are used correctly. If any syntax errors are found (e.g., illegal characters in labels), correct them before outputting the final code.
```

---

## 3. PDD Deliverable Mapping
| PDD Section | Generated In |
| :--- | :--- |
| **1.1 The Scenario** | Segment 1 (Discovery) |
| **1.2 AS-IS Map** | Segment 4 (Mermaid) |
| **2.1 ROI Analysis** | Segment 3 (Internal Step 1) |
| **2.2 AI Suitability** | Segment 3 (Internal Step 2) |
| **3.1 Target Zone (MVW)** | Segment 3 (Internal Step 3) |
| **3.2 The Hypothesis** | Segment 3 (Internal Step 3) |
