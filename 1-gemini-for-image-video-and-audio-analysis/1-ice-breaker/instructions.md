# Nano Banana - Building a Professional Image: From Concept to Creation

## Overview
This play teaches you how to leverage Gemini’s Nano Banana 2 model for sophisticated image generation within the fictitious corporate ecosystem of Cymbal-Mart. We'll start simple and progressively enhance our prompts to achieve a high-fidelity, professional marketing asset.

### Objectives
In this play, you will learn how to:
- Generate images from basic text prompts.
- Incorporate an input image (like a personal headshot) to guide identity in image generation.
- Develop advanced "meta-prompts" to engineer detailed and context-aware image generation requests.
- Combine branding elements and personal identity to create professional digital assets.

## Instructions

---

### Part 1: The Basic Concept
Let's start with a very simple idea to see how Gemini interprets minimal instructions.

1.  Open Gemini Enterprise in your browser.
2.  In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.
3.  In the chat, copy and paste the following simple prompt, then press ENTER.
    ```text
    A person in a warehouse.
    ```
4.  Observe the generated image. Notice its generic nature and how Gemini fills in the details without specific guidance. This is our baseline.

---

### Part 2: Introducing Identity
Now, let's try to guide the model with a specific identity using a headshot.

1.  Click `New chat` to open a fresh session.
2.  In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.
3.  Select `+ Add files` and choose `Upload files`.
4.  In the dialog, select `headshot.jpg` (located in the `data` folder) and click `Open`.
5.  In the chat, copy and paste the following prompt, then press ENTER.
    ```text
    Using the face from the headshot.jpg, place it onto the body of a worker in a warehouse.
    ```
6.  Compare this new image to the one from Part 1. You should see Gemini attempting to incorporate the facial features from your headshot, but the overall scene might still lack detail and corporate branding.

---

### Part 3: Engineering the Professional Image
To achieve a high-quality, professional marketing asset, we need to provide Gemini with very detailed instructions. This is where "prompt engineering" comes in. We'll even use a "meta-prompt" to help us craft the perfect prompt.

1.  Click `New chat` to open a fresh session.
2.  In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.
3.  Select `+ Add files` and choose `Upload files`.
4.  In the dialog, select `headshot.jpg` and `CymbalLogo.png` (both located in the `data` folder) and click `Open`.
5.  In the chat, copy and paste the following **meta-prompt**, then press ENTER. This prompt asks Gemini to *generate* a detailed image generation prompt for us.
    ```
    I want to create a professional corporate branding image for my company, Cymbal-Mart, that feels authentic and industrious. Please write a perfectly engineered image generation prompt for me. The scene needs to feature a worker (based on a headshot called headshot.jpg) in an industrial warehouse setting, and my company logo (CymbalLogo.png), but they must be integrated naturally into the environment. Make sure the logo appears as a realistic detail on the worker's gear or the architecture.
    ```
6.  Gemini will respond with a highly detailed image generation prompt. Click the Copy response icon at the end of the generated response.
    *Note: You may also copy the following example prompt that we’ve generated for you:*
    ```
    Photorealistic corporate image of a worker in an industrial warehouse (use [headshot.jpg] as the face reference). The worker wears a high-visibility vest and safety gear. Naturally integrate the logo [CymbalLogo.png] as an embroidered patch on the worker's vest and as a painted graphic on a background shipping container. Authentic, industrious atmosphere, cinematic warehouse lighting, shot on 50mm lens.
    ```
7.  In the chat, paste the detailed prompt you copied (or the example prompt above), then press ENTER.

8.  Save your final, high-fidelity result for sharing. Reflect on the difference between this image and the ones from Part 1 and Part 2. The level of detail and specificity in the prompt directly led to this professional output.

### Bonus: Adding Prompt Engineering
Part 3 already gives a strong result. As a best practice, you can do one extra pass to make the prompt more structured and consistent.

1. Click New chat to open a fresh session.

2. Copy and paste the following prompt into Gemini:
```
Engineer this image prompt to include Persona, Role, Steps, and Output format while keeping the same intent and details:
"Photorealistic corporate image of a worker in an industrial warehouse (use [headshot.jpg] as the face reference). The worker wears a high-visibility vest and safety gear. Naturally integrate the logo [CymbalLogo.png] as an embroidered patch on the worker's vest and as a painted graphic on a background shipping container. Authentic, industrious atmosphere, cinematic warehouse lighting, shot on 50mm lens."
```

3. Click the Copy response icon at the end of the generated response. You may also copy the following example prompt that we’ve generated for you:

```
Persona: You are a world-class commercial photographer and digital artist specializing in hyper-realistic corporate and industrial imagery.

Role: Your role is to art direct and generate a photorealistic corporate promotional image that seamlessly blends specific subject references and brand assets into a cinematic, authentic scene.

Steps:

Subject Generation: Create a central figure of a worker stationed in an industrial warehouse. Use the provided image [headshot.jpg] as the strict face reference to maintain the exact likeness of the subject.

Wardrobe & Gear: Dress the worker in realistic, industry-standard safety gear, prominently featuring a high-visibility vest.

Brand Integration (Foreground): Naturally and seamlessly integrate the provided logo [CymbalLogo.png] as a highly detailed, textured embroidered patch on the worker's high-visibility vest.

Environment & Setting: Design the background to depict an authentic, industrious warehouse environment.

Brand Integration (Background): Incorporate the [CymbalLogo.png] a second time as a realistic, slightly weathered painted graphic on a large shipping container in the background.

Lighting & Composition: Light the scene using cinematic warehouse lighting (e.g., dynamic shadows, dramatic industrial overhead lights) to establish an authentic, industrious atmosphere.

Output Format: A single, high-resolution photorealistic image rendered to perfectly mimic the depth of field, perspective, and optical qualities of a photograph shot on a professional 50mm lens.
```

4. Notice that the prompt now has distinct sections. This helps the model follow your instructions more reliably. Now let's test it. Click `New chat` to open a fresh session.

5. In the chat bar, select the Tools icon and then choose `Generate images (NB2)`.

6. Select `+ Add files` and choose `Upload files`. Select `headshot.jpg` and `CymbalLogo.png`, then click `Open`.

7. In the chat, paste the engineered prompt you copied, then press ENTER.
