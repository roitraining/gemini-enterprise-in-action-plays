# Gemini Enterprise in Action Plays

This repository contains course and play materials for the Gemini Enterprise in Action half-day training series.

Each course is organized as its own folder. Inside each course, every play has a numbered folder with step-by-step instructions and a dedicated images directory.

## Repository Structure

- `0-course-template/`
	- Template for creating new courses and plays.
- `1-gemini-for-image-video-and-audio-analysis/`
- `2-gemini-enterprise-tools-workshop/`
- `3-streamlining-workflows-with-notebooklm/`
- `4-building-agents-for-gemini-enterprise/`
- `5-vibe-coding-for-instant-deployable-apps/`

Each course folder includes:
- `README.md` with a course overview and case study summary.
- One subfolder per play, prefixed by sequence number (for example: `1-ice-breaker/`).

Each play folder includes:
- `instructions.md` with the play walkthrough.
- `images/` for screenshots and supporting visuals referenced by `instructions.md`.

## Naming Conventions

- Use lowercase folder names.
- Replace spaces with dashes.
- Prefix courses and plays with their display order (`1-`, `2-`, etc.).
- Keep image filenames lowercase and dash-separated.

## Writing Guidelines

For each play's `instructions.md`, include:
- Clear heading and short overview.
- Numbered step-by-step instructions.
- Bulleted notes and sub-bullets when helpful.
- Prompt or command examples in fenced code blocks.
- Inline images stored in the local `images/` folder.

Example image reference:

```markdown
![Screen capture](images/sample-image.png)
```

## How to Add a New Course

1. Copy `0-course-template/`.
2. Rename the course folder with the next numeric prefix and course name.
3. Add a short course overview and case study summary to the course `README.md`.
4. Create numbered play folders.
5. Fill in each play's `instructions.md` and place assets in that play's `images/` folder.

