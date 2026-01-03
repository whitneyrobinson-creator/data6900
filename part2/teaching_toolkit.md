## **Artifact 4: The Teacher & Builder’s Toolkit**
**Purpose:** AI Prompts to help students Design the Lesson, Build the Tech, and Defend the Strategy.


---

### **PART A: PEDAGOGY (Designing Your Lesson)**
*Use these prompts to prepare for your 60-minute teaching slot.*
> Besides below prompt, make use of all the prompting patterns you learned in Part 1 of the course.

**1. The "Analogy Architect" (Explaining the Unfamiliar)**
*Don't just say "JSON Object." Use a relatable comparison.*
> **Prompt:** "Act as a Technical Trainer. I need to explain **[Concept, e.g., 'Webhooks' or 'JSON Arrays']** to a class of business consultants who are not coders.
> **Task:** Give me 3 distinct analogies (e.g., using Logistics, Cooking, or Office Mail) to explain how this concept works.
> **Constraint:** Keep it simple, visual, and professional."

**2. The "Pacing Auditor" (Time Management)**
*Most students try to teach too much. Check your scope.*
> **Prompt:** "Here is my outline for a 60-minute 'Code-Along' workshop: **[Paste Outline]**.
> **Audience:** Graduate students with mixed technical skills.
> **Task:** Critique my timing. Where is the class most likely to get stuck or fall behind? Suggest exactly where I should add 'Buffer Time' or 'Checkpoints'."

**3. The "Q&A Simulator" (Anticipating Confusion)**
*Don't get blindsided during the Q&A session. Practice against a simulated student.*
> **Prompt:** "Act as a curious but confused MBA student attending an n8n workshop.
> **Context:** I just taught a lesson on **[Topic, e.g., Merging Data Streams]**.
> **Task:** Ask me 3 difficult questions that a beginner would likely ask at this point. Challenge my explanation."

---

### **PART B: RESEARCH (The Source of Truth)**

**4. The "Tutorial Adapter" (Generic $\to$ Specific)**
*Turn the official docs into a custom lesson for your project.*
> **Prompt:** "I have a generic tutorial from the n8n documentation on **[Insert Topic, e.g., 'Merging Data']**.
> **My Specific Context:** I am building a Refund Bot for a Dropshipping owner. I need to merge 'Shopify Order Data' with 'Gmail Customer Emails'.
> **Task:** Rewrite the steps of this generic tutorial to match my specific context. Tell me exactly what data fields to use in my example instead of the generic ones."

**5. The "Solution Scout" (Problem $\to$ Documentation)**
*Don't know which node to use? Ask the AI to point you to the right docs.*
> **Prompt:** "Act as a Senior n8n Developer.
> **My Problem:** I need to **[Describe Goal, e.g., 'Wait for a user to click a link in an email before continuing']**.
> **Task:** Identify the specific n8n Nodes I should use. Suggest search terms I should use in the **Official n8n Documentation** to find the correct reference manual."

---

### **PART C: BUILDING (The Implementation)**

**6. The "Code Generator" (Text-to-n8n)**
*Don't hand-code complex JSON configurations. Generate them.*
> **Prompt:** "Act as an n8n Expert. Create the JSON code for an n8n **[Node Type, e.g., HTTP Request]** node.
> **Configuration:** Method: POST. URL: [Insert URL]. Headers: Authorization: Bearer [Key]. Body: {'text': 'Hello'}.
> **Output:** Provide raw JSON I can paste into the canvas."

**7. The "Debug Loop" (When it breaks)**
*Stuck on a red error? Paste it.*
> **Prompt:** "I am getting this error in n8n: `[Paste Error Code/Message]`.
> **Context:** I am passing data from a Webhook to OpenAI.
> **Task:** Explain what this error means in plain English and give me the fix."

**8. The "Expression Wizard" (Handlebars/JS)**
> **Prompt:** "I need an n8n Expression.
> **Input JSON:** `{'customer': {'first_name': 'Lao', 'orders': 5}}`.
> **Goal:** Return the string: 'VIP Customer Lao' if orders > 3, else 'Standard Customer'.
> **Output:** Give me the Ternary Operator expression."

---

### **PART D: STRATEGY (The Defense)**

**9. The "Parsimony Check" (Efficiency Defense)**
*Use this to prepare for the Q&A "Red Team" attacks.*
> **Prompt:** "I am using an LLM Node to extract an email address from a text block.
> **Critique Me:** Is this an efficient use of compute? Compare the cost/speed of using GPT-4 vs. using a Regex Extraction Node.
> **Output:** A pros/cons list I can use to defend my decision."

**10. The "Resilience Audit" (Happy Path Check)**
> **Prompt:** "Look at this logic flow: [Describe flow].
> **Task:** Identify 3 ways this could break in a production environment (e.g., timeouts, empty data).
> **Output:** Suggest a 'Fallback' logic for each failure mode."
