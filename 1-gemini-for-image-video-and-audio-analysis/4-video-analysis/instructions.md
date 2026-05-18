# Store Safety Compliance

## Overview
This play teaches you how to use Gemini's multimodal reasoning to conduct a high-precision safety audit from raw store walk-through footage. You will start with a simple prompt, then add policy context, and finish by structuring the output for operational use.

### Objectives
In this play, you learn how to:
- Transform unstructured video data into actionable safety findings.
- Improve analysis quality by layering context and prompt structure.
- Generate a manager-ready compliance report with clear recommendations.

## Instructions

---

### Part 1: Baseline Video Analysis
Goal: Establish a baseline and show what Gemini can do with minimal instructions.

Estimated time: 5 to 7 minutes

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

Estimated time: 6 to 8 minutes

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

Estimated time: 7 to 9 minutes

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

### Bonus: Generate a Manager Memo
Goal: Turn technical findings into a communication artifact leaders can use immediately.

Estimated time: 4 to 6 minutes

1. In the same chat from Part 3, copy and paste the following prompt, then press ENTER.

```
Using your audit results, draft a professional memo addressed to the Store Manager.

Requirements:
- Tone: Professional, direct, and constructive.
- Include: Executive summary, top risks, and required immediate actions.
- Include a 7-day action plan with owner roles and deadlines.
- Close with a short follow-up request for status reporting.
```

2. Save the memo and the structured audit output for sharing.

---