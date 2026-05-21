# Creating Multi-Agent Systems

## Time Required
30–40 minutes

## Overview
In this lab, you will use the Agent Designer flow builder to build a multi-agent system. You will create a root Orchestrator Agent and four specialized sub-agents, each responsible for a distinct part of the new employee onboarding process. The Orchestrator delegates to all four simultaneously and assembles their outputs into a single, unified summary.

### You learn how to:
- Design a multi-agent system with a root orchestrator and specialized sub-agents.
- Add and configure sub-agents in the flow builder.
- Write routing logic that delegates tasks to the right agent.
- Test a multi-agent flow end to end with realistic input.

## Scenario

<p align="left">
  <img src="images/cymbal-insurance-logo.png" width="50%" alt="Cymbal Insurance Logo" />
</p>

Every time a new employee joins Cymbal Insurance, the same process plays out across four separate departments: IT sets up equipment and system access, HR sends paperwork and a welcome email, Facilities assigns a badge and workspace, and Training schedules the first week of orientation. Today, each team learns about a new hire independently — often late. The result is a fragmented onboarding experience where equipment isn't ready, badges aren't printed, and new employees spend their first day waiting.

In this lab, you will build a single Orchestrator Agent that takes new hire details and coordinates all four departments in one step.

## Lab Instructions

### Task 1: Create the Orchestrator Agent

1. Open your Gemini Enterprise web app and click **+ Create agent** in the navigation menu.

2. On the Agent Designer page, click **Proceed to builder**.

3. The **Flow** tab opens with a default agent node. Click the node to open its configuration panel. Configure the Orchestrator:
   - **Name:** `New Hire Onboarding Orchestrator`
   - **Description:** `Coordinates new employee onboarding by delegating tasks to IT, HR, Facilities, and Training sub-agents simultaneously.`
   - **Instructions:** Paste the following:

   ```text
   You are the New Hire Onboarding Orchestrator for Cymbal Insurance.

   When you receive new employee details, do the following:

   1. Confirm you have all five required fields: full name, start date, role, department, and office location. If any are missing, ask for them before proceeding.

   2. Once you have all required information, delegate onboarding tasks to ALL FOUR sub-agents simultaneously:
      - IT Provisioner: hardware, software, and system access setup
      - HR Assistant: welcome email to the employee and internal HR checklist
      - Facilities Agent: building access badge, parking, and workspace assignment
      - Training Coordinator: structured first-week onboarding schedule

   3. Collect all four sub-agent outputs and present them as a single "New Hire Onboarding Summary" with a clearly labeled section for each department.

   Do not skip any sub-agent, even if details about a particular department were not explicitly requested.
   ```

   - **Model:** Leave the default model selected.

4. Do not click **Create** yet — you need to add the sub-agents before launching.

   > [!IMPORTANT]
   > If you exit the Agent Designer at this point, your agent will be saved as a **Draft**. You can reopen it from **Agent Gallery > Your agents** and continue from where you left off.

### Task 2: Add the IT Provisioner and HR Assistant

1. In the **Flow** tab, hover over the **New Hire Onboarding Orchestrator** node. A **+ Add subagent** button appears. Click it.

   <p align="left">
     <img src="images/add-subagent.png" width="70%" alt="Flow tab showing the Add subagent button" />
     <br><em>Hover over the Orchestrator node to reveal the + Add subagent button</em>
   </p>

2. A new sub-agent node appears on the canvas. Click the node and configure it:
   - **Name:** `IT Provisioner`
   - **Description:** `Drafts an IT setup request for new employee hardware and system access.`
   - **Instructions:** Paste the following:

   ```text
   You are the IT Provisioner sub-agent for Cymbal Insurance's onboarding system.

   You receive new hire details from the Orchestrator. Draft a professional email to the IT department to set up the new employee's equipment and system access.

   The email must include:
   - Subject line: "New Hire IT Setup Request — [Full Name], Start Date: [Date]"
   - Hardware: standard laptop and accessories (request high-performance setup if the role is in Engineering, Data Science, or Analytics)
   - Software: standard productivity suite, corporate email account, VPN client, and any role-specific applications
   - System access: Active Directory account creation, network access, and shared drives appropriate for the department
   - Priority: flag as URGENT if the start date is within 5 business days

   Keep the tone direct and professional.
   ```

3. In the **Flow** tab, hover over the Orchestrator node again and click **+ Add subagent** to add a second sub-agent. Configure it:
   - **Name:** `HR Assistant`
   - **Description:** `Drafts a welcome email to the new employee and an internal HR pre-start checklist.`
   - **Instructions:** Paste the following:

   ```text
   You are the HR Assistant sub-agent for Cymbal Insurance's onboarding system.

   You receive new hire details from the Orchestrator. Produce two items:

   1. Welcome Email to the new employee:
      - Warmly welcome them to Cymbal Insurance by name
      - Confirm their start date, office location, and first-day arrival time (9:00 AM unless otherwise noted)
      - Let them know their manager will be in touch shortly with first-week details
      - Professional but warm tone

   2. Internal HR Checklist email to the HR team:
      - Subject: "New Hire Pre-Start Checklist — [Full Name], Starting [Date]"
      - Items: offer letter confirmation on file, benefits enrollment packet to send, I-9 documentation to collect, direct deposit form, employee badge request submitted to Facilities
      - Flag any items that must be completed before the start date
   ```

4. The **Flow** tab should now show the Orchestrator connected to two sub-agents.

   <p align="left">
     <img src="images/flow-two-subagents.png" width="70%" alt="Flow tab with Orchestrator connected to IT Provisioner and HR Assistant" />
     <br><em>The flow after adding IT Provisioner and HR Assistant sub-agents</em>
   </p>

### Task 3: Add the Facilities Agent and Training Coordinator, Then Test

1. Hover over the Orchestrator node and click **+ Add subagent** to add the third sub-agent:
   - **Name:** `Facilities Agent`
   - **Description:** `Requests building access, parking, and workspace assignment for the new employee.`
   - **Instructions:** Paste the following:

   ```text
   You are the Facilities Agent sub-agent for Cymbal Insurance's onboarding system.

   You receive new hire details from the Orchestrator. Draft an email to the Facilities team.

   The email must include:
   - Subject: "New Hire Facilities Setup — [Full Name], Start Date: [Date]"
   - Building access badge request for the employee's primary office location
   - Parking: confirm availability and provide instructions for the parking registration process
   - Workspace: assign a standard desk in the employee's department area; note any special requirements (standing desk, accessibility accommodations) if mentioned in the new hire details
   - Flag as URGENT if the start date is within 5 business days
   ```

2. Hover over the Orchestrator node and click **+ Add subagent** one final time to add the fourth sub-agent:
   - **Name:** `Training Coordinator`
   - **Description:** `Creates a structured first-week onboarding schedule for the new employee.`
   - **Instructions:** Paste the following:

   ```text
   You are the Training Coordinator sub-agent for Cymbal Insurance's onboarding system.

   You receive new hire details from the Orchestrator. Produce two items:

   1. First-Week Onboarding Schedule for the new employee:
      - Day 1: Company orientation, IT setup walkthrough, HR paperwork and benefits overview
      - Day 2: Department introduction and team meet-and-greet
      - Day 3: Role-specific systems and tools training
      - Day 4: Compliance training — code of conduct, data privacy policy, and security awareness
      - Day 5: Shadowing session with a senior team member, followed by end-of-week check-in with manager
      Format the schedule with clear day-by-day headings.

   2. A brief welcome note to the new employee explaining the purpose of the schedule and what to bring on Day 1.
   ```

3. The **Flow** tab should now show all four sub-agents connected to the Orchestrator.

   <p align="left">
     <img src="images/flow-complete.png" width="70%" alt="Complete flow diagram with Orchestrator and all four sub-agents" />
     <br><em>The complete multi-agent system: Orchestrator with IT, HR, Facilities, and Training sub-agents</em>
   </p>

4. Click the **Preview** tab. Test the full system with the following new hire details:

   ```text
   New hire details:
   - Full Name: Maria Santos
   - Start Date: June 2, 2025
   - Role: Claims Analyst
   - Department: Property Claims
   - Office Location: Austin, TX
   ```

5. Verify that the Onboarding Summary contains all four sections and that each is appropriate for Maria's role:
   - **IT:** Does it request the right hardware and software for a Claims Analyst? Is it flagged URGENT if June 2 is within 5 business days?
   - **HR:** Does the welcome email address Maria by name and confirm her start details? Does the checklist cover all five items?
   - **Facilities:** Does it include badge access, parking, and workspace for the Austin office?
   - **Training:** Does the schedule follow the five-day structure? Is the welcome note addressed to Maria?

6. If any sub-agent's output is weak or missing, click the **Flow** tab, select that sub-agent's node, and refine its instructions.

7. When all four sections are working correctly, click **Create** to launch the system.

### Bonus Task 4: Test Complex Scenarios

A well-built multi-agent system handles edge cases gracefully. Try the following to push the system further.

1. Test with a new hire who has special requirements and an urgent start date. Use a start date that is 3 business days from today:

   ```text
   New hire details:
   - Full Name: David Kim
   - Start Date: [3 business days from today]
   - Role: Senior Data Engineer
   - Department: Analytics & Data Science
   - Office Location: New York, NY
   - Special requirements: standing desk, high-performance laptop
   ```

2. Verify that the IT Provisioner flags the request as URGENT and requests a high-performance setup.

3. Verify that the Facilities Agent includes the standing desk request.

4. Now test what happens with incomplete input — submit just a name and start date, with no role, department, or location:

   ```text
   I need to onboard Alex Rivera starting March 10.
   ```

   The Orchestrator should ask for the missing required fields before proceeding rather than sending incomplete requests to the sub-agents.

5. Provide the missing fields and confirm the system completes the full onboarding summary correctly.

## Congratulations

In this lab, you have:
- Designed a multi-agent system with a root orchestrator and four specialized sub-agents.
- Added and configured sub-agents using the flow builder.
- Written routing logic that delegates tasks to the right agent simultaneously.
- Tested a multi-agent flow end to end with realistic and edge-case input.
