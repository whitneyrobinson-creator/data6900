### **Complete Week 4 Hands-on Package (GitHub Ready)**

# Week 4 Hands-on: The Intelligent Network
**Course:** DATA 6900: AI-Powered Business Process Automation
**Theme:** Adaptive Systems (Routers, Loops, and Logic).

## 1. Sequence Overview

| Step | Activity | PDD Support |
| :--- | :--- | :--- |
| **0** | **Context Priming:** Load Week 3 PDD; Initialize `[SCRATCH_PAD]`. | (Foundation) |
| **1** | **Diagnostic Interview:** User reports failures; AI updates Scratch Pad. | **3.1 Strategy** |
| **2** | **Strategy Analysis:** AI compares Router vs. Loop vs. Parallel. | **3.1 Rationale** |
| **3** | **Visual Blueprint:** AI draws the Advanced Mermaid Map. | **3.2 Map** |
| **4** | **Component Design:** Defining the Router & Critic Specs. | **3.4 Specs** |
| **5** | **Logic OS & Trace:** Writing the Logic Block and running the Sim. | **3.3 & 3.5** |
| **6** | **The Compiler:** Generating the reproducible Master Prompt. | **(Deliverable)** |

---

## 2. Implementation Artifacts

### Artifact 0: Context Priming (Step 0)
**Goal:** Initialize the AI with Week 3 constraints.

```markdown
# Role
You are a Senior AI Workflow Architect.

# Task
Read the attached **Week 3 PDD (Milestone 2)**. 
1. Extract the core Business Rules (Budget limits, MSA triggers).
2. Extract the Current Architecture (The 3-node Linear Chain).
3. Store these in a visible `[SCRATCH_PAD]` block at the start of your response.
4. **Stop** and await further instructions.

# Input
[PASTE WEEK 3 PDD HERE]
```

### Artifact 1: The Diagnostic Interview (Step 1)
**Goal:** Interactive diagnosis of specific node failures.

```markdown
# Role
You are a Diagnostic Systems Engineer.

# Task
Interview me to identify specific failure points in the Week 3 Linear Pipeline.

# Protocol
1. **One Question at a Time:** Ask targeted questions about each node (Gatekeeper, Judge, Worker) individually.
2. **Focus Areas:**
   - Ask about **Gatekeeper** robustness (e.g., "Did it fail on vague inputs?").
   - Ask about **Judge** reasoning (e.g., "Did it make lazy assumptions?").
   - Ask about **Worker** tone/risk (e.g., "Did it promise things it shouldn't?").
3. **Action:** After each answer, update the `[SCRATCH_PAD]` with the specific "Failure Mode" identified.

# Start
Begin by asking about the Gatekeeper.
```

### Artifact 2: The Strategy Analysis (Step 2)
**Goal:** Compare patterns (Router/Loop/Parallel) and get user buy-in.

```markdown
# Role
You are a Solutions Architect.

# Task
Analyze the "Failure Modes" in the `[SCRATCH_PAD]`. 
Compare three Adaptive Patterns: **Router**, **Evaluator-Optimizer Loop**, and **Parallel Workers**.

# Output Requirement
Provide a **Strategy Comparison Table**:

| Target Node | Proposed Pattern | Pros | Cons | Recommendation |
| :--- | :--- | :--- | :--- | :--- |
| **Gatekeeper** | **Router (Triage)** | Filters noise upstream. | Adds latency. | **RECOMMENDED** for Issue A (Noise). |
| **Judge** | **Evaluator Loop** | Enforces strict quality. | Can get stuck in loops. | **RECOMMENDED** for Issue B (Laziness). |
| **Judge** | **Parallel Workers** | Faster (Checks Budget & Legal at same time). | Harder to resolve conflicts. | **REJECTED** (Accuracy > Speed). |

# Constraint
Do not generate any code or diagrams yet.
**STOP** and ask: "Do you approve this architecture strategy?"
```

### Artifact 3: The Advanced Mermaid Map (Step 3)
**Goal:** Generate the PDD 3.2 Diagram based on the approved strategy.

```markdown
# Role
Visualization Expert (Mermaid.js).

# Task
Generate the **Week 4 Advanced Network Diagram** (`graph TD`) based on the **Approved Strategy**.

# Requirements (PDD 3.2)
1. **Implement the Router:** Insert a Decision Diamond (`{?}`) *before* the Gatekeeper. 
2. **Implement the Loop:** Insert a Critic Node and Decision Diamond *after* the Judge.
   - Show the "Feedback Arrow" looping back to the Judge.
3. **Styling:** 
   - Keep the Week 3 nodes in Orange (`#FFF4DD`).
   - Highlight the new **Router** and **Critic** nodes in Green (`#E6FFFA`) with a distinct border.

# Output
Provide the Mermaid code only.
```

### Artifact 4: Component Spec Generator (Step 4)
**Goal:** Generate PDD 3.4 Specs (Modules A & B).

```markdown
# Role
Senior Tool Engineer.

# Task
Design the specifications for the new components defined in the Approved Strategy.

# Instructions
1. **Router Spec:** Define the `Input Variable`, `Output Categories` (e.g., VALID, AMBIGUOUS, SPAM), and the RAFT prompt.
2. **Critic Spec:** Define the `Input Variable`, the `Evaluation Rubric` (Rules from Scratch Pad), and the RAFT prompt.
3. **Format:** Output clearly labeled sections ready for **PDD Section 3.4**.
4. **Order**: proposed one node at a time. Do not proceed until the user approves.
```

### Artifact 5: The Logic OS & Trace (Step 5)
**Goal:** PDD 3.3 (Logic) and 3.5 (Trace).

```markdown
# Role
System Orchestrator.

# Task 1: The Logic OS (PDD 3.3)
Write the "Operating System" logic block.
- Define `### VARIABLES` (from Scratch Pad).
- Define `### CONDITIONS` using IF/ELSE for the Router and WHILE/LOOP for the Critic.

# Task 2: The Master Simulation (PDD 3.5)
Execute this logic on a "Stress Test" input (e.g., A request that is valid but missing the MSA citation).
- **Requirement:** Output a **Trace Log** showing the decision path:
  `[ROUTER] -> VALID`
  `[JUDGE] -> APPROVE`
  `[CRITIC] -> REJECT (Reason: MSA missing)`
  `[JUDGE] -> RETRY`
  `[RESULT] -> FINAL MEMO`
```

### Artifact 6: The Master Compiler (Step 6)
**Goal:** Generate the reproducible System Prompt.

```markdown
# Role
Lead AI Engineer and System Integrator.

# Task
Compile all components designed in this session (Logic OS, Router, Critic, Core Chain) into a **Single, Self-Contained "Master System Prompt"**.
I should be able to paste this output into a fresh LLM window to run the entire simulation from scratch.

# Requirements
1. Include `### VARIABLES` and `### CONDITIONS`.
2. Include the full definition of every Tool (RAFT Prompts).
3. Enforce the **Trace Log** output format.
```




