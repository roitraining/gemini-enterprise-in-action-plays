# Video and Audio Generation

## Time Required
30–40 minutes

## Overview
In this lab, you will use Gemini to generate a short holiday social media video clip for Cymbal-Mart, complete with a synchronized voiceover script. You will then use Google AI Studio to generate an audio track from the script. The result is a complete, production-ready promotional asset built entirely with AI tools.

### You learn how to:
- Generate a short video clip with Gemini's video creation tool.
- Write a synchronized promotional script timed to match the video.
- Use Google AI Studio to generate an audio track from the script.

## Scenario

<p align="left">
  <img src="images/cymbal-mart-logo.png" width="50%" alt="Cymbal-Mart Logo" />
</p>

Cymbal-Mart's Social Media team needs a **10-second holiday ad** for Instagram and TikTok. The brief: a family discovering new holiday gift ideas in-store, festive and cinematic, with the Cymbal-Mart logo appearing naturally in the environment. The team also needs a punchy voiceover script that matches the visual energy. Budget: zero production hours — it all needs to be AI-generated.

## Lab Instructions

### Task 1: Generate the Video Clip

> [!IMPORTANT]
> Video generation uses **Gemini** (gemini.google.com), not Gemini Enterprise. Make sure you are in the correct product before starting.

1. Open **Gemini** in your browser (gemini.google.com).

2. In the chat bar, select the **Tools** icon and choose **Create video**.

   <p align="left">
     <img src="images/create_video.png" width="55%" alt="Create video tool in Gemini" />
     <br><em>Select Create video from the Tools menu</em>
   </p>

3. Click **+ Add files** → **Upload files**. If prompted, click **Agree**. In the dialog, select `CymbalLogo.png` and click **Open**.

4. Copy and paste the following prompt into the chat, then press **Enter**:

   ```text
   You are a creative director producing a holiday social media ad for Cymbal-Mart, a modern omnichannel retailer.

   Generate a 10-second cinematic video clip with the following specifications:

   Visual: A young family — two parents and two children — moving excitedly through a festive Cymbal-Mart store. The children discover a display of holiday gifts and light up with excitement. The parents exchange a warm, knowing look. The Cymbal-Mart logo (from the uploaded file) appears naturally on shopping bags in the family's hands and on digital signage in the background.

   Style: Warm, festive lighting with a shallow depth of field. Slow push-in camera movement. Brand colors are blue and silver. The feel is smart, modern, and emotionally warm — not kitschy.

   The video should feel like a 10-second cut from a premium TV commercial.
   ```

5. Review the generated video. Save the clip.

### Task 2: Write the Voiceover Script

The video needs a voiceover that fits the 10-second runtime precisely.

1. In a new Gemini chat (Gemini Enterprise is fine for this task), ask Gemini to write the script:

   ```text
   Write a 10-second voiceover script for a Cymbal-Mart holiday TV commercial. The tone should be smart, warm, and festive — not cheesy. The script must:
   - Open with a line that captures family excitement
   - Include a brief product or value mention (e.g., "thousands of gifts, all in one place")
   - End with the Cymbal-Mart tagline: "More for everyone."
   - Time out to exactly 10 seconds when read at a natural pace

   After the script, provide a word count and an estimated reading time in seconds.
   ```

2. Review the output and refine if needed. Ask Gemini to make it shorter, punchier, or more specific to holiday gifting if the first version isn't quite right.

### Task 3: Generate the Audio Track

1. Open **Google AI Studio** (aistudio.google.com) in a new tab.

2. Start a new prompt. Set the output type to **Audio** (if available in your account) or use the Text-to-Speech capability.

3. Paste the voiceover script and prompt AI Studio to generate the audio:

   ```text
   Generate a warm, upbeat voiceover recording of the following holiday ad script. The voice should be friendly and energetic — think network TV commercial narrator. Pace it to fit within 10 seconds.

   [Paste your finalized script here]
   ```

4. Download the audio file.

   > [!NOTE]
   > Text-to-speech audio generation features may vary depending on your Google AI Studio access tier. If this feature is not available in your account, record yourself reading the script aloud and use that as your audio track instead.

### Bonus Task 4: Assemble the Full Ad Concept

1. You now have three AI-generated components: the video clip, the voiceover script, and the audio track. Bring them together into a brief **creative brief document** that describes:
   - The target platform (Instagram Reels, TikTok, YouTube Shorts)
   - The video description and what it shows
   - The voiceover script with timestamp markers
   - Notes on how the audio and video are synchronized

2. Share the video, script, and brief with the group. Discuss: what would a human creative team need to do to take these AI-generated assets to a final, publishable state?

## Congratulations

In this lab, you have:
- Generated a branded holiday video clip using Gemini's video creation tool.
- Written a synchronized 10-second voiceover script timed to the video.
- Generated an audio track from the script using Google AI Studio.
- Assembled the components into a complete AI-generated promotional asset concept.

