# Professional Lifestyle Photography

## Overview
This play teaches you how to create high-end lifestyle marketing assets that blend personal identity with corporate branding using Gemini’s Nano Banana 2 model. You will start with a simple prompt, critique the weak spots, and then refine the prompt in a structured way.


### Objectives
In this play, you learn how to:
- Start with a baseline image prompt and identify weaknesses.
- Add identity grounding and brand integration while keeping style details intentionally vague.
- Use a critique loop to improve prompt quality in a structured way.
- Compare before and after outputs to measure quality gains.
- Create a Version B variant that emphasizes positive subject emotion for ad-style storytelling.

## Instructions
### Part 1: Baseline Prompt (intentionally simple)
Goal: Start with a simple prompt to establish the baseline.

1. Open Gemini Enterprise in your browser.

2. Click `New chat` to start a fresh session.

3. In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.

4. In the chat, copy and paste this baseline prompt, then press ENTER:

```
A person working out in a gym for a company ad.
```

5. Review the image and discuss what is missing: identity fidelity, brand presence, realism, and composition.

---

### Part 2: Add Identity Grounding and Brand Placement
Goal: Add identity grounding and natural brand placement while keeping style details vague.

1. Click `New chat` to start a fresh session.

2. In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.

3. Select `+ Add files` and choose `Upload files`.

4. In the dialog, select `headshot.jpg` and `CymbalLogo.png`, then click `Open`.

5. In the chat, copy and paste this prompt, then press ENTER:

```
Create a realistic marketing image of a person exercising in a gym. Use headshot.jpg as the face reference so the subject looks like the same person. Integrate CymbalLogo.png naturally into the environment or gear so it feels physically part of the scene, not pasted on top.
```

6. Save this output image as your `Version A - initial` result.

---

### Part 3: Critique Loop and Prompt Augmentation
Goal: Critique the draft, then use the feedback to strengthen the prompt.

1. Download or save the image from Part 2 so you can upload it into a new chat.

2. Click `New chat` to start a fresh session.

3. Upload the Part 2 image and paste this critique loop prompt:

```
You are a creative director reviewing a marketing image draft.

Evaluate this image on a 1-5 scale for:
1) identity fidelity,
2) logo realism and integration,
3) lighting realism,
4) material and texture quality,
5) composition and ad readiness.

Then provide:
- The top 3 weaknesses
- Specific fix instructions for each weakness
- A revised image-generation prompt that preserves the original intent but addresses the weaknesses

Output format:
1) Scorecard table
2) Weaknesses and fixes
3) Revised prompt
```

4. Copy the `Revised prompt` from the critique output.

5. Click `New chat` to start a fresh session.

6. In the chat bar, choose `Generate images (NB2)`.

7. Upload `headshot.jpg` and `CymbalLogo.png` again.

8. Paste the revised prompt and press ENTER to generate an improved image.

9. Save this output as your `Version A - improved` result.

10. Compare `Version A - initial` and `Version A - improved` side by side and note the quality gains.

---

### Bonus: Version B Focused on Subject Emotion
Goal: Try a variation that emphasizes ad-style emotion.

1. Click `New chat` to start a fresh session.

2. Choose `Generate images (NB2)` and upload `headshot.jpg` and `CymbalLogo.png`.

3. Use this variation prompt to emphasize ad-style emotion:

```
Create a realistic, premium athletic marketing image using headshot.jpg as the subject identity. The subject should look genuinely happy, energized, and confident while working out. Keep CymbalLogo.png naturally integrated into gear or architecture. Maintain realism and avoid artificial overlays.
```

4. Generate and save as `Version B - emotion emphasis`.

5. Compare `Version A - improved` vs `Version B - emotion emphasis` and discuss when each style is better for campaign goals.

---