### **PROMPT CHEATSHET - HANDS-ON 1**


#### **1. The "Genuinely Difficult" Lao Wang Transcript Snippet:**
```
Subject: Project Nova - Q3 Strategy Review

Lao Wang: Okay, the main agenda item is the vendor for our new cloud infrastructure. The finance team is still pushing for Vendor B due to cost.

Priya: I'm hesitant. Vendor A has much better security protocols, which is a major concern for the tech team.

Lao Wang: I agree. My final call is that we'll stick with Vendor A, but this is contingent on them providing the updated security compliance report by this Thursday, EOD. If they miss that deadline, we're forced to reconsider.

Alex: That puts pressure on marketing to have the partnership announcement ready. The messaging will need to be updated depending on the outcome.

Lao Wang: Right. That needs to be handled. Also, I reviewed the draft of the legal MSA. It’s missing the data residency clause. This is a showstopper, so it needs to be addressed immediately. Maria, can you get that ball rolling?

Maria: I can. I'll ping Daniel in the legal department right away.
```

#### **2. The Three Levels of Prompts to be Demonstrated:**

**Level 1 Prompt (The "Chatbot" / Brittle Prompt):**
```
Summarize the decisions and action items from the following meeting transcript.

[Paste the transcript here]
```

**Level 2 Prompt (The R.A.F.T. / Reliable "Data Contract" Prompt):**
```markdown
# Role
You are an expert project management assistant.

# Audience
The audience is a downstream computer program, so strict adherence to the JSON format is critical.

# Format
Provide the output in a single JSON object. The JSON must contain two top-level keys: "decisions" and "action_items".
- The "decisions" key should be a list of objects. Each object must have two keys: "decision" and "condition". If there is no condition, the value should be an empty string.
- The "action_items" key should be a list of objects. Each object must have four keys: "owner", "task", "priority", and "initiated_by". If a value is not mentioned, use an empty string.
- Do not include any introductory text or explanations outside of the JSON object.

# Topic & Task
The topic is the following meeting notes. Your task is to extract all decisions and action items, following the formatting rules precisely.

Meeting Notes:
[Paste the transcript here]
```

**Level 3 Prompt (The R.A.F.T. + Few-Shot / "Controlled" Prompt with Business Logic):**
```markdown
# Role
You are an expert project management assistant.

# Audience
The audience is a downstream computer program, so strict adherence to the JSON format is critical.

# Format
Provide the output in a single JSON object. The JSON must contain two top-level keys: "decisions" and "action_items".
- The "decisions" key should be a list of objects. Each object must have two keys: "decision" and "condition". If there is no condition, the value should be an empty string.
- The "action_items" key should be a list of objects. Each object must have four keys: "owner", "task", "priority", and "initiated_by". If a value is not mentioned, use an empty string.
- Do not include any introductory text or explanations outside of the JSON object.

# Topic & Task
The topic is the following meeting notes. Your task is to extract all decisions and action items, following the formatting rules precisely. To ensure accuracy and handle ambiguity, you must follow the logic demonstrated in the example below.

---
**EXAMPLE**
Input: "Let's use the blue design, but only if the client approves. Jane, can you get legal to check the new logo? It's urgent."
Output:
{
  "decisions": [
    {
      "decision": "Use the blue design",
      "condition": "Client must approve"
    }
  ],
  "action_items": [
    {
      "owner": "Legal Department",
      "task": "Check the new logo",
      "priority": "High",
      "initiated_by": "Jane"
    }
  ]
}
---

**MEETING NOTES TO PROCESS:**
[Paste the transcript here]
```

---
