# Deep Research for Investment Due Diligence

## Time Required
20 minutes

## Overview
In this lab, you will use Gemini Enterprise Deep Research to investigate a company before making an investment decision.

You will learn how to start with a broad question, narrow the research to founders and company background, test market viability, and turn the results into a partner-ready recommendation.

### You learn how to:
- Frame a strong Deep Research request for investment due diligence.
- Ask follow-up questions that improve source quality and answer depth.
- Separate company background, founder credibility, and market viability into distinct research passes.
- Spot missing evidence, unsupported claims, and weak market signals.
- Turn research output into a concise investment note for Cymbal Capital Partners.

## Scenario

Cymbal Capital Partners is a fictional venture capital and private equity firm looking for the next big investment opportunity.

The team wants to evaluate a company's background, founders, and market viability before investing. Your job is to use Gemini Enterprise Deep Research to gather evidence, compare signals, and produce a clear recommendation for the investment committee.

## Lab Instructions

### Task 1: Start with a Broad Research Brief

Begin with a wide question so Deep Research can surface the company overview and the main evidence themes.

1. Open Gemini Enterprise and start a new chat.

2. From the **Tools** list, select **Deep Research**.

3. Paste this prompt:

```text
You are helping Cymbal Capital Partners, a venture capital and private equity firm looking for their next big investment opportunity, to evaluate companies for a potential investment.

Research the company's background and summarize the most important facts for an investor.

Return:
1. What the company does
2. Who the founders are and why they matter
3. What problem the company claims to solve
4. The top 3 signs the company could be investable
5. The top 3 reasons to be cautious
6. A one-sentence preliminary recommendation

Use reliable sources and cite where each claim comes from.
```

4. Wait for Deep Research to generate a research plan. Examine the plan when it is complete. You can ask Deep Research to modify the plan if it does not match your preferences.

5. Scroll to the bottom of the plan, and click **Start research**. Gemini will begin researching the future for you.

### Task 2: Focus on the Founders

Now narrow the research to the people behind the company.

1. Ask a follow-up prompt focused only on the founders:

```text
Now focus only on the founders and leadership teams of these companies.

Research their background, relevant experience, and any signals that affect investor confidence.

Return:
1. Founder bios in one or two sentences each
2. Relevant startup, industry, or domain experience
3. Any prior exits, failures, or leadership gaps that matter
4. Evidence of founder-market fit
5. One concern an investor should investigate further

Use only evidence you can support from reliable sources.
```

2. Check whether Deep Research distinguishes between strong evidence and speculation. Good output should name specific roles, dates, companies, or prior outcomes.

### Task 3: Test Market Viability

Shift from people to market opportunity.

1. Ask a market-focused follow-up:

```text
Research the market viability of this company.

Answer as an investor would.

Return:
1. The market problem and why it matters now
2. The size or direction of the opportunity
3. The most important competitors or alternatives
4. The company's likely differentiation
5. The biggest market risk
6. Whether the market appears attractive enough for venture or growth investment
```

2. Look for evidence that the response is based on concrete sources rather than high-level industry language.

### Task 4: Compare Signals and Spot Gaps

Use Deep Research to pressure-test the story instead of accepting the first answer.

1. Ask for a balanced diligence view:

```text
Compare the company's story, the founders' background, and the market evidence.

Separate the strongest support from the biggest gaps.

Return:
1. What the evidence supports strongly
2. What remains unverified
3. Where sources conflict or are incomplete
4. The 3 most important diligence questions for Cymbal Capital Partners
5. A concise go / no-go view
```

2. If the answer sounds overconfident, ask it to label uncertain claims explicitly as unverified.

### Task 5: Produce an Investment Summary

Now turn the research into an internal memo.

1. Ask Deep Research to synthesize the evidence into a short decision note:

```text
Prepare a short investment note for Cymbal Capital Partners using only the research gathered so far.

Write a memo with these sections:
- Title
- One-line summary
- Why it stands out
- Key risks
- Missing information
- Recommendation

Rules:
- Stay grounded in the research.
- Do not invent facts.
- Mark any uncertain claims as Unverified.
- Keep it concise and decision-oriented.
```

2. Review whether the memo is useful for an investment committee. The best version should make the decision easier, not just repeat the research.

### Task 6: Refine for Better Investment Judgment

Use one final prompt to improve the quality of the decision.

1. Ask Deep Research to pressure-test the recommendation one more time:

```text
Before finalizing the investment view, challenge your own recommendation.

List:
1. The strongest reason to invest
2. The strongest reason not to invest
3. One fact that would most change the decision
4. The most important next step for diligence
```

2. Discuss how the answer changes when the model is forced to weigh the evidence against itself.

## Wrap-Up

In this lab, you have:
- Used Gemini Enterprise Deep Research to investigate a company's background.
- Evaluated the founders' credibility and founder-market fit.
- Tested whether the market is attractive enough to support investment.
- Turned research into a concise partner-facing recommendation.