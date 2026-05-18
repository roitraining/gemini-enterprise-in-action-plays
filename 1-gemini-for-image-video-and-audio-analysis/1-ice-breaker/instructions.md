# Nano Banana - Building a Professional Image: From Concept to Creation

## Overview
This play teaches you how to use Gemini’s Nano Banana 2 model to create professional corporate imagery for Cymbal-Mart. You will start with a simple prompt, then add identity and brand references, and finish by engineering a structured meta-prompt for a higher-fidelity result.

### Objectives
In this play, you will learn how to:
- Generate images from basic text prompts.
- Incorporate an input image, such as a headshot, to guide identity in image generation.
- Develop advanced meta-prompts to engineer detailed and context-aware image generation requests.
- Combine branding elements and personal identity to create professional digital assets.

## Instructions

---

### Part 1: Baseline Image
Goal: Establish a simple baseline and see how Gemini interprets minimal instructions.

1. Open Gemini Enterprise in your browser.
2. In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.
3. In the chat, copy and paste the following simple prompt, then press ENTER.
    ```text
    A person in a warehouse.
    ```
4. Review the generated image. Notice its generic nature and how Gemini fills in the details without specific guidance. This is our baseline.

---

### Part 2: Add Identity
Goal: Guide the model with a specific identity using a headshot.

1. Click `New chat` to start a fresh session.
2. In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.
3. Select `+ Add files` and choose `Upload files`.
4. In the dialog, select `headshot.jpg` (located in the `data` folder) and click `Open`.
5. In the chat, copy and paste the following prompt, then press ENTER.
    ```text
    Using the face from the headshot.jpg, place it onto the body of a worker in a warehouse.
    ```
6. Compare this new image to the one from Part 1. You should see Gemini attempting to incorporate the facial features from your headshot, but the overall scene may still lack detail and corporate branding.

---

### Part 3: Engineer the Professional Image
Goal: Provide Gemini with detailed instructions to produce a high-quality, professional marketing asset.

1. Click `New chat` to start a fresh session.

2. In the chat, copy and paste the following meta-prompt, then press ENTER. This prompt asks Gemini to generate a detailed image-generation prompt.
    ```
    I want to create a professional corporate branding image for my company, Cymbal-Mart, that feels authentic and industrious. Please write a perfectly engineered image generation prompt for me. The scene needs to feature a worker (based on a headshot called headshot.jpg) in an industrial warehouse setting, and my company logo (CymbalLogo.png), but they must be integrated naturally into the environment. Make sure the logo appears as a realistic detail on the worker's gear or the architecture.
    ```
3. Gemini will respond with a highly detailed image-generation prompt. Click the Copy response icon at the end of the generated response.

    *Note: You may also copy the following example prompt that we’ve generated for you:*

    ```
    Photorealistic portrait of an industrial worker \[insert headshot.jpg\] standing confidently in a busy, modern warehouse. The worker wears professional safety gear featuring the company logo \[insert CymbalLogo.png\] naturally integrated onto the hard hat or safety vest. Cinematic lighting, authentic industrious atmosphere, shot on an 85mm lens for corporate branding.
    ```

4. In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.

5. Select `+ Add files` and choose `Upload files`.

6. In the dialog, select `headshot.jpg` and `CymbalLogo.png` (both located in the `data` folder) and click `Open`.

7. In the chat, paste the detailed prompt you copied (or the example prompt above), then press ENTER.

8. Reflect on the difference between this image and the ones from Part 1 and Part 2. The level of detail and specificity in the prompt directly led to this professional output.


### Bonus: Structure the Prompt
Part 3 already gives a strong result, but as a best practice, we can do one extra pass to make the prompt more structured and consistent.

1. Click `New chat` to start a fresh session.

2. Copy and paste the following prompt into Gemini:
```
Engineer this image prompt to include Persona, Role, Steps, and Output format while keeping the same intent and details:
"Photorealistic portrait of an industrial worker \[insert headshot.jpg\] standing confidently in a busy, modern warehouse. The worker wears professional safety gear featuring the company logo \[insert CymbalLogo.png\] naturally integrated onto the hard hat or safety vest. Cinematic lighting, authentic industrious atmosphere, shot on an 85mm lens for corporate branding."
```

3. Click the Copy response icon at the end of the generated response. You may also copy the following example prompt that we’ve generated for you:

```
Persona: You are an expert Commercial Photographer and Brand Strategist specializing in corporate identity.

Role: Your goal is to produce a signature "hero image" for a professional training course. This image must blend the authentic appearance of an industrial worker with the high-tech, polished aesthetic of the Cymbal brand (Google’s demo holding company).

Steps:
Likeness Integration: Carefully adapt the facial features and professional expression from headshot.jpg to the central subject of the image.
Environment Design: Position the subject in a "busy, modern warehouse" that features clean lines, organized racking, and hints of automation/robotics to signify a cutting-edge facility.
Apparel & Branding: Dress the worker in high-quality, ANSI-compliant professional safety gear. Naturally integrate the CymbalLogo.png onto the left chest of the safety vest or the front center of the hard hat, ensuring the logo texture matches the fabric/plastic material perfectly.
Cinematic Treatment: Apply a "corporate branding" lighting scheme—soft key light on the face, cold industrial rim lighting from the warehouse background, and a warm, industrious atmosphere.
Optical Specifications: Simulate a shot on an 85mm prime lens with a wide aperture (f/1.8 to f/2.8) to create a shallow depth of field, keeping the subject sharp while the warehouse background falls into a creamy, professional bokeh.

Output Format:
Medium: Photorealistic Corporate Photography.
Resolution: 8K, highly detailed textures.
Tone: Confident, innovative, and reliable. 
Visual Priority: Subject's face and the Cymbal logo must be the primary focal points.
```

4. Notice that the prompt now has distinct sections. This helps the model follow your instructions more reliably. Now let's test it. 

5. Click `New chat` to open a fresh session.

6. In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.

7. Select `+ Add files` and choose `Upload files`. Select `headshot.jpg` and `CymbalLogo.png`, then click `Open`.

8. In the chat, paste the engineered prompt you copied, then press ENTER.
