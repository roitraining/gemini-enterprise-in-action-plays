# Managing Files as Context

## Time Required
20 minutes

## Overview
In this lab, you will use Gemini Enterprise's Manage files feature to turn scattered source material into useful context for prompts.

You will attach files from different sources, compare how file type affects the answer, and learn how to update the attached file set when you want the model to focus on different evidence.

### You learn how to:
- Add files from your computer and other connected sources to Gemini Enterprise.
- Work with multiple file types, including PDFs, spreadsheets, documents, text files, and images.
- Ask questions that force Gemini to ground its answer in attached files.
- Compare how answers change when you add, remove, or replace context files.
- Build a cleaner, decision-ready response for a Cymbal Capital Partners investment workflow.

## Scenario

Cymbal Capital Partners is a fictional venture capital and private equity firm evaluating a new investment opportunity.

The team has collected a deal memo, traction metrics, customer notes, and product visuals in different file types and from different sources. Your job is to use Gemini Enterprise to manage those files as context so the model can summarize the opportunity, compare signals, and produce a partner-ready recommendation.

## Lab Instructions

### Task 1: Start with One File

Begin with a single source so you can see how much context Gemini gets from one attachment.

1. Open Gemini Enterprise and start a new chat.

2. Click **+ Add files**.

3. Use **Upload files** to attach `cymbal-alpha-deal-memo.pdf` from your computer.

4. Ask Gemini to summarize the opportunity using only that file:

```text
You are supporting Cymbal Capital Partners.

Summarize the attached deal memo for a partner meeting.
Use only facts from the file.
Return:
1. What the company does
2. Why it could be attractive
3. The biggest risk
4. A one-sentence recommendation
```

5. If the answer is too generic, ask a follow-up question that forces a tighter summary.

### Task 2: Add a Second File Type

Now add a different type of evidence so Gemini can combine narrative and numbers.

1. Keep the same chat open.

2. Click **+ Add files** again.

3. Upload `traction-metrics.xlsx` from your computer.

4. Ask Gemini to compare the two files:

```text
Use the attached deal memo and traction metrics spreadsheet.

Compare the story in the memo with the operating signals in the spreadsheet.

Return:
1. Where the two files agree
2. Where the spreadsheet raises questions or supports the memo
3. Any metrics that look especially strong or weak
4. Two diligence questions for the investment team
```

5. Review whether Gemini uses the spreadsheet as evidence. It should cite specific rows, columns, or metric names from the spreadsheet.

### Task 3: Add a File from Another Source

Use a third source to show that Manage files can combine material across multiple upload.

1. Attach the file `customer-interview-notes.docx`. Ask Gemini to identify customer signals:

```text
Use the attached deal memo, traction spreadsheet, and customer interview notes.

Identify the strongest customer evidence for or against the investment.

Return:
1. Positive customer signals
2. Negative customer signals
3. Any contradictions across the files
4. The single most important follow-up question for a partner discussion
```

2. Notice that the extra file source gives Gemini more complete context or introduces noise.

### Task 4: Use an Image as Context

Now add a visual file so Gemini has to interpret a different format.

1. Click **+ Add files** and upload `product-infographic.png`

2. Ask Gemini to read the image together with the written material:

```text
Use the attached files, including the product infographic.

Based on the memo, metrics, notes, and the infographic, explain whether the product looks real, differentiated, and ready for customers.

Return:
1. What the image appears to show
2. Whether it supports the company story
3. Any concerns about product maturity or positioning
4. A concise investment view
```

3. Check whether Gemini describes only what is visible and avoids inventing details from the image.

4. If the response is vague, ask it to separate visual evidence from written evidence.


### Task 5: Manage the File Set Deliberately

A key part of Manage files is knowing when to reduce context, not just add more. In this step you'll run a focused cleaning prompt that removes noisy evidence and returns a compact, evidence-backed synthesis.

1. In the same chat, run the following prompt exactly to clean the files previosly uploaded ( `cymbal-alpha-deal-memo.pdf`, `traction-metrics.xlsx`, `customer-interview-notes.docx`, and `product-infographic.png`):

```text
You are an investment analyst for Cymbal Capital Partners. Use ONLY the attached files and do not browse external sources or invent facts.

Task — Clean & Synthesize:
1. Identify and remove noisy or unreliable data across these files (unsupported claims, contradictions, undated items, unexplained outliers, or unclear provenance). For each removed item list: file, precise location (PDF page/paragraph, spreadsheet sheet+row/cell, docx paragraph, image area), and a one-line reason for removal.
2. Using the remaining reliable evidence, produce a concise synthesis (max 250 words) with:
   - Investment thesis (one sentence)
   - Top 3 supporting facts (each with file citation and location)
   - Top 3 risks (each with file citation and location)
   - Two missing data points that materially affect the decision
   - One-line recommendation: `Proceed to diligence` / `Hold` / `No` and a one-line rationale
3. Appendix: list exact spreadsheet cells/sheets used, PDF pages and paragraph ranges used, and docx paragraph excerpts used.

Output headings: Investment Thesis, Supporting Facts, Risks, Missing Data, Recommendation, Appendix, Removed Items.
Begin by listing the number of removed items and the number of retained evidence items, then deliver the synthesis and appendix.
```

2. Review the cleaned synthesis. Compare this cleaned view with earlier, noisier answers from Tasks 1–4. Ask a follow-up if something looks incorrectly removed or still noisy.

### Task 6: Produce a Final Investment Note

Use the cleaned evidence to create a tight partner-ready memo.

1. Now that the cleaning step produced a short evidence appendix, run the following prompt to produce a final memo:

```text
You are preparing a partner note for Cymbal Capital Partners.

Using only the cleaned evidence (attached files taking into account the items removed and evidence items retained), write a short investment memo (max 300 words) with these sections:
- Title
- One-line Summary
- Why it stands out (3 bullets, each citing file+location)
- Key risks (3 bullets, each citing file+location)
- Missing information (2 bullets)
- Recommendation (one line: `Proceed to diligence` / `Hold` / `No` and one-line rationale)

Rules:
- Stay grounded in the provided files.
- Do not invent missing facts.
- Mark any uncertain claims `Unverified` and explain why in one line.
- Keep language concise and decision-oriented.
```

2. Review the memo for clarity and evidence linkage. You can save the final memo to share it by clicking the **Download responce** button.

## Congratulations

In this lab, you have:
- Added contextual files (PDF, spreadsheet, DOCX, image) to Gemini Enterprise.
- Cleansed unsupported, contradictory, or undated items and documented removed evidence.
- Created a concise, evidence-backed investment thesis and partner-ready memo  with supporting facts and risks.