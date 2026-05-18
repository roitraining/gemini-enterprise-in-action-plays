# Store Safety Compliance

## Overview
This play teaches you how to leverage Gemini’s multimodal reasoning to conduct an automated, high-precision safety audit using raw video footage of a store walk-through. 

### Objectives
In this play, you learn how to:
- to transform unstructured video data into an actionable, timestamped compliance report.
- bridge the gap between static corporate policy and real-time operational oversight to ensure a safer, more efficient retail ecosystem.


## Instructions
1. Open Gemini Enterprise in your browser.

2. Click the + Add files icon and select Upload files. 

3. In the dialog, select store.mp4 and Cymbal-Mart_VisualMerchandising_and_Store_Standards.pdf and click Open.

4. In the chat, copy and paste the following prompt, then press ENTER.

```
Role: You are the Primary Safety Manager for Cymbal-Mart, conducting a high-stakes virtual safety audit.
Task: Analyze the provided store walk-through video. Your objective is to identify every instance of non-compliance based strictly on the "Cymbal-Mart Visual Merchandising and Store Standards" document.
Instructions: Cross-Reference: For every hazard identified, cite the specific section of the Cymbal-Mart Standards document (e.g., "Violation of Section 3: Vertical Stacking").  Evidence: Provide the exact timestamp from the video where the violation occurs.
Output Format: Create an Audit Log: A chronological list of violations with [Timestamp], [Violation Category], and [Description of Hazard], and a Critical Risk Summary: A concluding section highlighting the top 3 most dangerous hazards that require immediate intervention (e.g., life-safety or fire code violations). Finally, make Operational Recommendations: Brief suggestions for the Store Manager to prevent recurrence.
```

5. Save your final result for sharing.