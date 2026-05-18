# Back to School Infographic

## Overview
This play teaches you how to use Gemini's Nano Banana 2 model to turn a promotional concept into a high-fidelity infographic. You will start with a generic baseline, add research-backed numbers, and finish by using meta-prompt engineering to improve consistency.

### Objectives
In this play, you will learn how to:
- Generate a baseline infographic from a simple prompt.
- Use Gemini research capabilities to find and verify current data points.
- Build a second infographic that uses approved statistics.
- Apply meta-prompt engineering to improve control and output quality.

## Instructions

---

### Part 1: Baseline Infographic
Goal: Establish a simple, generic version as the baseline.

1. Open Gemini Enterprise in your browser.
2. Click `New chat` to start a fresh session.
3. In the chat bar, select the Tools icon and choose `Generate images (NB2)`.
4. Copy and paste this baseline prompt, then press ENTER:

```text
Create a horizontal infographic promoting a back-to-school campaign for Cymbal-Mart.
Use a clear left-to-right story: challenge on the left, solution on the right.
Keep text minimal and readable, with a bold headline, 3 data callouts, and a closing tagline.
Visual style: energetic, family-friendly, polished marketing graphic.
```

5. Review the result and discuss:
- What is clear?
- What is vague or unsupported?
- Which details should be backed by real numbers?

---

### Part 2: Research and Approve Numbers
Goal: Gather current, source-backed statistics before creating the next infographic.

1. Click `New chat` to start a fresh session.
2. Copy and paste this research prompt, then press ENTER:

```text
Research current U.S. back-to-school spending statistics for families with K-12 students.
Find 3-5 high-confidence figures suitable for a retail infographic, including:
- Average annual household spend
- Percent of shoppers planning to shop early
- Top spending categories
- Value-seeking behavior (discounts, private label, or deal participation)

Requirements:
- Prioritize 2024-2025 data.
- Provide source name, publication date, and direct URL for each figure.
- Flag conflicting numbers and recommend one value to use.
- Return a final "Approved Data Block" with exactly 3 numbers formatted for infographic text.
```

4. Review Gemini's response and confirm each number has:
- A source
- A date
- A clear explanation

5. Copy the final `Approved Data Block` from the response.

---

### Part 3: Build the Evidence-Based Infographic
Goal: Create a second infographic using the approved numbers exactly.

Estimated time: 9 minutes

1. Click `New chat` to start a fresh session.
2. In the chat bar, select the Tools icon and choose `Generate images (NB2)`.
3. Copy and paste the prompt below. Replace `[PASTE APPROVED DATA BLOCK HERE]` with your research output.

```text
Create a striking, horizontal infographic-style image promoting "Cymbal-Mart: Back-to-School Super Sale."

Use this approved data exactly as written:
[PASTE APPROVED DATA BLOCK HERE]

Composition:
- Left panel: family spending challenge
- Right panel: Cymbal-Mart value solution
- Include all 3 approved numbers as highly legible callouts
- Add one strong CTA banner at the bottom

Design constraints:
- Clean visual hierarchy and high contrast for readability
- Keep copy concise and presentation-ready
- Do not change any numeric values
- Keep the image horizontal
```

4. Compare this result to Part 1.
5. Identify what improved due to research-backed data.

---

### Bonus: Meta-Prompt Engineering
Goal: Use Gemini to engineer a stronger, structured image prompt format.

1. Click `New chat` to start a fresh session.
2. Copy and paste this meta-prompt, then press ENTER:

```text
Engineer the following infographic prompt using these sections:
Persona, Role, Inputs, Steps, Constraints, and Output Format.
Preserve all campaign intent and all approved numeric values exactly.
Then provide one final optimized prompt.

[PASTE YOUR PART 3 PROMPT HERE]
```

3. Copy the optimized prompt Gemini returns.
4. Open another `New chat`, select `Generate images (NB2)`, and run the optimized prompt.
5. Compare all three outputs (Part 1, Part 3, Bonus) and discuss:
- Which output is most persuasive?
- Which one is most trustworthy?
- How did prompt structure affect quality?

---

### Wrap-Up
Save your best final image for sharing. In your reflection, include one thing that improved after research and one thing that improved after meta-prompt engineering.