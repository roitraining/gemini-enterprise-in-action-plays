# Meta Prompting for Deep Research (Investment Diligence)

## Time Required
12-15 minutes

## Overview
This lab teaches students how meta prompting improves Gemini Enterprise Deep Research quality.

Instead of only asking a company question, students first ask Gemini to design a better Deep Research prompt. They then compare results from a weak prompt versus a meta-prompted prompt.

### You learn how to:
- Explain what meta prompting is in practical terms.
- Identify when to use meta prompting before Deep Research.
- Build a stronger Deep Research request from a weak starting prompt.
- Compare evidence quality, structure, and decision usefulness across outputs.

## What Is Meta Prompting?
Meta prompting means prompting the model to create or improve another prompt before running the main task.

For Deep Research, this helps because the quality of the research plan and final answer depends heavily on prompt clarity, scope, output format, and evidence standards.

## Scenario
Cymbal Capital Partners is a fictional venture capital and private equity firm looking for its next investment opportunity.

Your class will evaluate one company and decide whether the available evidence supports a go/no-go recommendation.

## Lab Instructions

### Task 1: Run a Weak Baseline Prompt

1. Open Gemini Enterprise in a new chat.

2. Select **Deep Research** from **Tools**.

3. Use this intentionally weak prompt:

```text
Research potentially companies on behalf of Cymbal Capital Partners - a venture capital and private equity firm looking for its next investment opportunity - and tell me if it is a good investment.
```

4. Wait for Deep Research to generate a research plan. Scroll to the bottom of the plan, and click **Start research**.

5. Note what is missing:
- unclear scope
- weak structure
- vague recommendation criteria
- inconsistent sourcing expectations

### Task 2: Use Meta Prompting to Build a Better Prompt

1. In a new chat, ask Gemini to generate a stronger Deep Research prompt before running research again. Copy and paste the following prompt:

```text
You are a prompt engineer helping Cymbal Capital Partners run Deep Research for investment due diligence.

Rewrite my weak prompt into one high-quality prompt for Gemini Enterprise Deep Research.

Weak prompt:
"Research potentially companies on behalf of Cymbal Capital Partners - a venture capital and private equity firm looking for its next investment opportunity - and tell me if it is a good investment."

Requirements for the improved prompt:
1. Define investor context (venture capital/private equity)
2. Require coverage of company background, founders, market viability, and risks
3. Require reliable sources and citation-aware claims
4. Force clear output sections with concise bullet points
5. Include a go/no-go preliminary recommendation plus top open diligence questions
6. Instruct the model to label uncertain claims as Unverified

Return only the improved Deep Research prompt.
```

2. Take a moment to read through the old and new prompts. What has changed?

### Task 3: Compare Outputs (Weak vs Meta-Prompted)

1. In the same chat, paste this comparison prompt:

```text
Compare the two Deep Research outputs:
1) weak baseline prompt I provided
2) meta-prompted improved prompt you generated

Score each from 1-5 on:
- Clarity of scope
- Quality of evidence
- Actionability for investors
- Transparency of uncertainty

Then provide:
1. Three concrete improvements from the meta-prompted version
2. One remaining weakness
3. A final one-sentence recommendation for Cymbal Capital Partners
```

2. What did Gemini Enterprise rate your original prompt? What about after it was engineered?

### Task 4: Run Deep Research with the Improved Prompt

1. Copy the improved prompt from Task 2.

2. Open a new chat and start a new Deep Research run using the improved prompt.

3. Review the plan and click **Start research**.

4. Observe the changes between this research result compared to the first run.

## When and Why to Use Meta Prompting

Use meta prompting when:
- the task is high-stakes (investment, compliance, legal, strategy)
- you need consistent structure across teams
- you need stronger evidence standards and explicit uncertainty
- the first prompt is broad, vague, or inconsistent

Benefits over a poorly written prompt:
- better research plans
- fewer missing sections and unsupported claims
- clearer decision-ready outputs
- easier quality review and team alignment

## Wrap-Up

In this lab, students:
- saw how a weak prompt limits Deep Research quality
- used meta prompting to generate a stronger prompt
- compared outputs side-by-side
- produced a clearer investment recommendation for Cymbal Capital Partners