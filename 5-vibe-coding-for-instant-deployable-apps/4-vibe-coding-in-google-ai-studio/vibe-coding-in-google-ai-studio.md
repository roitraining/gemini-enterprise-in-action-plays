# Vibe Coding in Google AI Studio

## Time Required
20-30 minutes

## Overview
In this lab, you'll ...

### You learn how to:
- ...

## Scenario

<p align="left">
  <img src="images/cymbal-logistics-logo-dark.png" width="50%" alt="Cymbal Logo" />
</p>

Cymbal Logistics is ...

This application will ...



## Lab Instructions

### Task 1: Create the Driver Log App
...

1. Open [Google AI Studio](https://aistudio.google.com/apps), and login.  If a video appears, click __Skip__.

2. Select the __Build__ menu on the left and then run the following prompt which describes your app. 

```text
Create a simple React application using Tailwind CSS called "Cymbal Driver Log". 
This is a basic tablet interface for a truck driver to log their shift details.

CRITICAL INSTRUCTION: Keep the UI extremely simple. Do not add mock data simulators, charts, side navigation bars, or any features not explicitly requested below. Build ONLY a static layout.

UI Requirements:
- Use a stacked layout centered on the screen optimized for a tablet. Make it responsive to different screen sizes and support Portrait and Landscape modes. 
- Theme: Light background with dark blue and slate accents. 
- Ensure all inputs and buttons are large and easy to tap.

Include EXACTLY these four sections, stacked vertically:
1. Header: A simple title that says "Cymbal Driver Log".
2. Shift Status: A row of three large, distinct buttons: "ON DUTY", "OFF DUTY", and "ON BREAK".
3. Trip Details: Two large input fields for "Current Odometer" and "Trailer ID".
4. Add a row of four buttons that verify they performed their safetly checklist (Fuel, Tire pressure, Engine Check, and Trailor Check)
5. Shift Notes: A single large text area for adding notes.
6. Add a Login link that simply asks the driver for their name and driver ID. (This is not a username and password, they are just identifying themselves.) Display this in the upper right corner. 

Stop here. Just build the visual layout.

```

> [!WARNING] 
> It will take a little while for your app to be generated. 

3. At one point, while the app is being built, you will be prompted to select a theme. Examine the choices and pick the one you like the best. 

> [!NOTE] 
> Your output should be similar to the following. 

IMAGE HERE

4. Click the __Code__ button at the top. Notice, this app is not being coded in a single file like in Gemini using Canvas. This program uses a proper structure for a ReactJS app using Typescript files, CSS, and an organized folder structure. 

5. Go back to __Preview__ and then click the __Fullscreen__ icon and explore the app. Try to make sense of the various features. 

6. Select the __Device__ button and choose __Tablet__. 

7. Exit fullscreen and click the __Edit tool__ icon. 

8. Enter the following prompt in the Chat and run it. 

```text
Now, let's make the app store shift history. 
- Use React 'useState' and 'useEffect' to ensure that all inputs: Current Date and Time, Driver Name, Driver ID, Odometer, Trailer ID, Safety Checklist, and Shift notes) are saved to 'localStorage'.
- When I refresh the page, the app should remember exactly what I entered and which status button was active.
- Add an "Add New Shift" button at the bottom that resets the form for a new day (shift). 
- Keep the history in Local storage, so the user can pull up past shifts. 
```

### Task 2: Add features to the Driver Log App
...

1. Ask AI Studio to add an "Export History". It should retrieve all the data from local storage, format it as CSV, and pop up a window where the user can copy it to their clipboard. 

2. Make sure you samve some shift data and test the export feature. 

3. Ask AI Studio to create a new tab in the application that allows the driver to log expenses. You can do this any way you like. It should be easy to add reciepts and expense information. They should also be able to export the expenses and easily be able to add them to an email or spreadsheet to be submitted. 

## Congratulations
In this lab, you have:
- ...