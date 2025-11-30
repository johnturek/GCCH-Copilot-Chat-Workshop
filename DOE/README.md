# Department of Education Copilot Chat Hands-On Workshop: Proctor Guide

## 6 Copilot Capabilities Across Real-World Department of Education Scenarios (GCC-High Cloud, Web Grounding Disabled)

**Version:** October 22, 2025  
**Classification:** UNCLASSIFIED  
**Duration:** 3 hours (6 scenarios × 20-25 min each)

---

## Table of Contents

- [Workshop Overview](#workshop-overview)
- [Prerequisites & Setup](#prerequisites--setup)
- [Scenario Modules](#scenario-modules)
  - [Scenario 1: Language Understanding & Generation](#scenario-1-language-understanding--generation)
  - [Scenario 2: Reasoning & Decision Support](#scenario-2-reasoning--decision-support)
  - [Scenario 3: Data Analysis & Visualization](#scenario-3-data-analysis--visualization)
  - [Scenario 4: Automation & Orchestration](#scenario-4-automation--orchestration)
  - [Scenario 5: Search & Retrieval](#scenario-5-search--retrieval)
  - [Scenario 6: Personalization & Context Awareness](#scenario-6-personalization--context-awareness)
- [Quick Reference](#quick-reference)

---

## Workshop Overview

This guide provides facilitators with the structure and technical steps to facilitate a hands-on workshop for U.S. Department of Education personnel on using standalone Copilot Chat. The workshop demonstrates six independent scenarios, each highlighting a unique Copilot capability in authentic educational policy, grant administration, and program management contexts at headquarters and regional offices.


### Training Objectives
- Demonstrate how to use Microsoft 365 Copilot Chat (with web grounding disabled by admin policy) to enhance productivity in Microsoft 365 applications.
- Build skills in progressive prompt building, meta-prompting, and chain of reasoning for effective Copilot interactions.
- Apply Copilot capabilities to real-world Department of Education tasks relevant to both Entry-level (GS-7/GS-9) and Mid-level (GS-11/GS-13) personas.
- Ensure participants can copy/paste and/or upload files between Copilot Chat and M365 apps in a secure government cloud environment.

### Target Audience Description
- **Personas:** Entry-level (junior program specialists and grants management specialists) and Mid-level (experienced program officers and division directors overseeing operations).
- **Skill Level:** L100-L200 (beginner to intermediate familiarity with M365 apps and basic prompting).
- **Environment:** Department of Education headquarters, regional offices, and field sites, focusing on grant administration, program oversight, policy development, and student services.

### Workshop Structure
The workshop consists of six independent scenarios, each 20-25 minutes, allowing flexibility for breaks or Q&A. Scenarios do not build on each other and can be reordered if needed.

### Facilitation Approach
- Guide participants through technical steps without scripts.
- Emphasize hands-on practice with progressive prompts.
- Monitor for compliance with standalone Copilot Chat usage (no in-app integrations).
- Encourage discussion on meta-prompting and chain of reasoning.


### Required Materials/Setup
- Laptops with Microsoft 365 E5 **plus Microsoft 365 Copilot add-on licenses** (GCC-High compliant).
- Access to Microsoft 365 Copilot Chat via web browser (web-only for government cloud tenants).
- Sample data files (e.g., mock grant applications, policy documents, program reports) pre-loaded in M365 apps.
- Venue with good connectivity both for participants and facilitator.
- Projector for demonstrating steps.

### Timing Breakdown
- Introduction: 10 minutes
- Each Scenario: 20-25 minutes (setup 2 min, hands-on 15 min, discussion 5 min)
- Breaks: 10 minutes total
- Wrap-up: 10 minutes  
⏱️ **Total:** 3 hours

---

## Prerequisites & Setup.

### For Facilitator
- Verify GCC-High environment: Standalone Copilot Chat enabled, no web grounding or M365 Copilot integrations.
- Prepare sample datasets: Mock Department of Education documents (e.g., grant applications, compliance reports, policy briefs) compliant with UNCLASSIFIED handling.
- Test workflows: Copy/paste between Copilot Chat and M365 apps.
- Setup attendee accounts: Ensure participants have access to required apps.
- Change mouse pointer size and color.


### Technical Environment Verification
- Confirm **web search grounding is disabled**: Copilot Chat is configured by admin policy to not use web search.
- Verify GCC-High cloud environment: Confirm government tenant (web-only Copilot Chat experience).
- Check Copilot license assignments: All participants have Microsoft 365 Copilot add-on licenses.
- Check app versions: Outlook, Word, Excel, Power Automate, Power BI, Teams (latest government-approved).
- Validate security: All activities in approved government network environment.


### Required Attendee Access/Accounts
- Microsoft 365 accounts with Copilot Chat and Microsoft 365 Copilot add-on license access.
- Permissions for M365 apps in scenarios.
- Power BI desktop client installed.


### Pre-Work Attendees Should Complete
- Review basic Copilot Chat interface (5-10 min tutorial).
- Familiarize with M365 apps used in scenarios.
- Review government cloud limitations for Copilot features (web-only, some features may be restricted).


### Expected Baseline Knowledge for Attendees
- Basic navigation in M365 apps.
- Understanding of Department of Education organizational structure (offices and programs).
- Familiarity with education terminology (e.g., Title I, IDEA, Pell Grants, FERPA, ESSA).

---

## Scenario Modules

### Introduction

- Team Introduction
    - Bonus points: Use M365 Copilot to introduce yourself with this prompt and play the response on the room's speakers:  
    ```
    "Hi Copilot, I'm giving a workshop on Copilot Chat to Department of Education personnel. Please introduce me to the participants in 100 words or less."
    ```
- Administrative Topics
- Rules of Engagement:
  - This is meant to be hands-on and immersive.  We learn by doing.  Dive in.
  - If you fall behind or you miss something, don't be bashful, let me know.
  - Ask questions.  A ton of them!

### Lead an AI Discussion
Start by getting a gauge for your audience and their thoughts on AI.  This can be done by asking open-ended questions and giving your participants room to speak. Rather than answering them directly, open it up to the rest of the room, "Yeah, that's a great comment.  Does anyone have any thoughts on that?"  

Another great way is by using Microsoft Forms and having folks submit answers to, "What are your thoughts on AI in three words or less?"

Some talking points that will most likely be discussed:
- AI is bad for society
- AI hallucinations
- AI increases productivity and efficiency
- AI makes it easier for bad actors to do bad things

In the end, the conversation should lead to this:  
```
No matter your viewpoint on AI, our enemies are using it.  If we don't want to bring bows and arrows to the next battle, then we need to use AI as well.  This session is designed to give you hands-on experience into six AI functions and hopefully some insight how you can use AI in your day-to-day work.
```
Let's dive right in...

### Scenario 1: Language Understanding & Generation
**Application:** Outlook | **ED Focus:** Office of Federal Student Aid (FSA) | **Duration:** 20-25 min

#### Scenario Context
At the Department of Education's Office of Federal Student Aid, a program specialist (GS-9) processes student loan inquiries and responds to institution questions, while a program officer (GS-13) oversees case management. Use Copilot to handle email correspondence on student aid applications, loan servicing inquiries, and institutional compliance questions. This demonstrates efficient communication in student aid operations.

#### Copilot Capability Focus
- Primary: Language Understanding & Generation for summarization and drafting.
- Sub-capabilities: Tone adjustment, content rewriting, action item extraction.
- Application to ED: Streamlines student aid services, ensuring professional tone aligned with Department protocols.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Summarize this email thread about student loan inquiries.
```
- What this prompt does: Provides a simple overview of the thread.
- Output example: A short paragraph listing key points.
- Limitations: Lacks ED context, may miss deadlines or regulatory references.

##### Iteration 2: Add Context
```
Summarize this email thread about student loan inquiries at the Office of Federal Student Aid, including applicant details and processing deadlines.
```
- How context improves output: Incorporates ED specifics like loan types and applicant information.
- Comparison to iteration 1: More detailed, identifies action items like application review scheduling.

##### Iteration 3: Add Specificity
```
Summarize this email thread about student aid inquiries in a structured format: Key applicants and case numbers, main action items, deadlines, and draft a response email to the applicant using professional government tone.
```
- Why specificity matters: Ensures formatted output for easy pasting into Outlook.
- Improved output quality: Includes bullet points and a drafted response.

##### Iteration 4: Final Optimized Prompt
```
As a program specialist at the Office of Federal Student Aid, summarize this email thread on student loan inquiries: List applicants by case number and loan type, extract action items and processing deadlines, then draft a response email with formal government language, ensuring compliance with Higher Education Act guidance.
```
- Final refinements: Adds regulatory reference for authenticity.
- Complete output example: Structured list plus full email draft.


#### Technical Steps
1. Open the [sample email thread](/DOE/sample%20data/scenario1_email_thread.txt) on student aid inquiries and review the contents.
2. Either upload the [sample email file](/DOE/sample%20data/scenario1_email_thread.txt) to Copilot Chat or copy and paste the thread content into the chat interface.
3. Enter progressive prompts (iterations 1-4) one by one, observing improvements with each iteration.
4. Review Copilot's output (summary and draft response). Note that in a real-world scenario, this output could be used to reply to the actual email thread.
5. Verify tone adjustment for internal vs. external communications.

#### Facilitation Notes
> 💡 **Tips:**
> - Watch for copy/paste errors between windows.
> - Checkpoint: Ask participants to share one improved action item.
> - Troubleshooting: If output is vague, remind to add ED context.
> - Explain benefits: Progressive prompts reduce revisions in student aid workflows.

#### Expected Outcomes
- ✅ Deliverable: Summarized thread and drafted email in Outlook.
- ✅ Verification: Output matches professional government tone and includes deadlines.
- ✅ Capability demonstration: Clear language generation for student aid correspondence.
- ✅ Prompt building: Participants iterate prompts 3-4 times.

#### Discussion Points

**Meta-Prompting**
- Enhance by asking Copilot to refine prompts: "Help me create an effective prompt to summarize student loan inquiry emails. What ED details should I include?"
- Valuable when starting complex tasks like loan consolidation documentation processing.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Identify key emails, 2) Extract case numbers and actions, 3) Generate summary, 4) Draft response."
- Improves quality for detailed student aid reports.

**When to Use**
- Use complex prompts for high-stakes communications like formal determinations or compliance responses.
- Trade-offs: Simple prompts for quick tasks; complex for accuracy in student aid duties.
- Real-world: Drafting loan forgiveness determination letters or institutional compliance responses.

---

### Scenario 2: Reasoning & Decision Support
**Application:** Word | **ED Focus:** Office of Elementary and Secondary Education (OESE) | **Duration:** 20-25 min

#### Scenario Context
At the Office of Elementary and Secondary Education, a program specialist (GS-11) drafts policy briefs and program reports, while a division director (GS-14) reviews grant guidance documents. Use Copilot to structure documents and resolve conflicts in policy analysis and ESSA implementation reporting.

#### Copilot Capability Focus
- Primary: Reasoning & Decision Support for analysis and recommendations.
- Sub-capabilities: Conflict identification, priority frameworks, comparative options.
- Application to ED: Aids in efficient policy development, ensuring alignment with Department guidance and statutory requirements.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Draft a policy brief on educational program developments.
```
- What this prompt does: Generates a generic outline.
- Output example: Basic document structure.
- Limitations: Ignores ED specifics like ESSA requirements or program priorities.

##### Iteration 2: Add Context
```
Draft a policy brief on Title I program developments for the Office of Elementary and Secondary Education, including key implementation trends and state compliance impacts.
```
- How context improves output: Adds office and focus area.
- Comparison to iteration 1: Includes realistic programmatic considerations.

##### Iteration 3: Add Specificity
```
Draft a policy brief in standard Department of Education format: Include sections for background, analysis, recommendations; identify potential policy conflicts; suggest prioritization based on educational equity objectives.
```
- Why specificity matters: Structures output per ED standards.
- Improved output quality: Provides reasoned recommendations.

##### Iteration 4: Final Optimized Prompt
```
As a program specialist at the Office of Elementary and Secondary Education, draft a policy brief: Structure with standard Department format matching Administrative guidance, analyze conflicts between competing program priorities under ESSA, recommend courses of action based on educational equity objectives, and suggest risk mitigations for state engagement.
```
- Final refinements: Incorporates doctrinal references.
- Complete output example: Full policy brief with decision framework.


#### Technical Steps
1. Open [sample document](/DOE/sample%20data/scenario2_training_data.txt) for the policy brief.
2. Upload the sample data file or paste sample policy data (e.g., program developments list) into Copilot Chat.
3. Input progressive prompts, refining based on outputs.
4. Optional: Copy recommendations and structure into a new Word document.
5. Edit for final formatting, demonstrating reasoning application.

#### Facilitation Notes
> 💡 **Tips:**
> - Monitor for prompt overload; break into steps.
> - Checkpoint: Verify policy analysis in output.
> - Troubleshooting: If recommendations are off, add more context.
> - Explain benefits: Builds logical decision-making in policy development.

#### Expected Outcomes
- ✅ Deliverable: Structured policy brief in Word with recommendations.
- ✅ Verification: Includes policy analysis and priorities.
- ✅ Capability demonstration: Reasoning for programmatic decisions.
- ✅ Prompt building: 3-4 iterations showing progressive logic.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to analyze policy conflicts. What programmatic considerations should I include?"
- Valuable for developing guidance documents and state engagement strategies.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) List developments, 2) Identify policy implications, 3) Evaluate priorities, 4) Recommend actions."
- Improves for program reports and grant guidance drafting.

**When to Use**
- Complex prompts for multi-factor decisions like formula grant allocations.
- Trade-offs: Simple for outlines; complex for in-depth analysis.
- Real-world: Updating state plan guidance or Congressional testimony prep.

---

### Scenario 3: Data Analysis & Visualization
**Application:** Excel | **ED Focus:** Office of Management (OM) | **Duration:** 20-25 min

#### Scenario Context
At the Department of Education's Office of Management, a management analyst (GS-11) tracks facility assets and equipment inventory, while a management officer (GS-14) analyzes resource allocation data. Use Copilot to interpret facility management logs and budget tracking.

#### Copilot Capability Focus
- Primary: Data Analysis & Visualization for insights and chart suggestions.
- Sub-capabilities: Pattern detection, bottleneck identification, visualization recommendations.
- Application to ED: Enhances resource management accountability and operational efficiency.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Analyze this facility equipment data.
```
- What this prompt does: Gives basic summary.
- Output example: Average utilization rates.
- Limitations: No patterns or visuals.

##### Iteration 2: Add Context
```
Analyze this Department of Education facility equipment data from headquarters, including asset conditions and replacement schedules.
```
- How context improves output: Ties to ED facility management.
- Comparison to iteration 1: Identifies specific issues like equipment lifecycle concerns.

##### Iteration 3: Add Specificity
```
Analyze this data: Identify patterns in maintenance issues, calculate operational readiness rates, suggest visualizations like bar charts for resource allocation bottlenecks.
```
- Why specificity matters: Directs to actionable insights.
- Improved output quality: Includes chart types and explanations.

##### Iteration 4: Final Optimized Prompt
```
As a management officer at Department of Education headquarters, analyze this facility asset data: Detect patterns in equipment failures, provide insights on procurement needs, recommend Excel visualizations (e.g., pie charts) for management briefings and budget justifications.
```
- Final refinements: Adds briefing context.
- Complete output example: Insights plus chart descriptions.


#### Technical Steps
1. Open Excel with [sample facility dataset](/DOE/sample%20data/scenario3_equipment_readiness.csv) and review the data.
2. Create a table in Excel: Select the data range, then click **Insert > Table** (or press Ctrl+T) and confirm the range includes headers.
3. **Option A - Copy/Paste:** Copy the table data range and paste into Copilot Chat.
   **Option B - Drag/Drop:** First save the file as an Excel workbook (.xlsx) with **File > Save As**, then drag and drop the .xlsx file into Copilot Chat.
4. Use progressive prompts to generate insights.
5. Copy suggestions back to Excel to create charts.
6. Verify patterns match data.

#### Facilitation Notes
> 💡 **Tips:**
> - Ensure data is pasted accurately.
> - Checkpoint: Participants create one recommended chart.
> - Troubleshooting: If insights miss, add row/column details.
> - Explain benefits: Visuals aid quick management decisions.

#### Expected Outcomes
- ✅ Deliverable: Analyzed data with charts in Excel.
- ✅ Verification: Insights highlight resource gaps.
- ✅ Capability demonstration: Data interpretation for facility management.
- ✅ Prompt building: Iterations refine analysis depth.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to analyze facility data. What metrics to include?"
- Valuable for budget execution reports.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Calculate utilization rates, 2) Spot patterns, 3) Identify causes, 4) Suggest visuals."
- Improves for asset tracking and procurement planning.

**When to Use**
- Complex prompts for trend analysis across multiple facilities.
- Trade-offs: Simple for summaries; complex for visuals.
- Real-world: Annual facility inventory audits and budget justifications.

---

### Scenario 4: Automation & Orchestration
**Application:** Power Automate | **ED Focus:** Office of the Chief Information Officer (OCIO) | **Duration:** 20-25 min

#### Scenario Context
At the Department of Education's Office of the Chief Information Officer, an IT specialist (GS-9) processes IT service tickets, while an IT manager (GS-13) designs workflow improvements. Use Copilot to build automations for IT support and system access requests.

#### Copilot Capability Focus
- Primary: Automation & Orchestration for workflow design.
- Sub-capabilities: Logic optimization, decision branching, process troubleshooting.
- Application to ED: Streamlines IT service delivery and system administration.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Design a workflow for IT help desk tickets.
```
- What this prompt does: Basic flow outline.
- Output example: Simple steps.
- Limitations: No ED specifics.

##### Iteration 2: Add Context
```
Design a workflow for Department of Education IT help desk tickets, including routing to IT specialists.
```
- How context improves output: Adds government environment elements.
- Comparison to iteration 1: Includes notification protocols.

##### Iteration 3: Add Specificity
```
Design a Power Automate flow: Trigger on new ticket submission, route based on issue type (network/application/hardware), send notifications, track resolution times.
```
- Why specificity matters: Defines triggers and actions.
- Improved output quality: Step-by-step logic.

##### Iteration 4: Final Optimized Prompt
```
As an IT specialist at Department of Education OCIO, design a Power Automate flow for IT helpdesk: Trigger on email ticket, branch logic for system access requests, optimize for compliance with FISMA policies, troubleshoot potential errors.
```
- Final refinements: Adds compliance reference.
- Complete output example: Full flow description.


#### Technical Steps
1. Open Power Automate and start a new flow.
2. Upload or paste [ticket sample data](/DOE/sample%20data/scenario4_helpdesk_tickets.csv) into Copilot Chat.
3. Use prompts to generate flow logic and step-by-step pseudocode (Copilot does not directly automate Power Automate flows; users must implement logic manually).
4. Copy Copilot's suggested steps to Power Automate and build the flow.
5. Test basic automation.

#### Facilitation Notes
> 💡 **Tips:**
> - Guide on flow connectors.
> - Checkpoint: Verify branching logic.
> - Troubleshooting: If logic fails, refine prompt with errors.
> - Explain benefits: Reduces manual IT service tasks.

#### Expected Outcomes
- ✅ Deliverable: Working flow in Power Automate.
- ✅ Verification: Routes tickets correctly.
- ✅ Capability demonstration: Orchestration for IT processes.
- ✅ Prompt building: Iterations optimize automation.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to design IT ticket workflows. What decision branches to include?"
- Valuable for Standard Operating Procedure automation.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Define trigger, 2) Add conditions, 3) Set actions, 4) Test logic."
- Improves for IT service management.

**When to Use**
- Complex prompts for branched flows with multiple approval levels.
- Trade-offs: Simple for basics; complex for optimization.
- Real-world: System access request processing.

---

### Scenario 5: Search & Retrieval
**Application:** Power BI | **ED Focus:** Institute of Education Sciences (IES) | **Duration:** 20-25 min

#### Scenario Context
At the Institute of Education Sciences, a research analyst (GS-11) compiles education research data, while a program officer (GS-13) organizes national education statistics reports. Use Copilot to extract information from education dashboards for analytical products.

#### Copilot Capability Focus
- Primary: Search & Retrieval for data extraction.
- Sub-capabilities: Information organization, key point consolidation, content finding.
- Application to ED: Supports analytical reporting and evidence-based decision making.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Find key indicators in this data.
```
- What this prompt does: Lists basic items.
- Output example: Unstructured list.
- Limitations: No organization.

##### Iteration 2: Add Context
```
Find specific educational achievement and enrollment indicators from this education statistics dashboard data at IES, focusing on national trends.
```
- How context improves output: Ties to ED analytical work.
- Comparison to iteration 1: Groups by topic area.

##### Iteration 3: Add Specificity
```
Extract education indicators: Organize into categories (e.g., achievement gaps, enrollment trends, graduation rates), include sources and dates, create a structured analytical brief.
```
- Why specificity matters: Formats for easy use in reporting.
- Improved output quality: Tabular extraction.

##### Iteration 4: Final Optimized Prompt
```
As a research analyst at the Institute of Education Sciences, search this Power BI dashboard data: Retrieve key indicators from education research reports, organize by analytical priority, extract critical points for a condition of education report per IES standards.
```
- Final refinements: Adds priority and analytical standards.
- Complete output example: Structured summary.


#### Technical Steps
1. Open Power BI with [sample education dataset](/DOE/sample%20data/scenario5_intelligence_data.csv).
2. Copy dashboard metrics or visual descriptions into Copilot Chat (Copilot does not directly extract data from Power BI dashboards; users must manually describe or export data).
3. Use prompts to extract and organize data.
4. Copy organized output back to Power BI notes or report.
5. Verify extraction accuracy.

#### Facilitation Notes
> 💡 **Tips:**
> - Describe visuals if not copyable.
> - Checkpoint: Check organized indicators.
> - Troubleshooting: Add more data details if missed.
> - Explain benefits: Speeds analytical consolidation.

#### Expected Outcomes
- ✅ Deliverable: Extracted brief from dashboard.
- ✅ Verification: Includes key indicators.
- ✅ Capability demonstration: Retrieval for analytical tasks.
- ✅ Prompt building: Iterations enhance organization.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to extract education data. What categories to include?"
- Valuable for national education statistics reports.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Scan data, 2) Identify indicators, 3) Categorize, 4) Organize brief."
- Improves for condition of education assessments and research briefs.

**When to Use**
- Complex prompts for large datasets across multiple sources.
- Trade-offs: Simple for quick finds; complex for structured analysis.
- Real-world: Annual condition of education report compilation or Congressional testimony data.

---

### Scenario 6: Personalization & Context Awareness
**Application:** Teams | **ED Focus:** Office of the Secretary (OS) | **Duration:** 20-25 min

#### Scenario Context
At the Office of the Secretary, a staff assistant (GS-11) uses a Teams meeting transcript to summarize senior staff meetings, while a Deputy Assistant Secretary (SES) generates agendas. Use Copilot to adapt communications to rank and role in Department leadership coordination.

#### Copilot Capability Focus
- Primary: Personalization & Context Awareness for adaptive content.
- Sub-capabilities: Terminology adjustment, role-specific suggestions, organizational hierarchy awareness.
- Application to ED: Ensures appropriate language in executive communications and leadership coordination.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Summarize this meeting notes.
```
- What this prompt does: General overview.
- Output example: Plain summary.
- Limitations: No ED adaptation.

##### Iteration 2: Add Context
```
Summarize these senior staff meeting notes from Department of Education headquarters, including key decisions and action items.
```
- How context improves output: Adds location and government focus.
- Comparison to iteration 1: Mentions sections vaguely.

##### Iteration 3: Add Specificity
```
Summarize notes: Use government terminology, adapt language for office directors and Deputy Secretaries, generate follow-up messages aligned with organizational hierarchy.
```
- Why specificity matters: Personalizes tone.
- Improved output quality: Role-appropriate phrasing.

##### Iteration 4: Final Optimized Prompt
```
As a staff assistant at the Office of the Secretary, summarize senior staff meeting notes: Incorporate Department policy references, personalize follow-ups by position (e.g., formal for Secretary and Deputy Secretary), demonstrate context awareness of Department organizational structure and reporting relationships.
```
- Final refinements: Adds policy references.
- Complete output example: Adapted summary and messages.


#### Technical Steps
1. Open the [sample meeting transcript](/DOE/sample%20data/scenario6_meeting_transcript.txt) and review.
2. Copy or upload sample meeting transcript into Copilot Chat.
3. Apply progressive prompts for refinements.
4. Paste personalized output back to Teams chat or meeting notes.
5. Check context alignment.

#### Facilitation Notes
> 💡 **Tips:**
> - Focus on role and rank sensitivity.
> - Checkpoint: Verify tone in follow-ups.
> - Troubleshooting: Add more context if generic.
> - Explain benefits: Enhances leadership team collaboration.

#### Expected Outcomes
- ✅ Deliverable: Personalized summary in Teams.
- ✅ Verification: Adapts to organizational hierarchy.
- ✅ Capability demonstration: Context-aware generation.
- ✅ Prompt building: Iterations build personalization.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt for role-appropriate summaries. What government context to include?"
- Valuable for Secretary-level briefing preparation.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Review notes, 2) Identify actions, 3) Adapt tone, 4) Generate messages."
- Improves for executive communications and leadership coordination.

**When to Use**
- Complex prompts for audience-specific government tasks.
- Trade-offs: Simple for basics; complex for personalization.
- Real-world: Senior staff meeting coordination or Secretary action requests.

---

## Quick Reference

### Summary Table of All 6 Scenarios

| Scenario | Capability | Application | ED Focus | Duration |
|----------|------------|-------------|------------|----------|
| 1 | Language Understanding & Generation | Outlook | Federal Student Aid (FSA) | 20-25 min |
| 2 | Reasoning & Decision Support | Word | Elementary and Secondary Education (OESE) | 20-25 min |
| 3 | Data Analysis & Visualization | Excel | Office of Management (OM) | 20-25 min |
| 4 | Automation & Orchestration | Power Automate | Chief Information Officer (OCIO) | 20-25 min |
| 5 | Search & Retrieval | Power BI | Institute of Education Sciences (IES) | 20-25 min |
| 6 | Personalization & Context Awareness | Teams | Office of the Secretary (OS) | 20-25 min |

### Progressive Prompt Building Tips
- Start basic, add context, then specificity.
- Use 3-4 iterations to show improvements.
- Include ED education terminology for relevance.

### Key Talking Points for Each Copilot Capability
- Language Understanding: Focus on tone and drafting for student aid and program communications.
- Reasoning: Emphasize decisions and policy frameworks.
- Data Analysis: Highlight insights and visuals for management and budgeting.
- Automation: Stress logic and optimization for IT and administrative processes.
- Search: Prioritize extraction and organization for analytical products.
- Personalization: Adapt to organizational context and government protocols.

### Meta-Prompting and Chain of Reasoning Quick Reference
- **Meta-Prompting Example:** "Help me build a prompt for [task]. Suggest improvements."
- **Chain of Reasoning Example:** "Step by step: 1) Analyze, 2) Recommend, 3) Output."
- Use when outputs need structure or depth.

### Common Questions with Answers
- Q: Why no web search? A: Government cloud environment restricts external grounding for security.
- Q: How to handle vague outputs? A: Iterate prompts with more educational and contextual details.


### Troubleshooting Common Issues
- Copy/paste fails: Check windows focus.
- File upload fails: Use copy/paste as fallback.
- Generic outputs: Add ED context and educational terminology.
- App access: Verify licenses (Microsoft 365 E5 + Copilot add-on).


### Additional Learning Resources
- [Microsoft Learn: Copilot Fundamentals](https://learn.microsoft.com/en-us/microsoft-copilot/)
- [Microsoft Learn: Prompt Engineering](https://learn.microsoft.com/en-us/training/modules/engineer-copilot-prompts/)
- [Microsoft Learn: Copilot for Government Cloud](https://learn.microsoft.com/en-us/office365/servicedescriptions/office-365-platform-service-description/microsoft-365-copilot#feature-availability)
- ED-specific: Internal training modules on M365 and educational program communications (if available).
