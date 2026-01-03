### **The Showcase Playbook (Run-of-Show)**
**Use this to fill the 45-minute slot in Week 14.**

#### **PART 1: THE PITCH (0:00 - 10:00)**
*   **Slide 1:** The Hook (The "Villain" - Human Pain).
*   **Slide 2:** The "Iceberg" (TCO/ROI).
*   **Slide 3:** The Pivot Story (Your STAR Narrative).

#### **PART 2: THE DEMO CHOREOGRAPHY (10:00 - 25:00)**
*Do not use "Engineer Voice." Use "Value Commentary."*

**Pre-Demo Setup:**
1.  Open **Tab 1**: The Trigger App (e.g., Typeform/Gmail).
2.  Open **Tab 2**: n8n Editor (Zoomed to 150%).
3.  Open **Tab 3**: The Destination App (e.g., Slack/Sheets).

**The Scripted Flow:**
1.  **The Trigger (Min 0-5):** Submit the request as a customer.
2.  **The "Under the Hood" (Min 5-10):** Switch to n8n.
    *   **Engineer Voice (BAD):** *"This HTTP node sends a GET request to the API and parses the JSON."*
    *   **Value Commentary (GOOD):** *"Right here, the AI is reading the email. This task used to take Lao Wang 5 minutes of reading time. The green light means we just saved $4.50 in billable time instantly."*
    *   *Rule:* Every time you point at a node, mention **Speed**, **Risk**, or **Cost**.
3.  **The Resilience Check (Min 10-15):**
    *   Force an error (Injection/Bad Input).
    *   Show the **Auditor Node** blocking it.
    *   *Commentary:* "A cheaper bot would have just refunded $5,000 here. Our governance layer caught it, saving the company from fraud."
4. Other contents to consider (IMPORTANT):
     * *what we delivered is a detailed "proof of concept" - the student group ("we") are willing to work with your organization to make it production level*
     * *user training/testing plan*
     * *other measures to make it to the next level (production)* 

#### **PART 3: THE INQUISITION (25:00 - 45:00)**
*Prepare for the Partner's Questions.*

**1. The "Bridge" Technique (If you don't know the answer):**
*   *"That is an excellent feature for Phase 2 (refer to Section 6 of Proposal). In this MVP, we prioritized [X] for cost reasons, but the architecture allows us to add [Y] easily."*

**2. The "Black Swan" Defense (The Pre-Mortem):**
*   **Judge's Question:** *"What kills this project in 6 months?"*
*   **Your Prepared Answer:** *"We identified [Risk, e.g., OpenAI pricing changes] as the biggest threat. That is why we used a modular **Model Switch** node. We can swap OpenAI for Anthropic or a Local Llama model in 15 minutes without rewriting the logic."*
