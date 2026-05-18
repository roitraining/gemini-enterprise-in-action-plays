# Store Safety Compliance

## Overview
This play teaches you how to use Gemini's multimodal reasoning to conduct a high-precision safety audit from raw store walk-through footage. You will start with a simple prompt, then add policy context, and finish by structuring the output for operational use.

### Objectives
In this play, you learn how to:
- Transform unstructured video data into actionable safety findings.
- Improve analysis quality by layering context and prompt structure.
- Generate a manager-ready compliance report with clear recommendations.

## Instructions



### Part 1: Baseline Video Analysis
Goal: Establish a baseline and show what Gemini can do with minimal instructions.

1. Open Gemini Enterprise in your browser.
2. Click the `+ Add files` icon and select `Upload files`.
3. In the dialog, select `store.mp4` and click `Open`.
4. In the chat, copy and paste the following prompt, then press ENTER.

```
Analyze this store walk-through video and identify potential safety hazards.
Include timestamps and a short description of each issue.
```

5. Review the output and discuss:
   - What did Gemini identify well?
   - What seems ambiguous or inconsistent?
   - What information is missing for operational use?

---

### Part 2: Add Company Standards
Goal: Improve precision by grounding the analysis in policy.

1. Click `New chat` to start a fresh session.
2. Click the `+ Add files` icon and select `Upload files`.
3. In the dialog, select `store.mp4` and `Cymbal-Mart_VisualMerchandising_and_Store_Standards.pdf`, then click `Open`.
4. In the chat, copy and paste the following prompt, then press ENTER.

```
Role: You are the Primary Safety Manager for Cymbal-Mart.
Task: Analyze the provided store walk-through video and identify all instances of non-compliance.
Instruction: Use the "Cymbal-Mart Visual Merchandising and Store Standards" document as the authority for determining violations.
For each issue found, include the timestamp and cite the relevant policy section.
```

5. Compare this output with Part 1:
   - Which findings are more credible now?
   - Where did policy grounding improve specificity?
   - What is still difficult to scan quickly?

---

### Part 3: Add Structured Output Requirements
Goal: Convert policy-grounded findings into an action-ready audit format.

1. Click `New chat` to start a fresh session.
2. Click the `+ Add files` icon and select `Upload files`.
3. In the dialog, select `store.mp4` and `Cymbal-Mart_VisualMerchandising_and_Store_Standards.pdf`, then click `Open`.
4. In the chat, copy and paste the following prompt, then press ENTER.

```
Role: You are the Primary Safety Manager for Cymbal-Mart conducting a virtual compliance audit.
Task: Analyze the store walk-through video and identify every non-compliance issue based strictly on the "Cymbal-Mart Visual Merchandising and Store Standards" document.

Output Format:
1) Audit Log (chronological)
- [Timestamp]
- [Violation Category]
- [Policy Section Citation]
- [Description of Hazard]
- [Severity: Low, Medium, High, Critical]

2) Critical Risk Summary
- List the top 3 most dangerous issues requiring immediate intervention.

3) Operational Recommendations
- Provide short prevention recommendations for the Store Manager.
```

5. Review the result and highlight how output formatting improves:
   - readability,
   - prioritization,
   - and operational follow-through.

---

### Bonus: Generate a Manager Memo with the CARE Prompt Format
Goal: Apply a CARE prompt to transform your raw audit findings into a professional memo leaders can use immediately. The CARE framework is a structured prompt technique that improves clarity and consistency. CARE stands for:

- **Context**: Establish the background, situation, and stakes.
- **Action**: Specify exactly what you want the model to do and how.
- **Result**: Define the output format, tone, and expected deliverables.
- **Evaluation**: State how success will be measured.

1. In the same chat from Part 3, copy and paste the following CARE-structured prompt, then press ENTER.

```
Context:
You are a Senior Compliance Auditor for a national retail chain. You have just completed a high-stakes operational audit of a local branch. The audit revealed several critical failures in inventory management, safety protocols, and cash handling that require immediate intervention to prevent financial loss and safety hazards.

Action:
Using the audit data provided, draft a professional memo addressed to the Store Manager. Your writing must be direct, constructive, and avoid fluff. You must:

Synthesize the findings into a concise Executive Summary.

Identify and prioritize the 'Top 3 Risks' based on their impact on the business.

Outline specific 'Immediate Actions' to be taken within 24 hours.

Construct a 7-day Action Plan in a table format with columns for Task, Owner (e.g., Ops Lead, Floor Manager), and Deadline (Day 1–7).

Result:
The final memo should be formatted for internal distribution, using clear headings and a tone that balances accountability with professional support. It must conclude with a formal request for a status report by a specific date.

Evaluation:
"Success will be measured by the clarity of the risk assessment and the feasibility of the 7-day plan. Ensure the language is firm enough to convey urgency but constructive enough to maintain a positive working relationship with the Store Manager.
```

2. Review the output and notice how the CARE structure delivered:
   - Clear expectations about tone and format.
   - A logical flow from summary to risk to action.
   - Credible, actionable next steps the Store Manager can execute.

3. Save the memo and the structured audit output for sharing.

---