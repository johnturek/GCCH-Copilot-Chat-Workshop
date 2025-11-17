# Federal Bureau of Investigation Copilot Chat Hands-On Workshop: Proctor Guide

## 6 Copilot Capabilities Across Real-World FBI Scenarios (GCC-High Cloud, Web Grounding Disabled)

**Version:** November 17, 2025  
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

This guide provides facilitators with the structure and technical steps to facilitate a hands-on workshop for FBI personnel on using standalone Copilot Chat. The workshop demonstrates six independent scenarios, each highlighting a unique Copilot capability in authentic law enforcement, intelligence, and administrative contexts at FBI field offices, headquarters, and operational units.


### Training Objectives
- Demonstrate how to use Microsoft 365 Copilot Chat (with web grounding disabled by admin policy) to enhance productivity in Microsoft 365 applications.
- Build skills in progressive prompt building, meta-prompting, and chain of reasoning for effective Copilot interactions.
- Apply Copilot capabilities to real-world FBI tasks relevant to both Entry-level (GS-7/GS-9, Intelligence Analysts, Staff Operations Specialists) and Mid-level (GS-11/GS-13, Supervisory Special Agents, Senior Intelligence Analysts) personas.
- Ensure participants can copy/paste and/or upload files between Copilot Chat and M365 apps in a secure government cloud environment.

### Target Audience Description
- **Personas:** Entry-level (new Special Agents, Intelligence Analysts, professional staff) and Mid-level (Supervisory Special Agents, Senior Intelligence Analysts, Unit Chiefs).
- **Skill Level:** L100-L200 (beginner to intermediate familiarity with M365 apps and basic prompting).
- **Environment:** FBI field offices, headquarters divisions, operational squads, and intelligence units focusing on investigative, analytical, administrative, and operational support work.

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
- Sample data files (e.g., mock case files, intelligence reports, operational documents) pre-loaded in M365 apps.
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
- Prepare sample datasets: Mock FBI documents (e.g., case communications, intelligence reports, operational data) compliant with UNCLASSIFIED handling.
- Test workflows: Copy/paste between Copilot Chat and M365 apps.
- Setup attendee accounts: Ensure participants have access to required apps.
- Change mouse pointer size and color.


### Technical Environment Verification
- Confirm **web search grounding is disabled**: Copilot Chat is configured by admin policy to not use web search.
- Verify GCC-High cloud environment: Confirm government tenant (web-only Copilot Chat experience).
- Check Copilot license assignments: All participants have Microsoft 365 Copilot add-on licenses.
- Check app versions: Outlook, Word, Excel, Power Automate, Power BI, Teams (latest government-approved).
- Validate security: All activities in OpenNet or equivalent.


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
- Understanding of FBI organizational structure (divisions, field offices, squads).
- Familiarity with FBI terminology (e.g., investigative leads, intelligence products, case management).

---

## Scenario Modules

### Introduction

- Team Introduction
    - Bonus points: Use M365 Copilot to introduce yourself with this prompt and play the response on the room's speakers:  
    ```
    "Hi Copilot, I'm giving a workshop on Copilot Chat to FBI personnel. Please introduce me to the participants in 100 words or less."
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
No matter your viewpoint on AI, our enemies are using it.  If we don't want to bring bows and arrows to the next battle, then we need to use AI as well.  This session is designed to give you ahnds-on experience into six AI functions and hopefully some insight how you can use AI in your day-to-day work.
```
Let's dive right in...

### Scenario 1: Language Understanding & Generation
**Application:** Outlook | **FBI Focus:** Counterterrorism Division | **Duration:** 20-25 min

#### Scenario Context
At the FBI Washington Field Office, an Intelligence Analyst (GS-11) coordinates investigative leads across multiple squads, while a Supervisory Special Agent (GS-14) oversees case assignments and interagency coordination. Use Copilot to handle email correspondence on counterterrorism investigations, threat assessments, and taskforce coordination. This demonstrates efficient communication in investigative operations.

#### Copilot Capability Focus
- Primary: Language Understanding & Generation for summarization and drafting.
- Sub-capabilities: Tone adjustment, content rewriting, action item extraction.
- Application to FBI: Streamlines investigative communications, ensuring professional law enforcement tone aligned with FBI guidelines and investigative protocols.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Summarize this email thread about investigative leads.
```
- What this prompt does: Provides a simple overview of the thread.
- Output example: A short paragraph listing key points.
- Limitations: Lacks FBI context, may miss critical deadlines or investigative requirements.

##### Iteration 2: Add Context
```
Summarize this email thread about counterterrorism investigative leads at FBI Washington Field Office, including subject details and action deadlines.
```
- How context improves output: Incorporates FBI specifics like case numbers, squad assignments, and subject information.
- Comparison to iteration 1: More detailed, identifies action items like surveillance coordination and taskforce meetings.

##### Iteration 3: Add Specificity
```
Summarize this email thread about investigative leads in a structured format: Key subjects and case numbers, main action items, investigation deadlines, and draft a response email using professional law enforcement tone.
```
- Why specificity matters: Ensures formatted output for easy pasting into Outlook.
- Improved output quality: Includes bullet points and a drafted response.

##### Iteration 4: Final Optimized Prompt
```
As a Supervisory Special Agent at FBI Washington Field Office, summarize this email thread on counterterrorism investigative leads: List subjects by case number and threat category, extract action items and operational deadlines, then draft a response email with formal law enforcement language, ensuring compliance with FBI Domestic Investigations and Operations Guide (DIOG).
```
- Final refinements: Adds regulatory reference for authenticity.
- Complete output example: Structured list plus full email draft.


#### Technical Steps
1. Open the [sample email thread](/FBI/sample%20data/scenario1_email_thread.txt) on investigative leads and review the contents.
2. Either upload the [sample email file](/FBI/sample%20data/scenario1_email_thread.txt) to Copilot Chat or copy and paste the thread content into the chat interface.
3. Enter progressive prompts (iterations 1-4) one by one, observing improvements with each iteration.
4. Review Copilot's output (summary and draft response). Note that in a real-world scenario, this output could be used to reply to the actual email thread.
5. Verify tone adjustment for internal vs. interagency communications.

#### Facilitation Notes
> 💡 **Tips:**
> - Watch for copy/paste errors between windows.
> - Checkpoint: Ask participants to share one improved action item.
> - Troubleshooting: If output is vague, remind to add FBI operational context.
> - Explain benefits: Progressive prompts reduce revisions in investigative workflows.

#### Expected Outcomes
- ✅ Deliverable: Summarized thread and drafted email in Outlook.
- ✅ Verification: Output matches law enforcement tone and includes operational deadlines.
- ✅ Capability demonstration: Clear language generation for investigative correspondence.
- ✅ Prompt building: Participants iterate prompts 3-4 times.

#### Discussion Points

**Meta-Prompting**
- Enhance by asking Copilot to refine prompts: "Help me create an effective prompt to summarize investigative lead emails. What FBI operational details should I include?"
- Valuable when starting complex tasks like threat assessment coordination or taskforce communications.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Identify key emails, 2) Extract case numbers and actions, 3) Generate summary, 4) Draft response."
- Improves quality for detailed investigative reports.

**When to Use**
- Use complex prompts for high-stakes communications like formal investigative requests or interagency coordination.
- Trade-offs: Simple prompts for quick tasks; complex for accuracy in case management.
- Real-world: Drafting lead assignment memos or operational coordination emails.

---

### Scenario 2: Reasoning & Decision Support
**Application:** Word | **FBI Focus:** Criminal Investigative Division | **Duration:** 20-25 min

#### Scenario Context
At FBI Headquarters in Washington D.C., a Senior Intelligence Analyst (GS-13) drafts intelligence assessments and threat reports, while a Unit Chief reviews analytical products for investigative prioritization. Use Copilot to structure documents and resolve conflicts in threat analysis and resource allocation.

#### Copilot Capability Focus
- Primary: Reasoning & Decision Support for analysis and recommendations.
- Sub-capabilities: Threat identification, priority frameworks, comparative investigative approaches.
- Application to FBI: Aids in efficient intelligence analysis, ensuring alignment with FBI priorities and investigative guidelines.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Draft a threat assessment on criminal activities.
```
- What this prompt does: Generates a generic outline.
- Output example: Basic document structure.
- Limitations: Ignores FBI specifics like intelligence product format or investigative priorities.

##### Iteration 2: Add Context
```
Draft a threat assessment on cybercrime developments for FBI Headquarters Criminal Investigative Division, including key threat trends and impact on national security.
```
- How context improves output: Adds division focus and threat area.
- Comparison to iteration 1: Includes realistic investigative considerations.

##### Iteration 3: Add Specificity
```
Draft a threat assessment in standard FBI intelligence product format: Include sections for executive summary, threat analysis, investigative recommendations; identify potential resource conflicts; suggest prioritization based on FBI strategic priorities.
```
- Why specificity matters: Structures output per FBI intelligence standards.
- Improved output quality: Provides reasoned investigative recommendations.

##### Iteration 4: Final Optimized Prompt
```
As a Senior Intelligence Analyst at FBI Headquarters, draft a threat assessment: Structure with standard FBI intelligence product format, analyze conflicts between competing investigative priorities, recommend courses of action based on FBI Strategic Plan objectives, and suggest resource allocation strategies for field office coordination.
```
- Final refinements: Incorporates FBI doctrinal references.
- Complete output example: Full threat assessment with decision framework.


#### Technical Steps
1. Open [sample document](/FBI/sample%20data/scenario2_training_data.txt) for the threat assessment.
2. Upload the sample data file or paste sample intelligence data (e.g., threat indicators list) into Copilot Chat.
3. Input progressive prompts, refining based on outputs.
4. Optional: Copy recommendations and structure into a new Word document.
5. Edit for final formatting, demonstrating reasoning application.

#### Facilitation Notes
> 💡 **Tips:**
> - Monitor for prompt overload; break into steps.
> - Checkpoint: Verify threat analysis in output.
> - Troubleshooting: If recommendations are off, add more operational context.
> - Explain benefits: Builds logical decision-making in intelligence analysis.

#### Expected Outcomes
- ✅ Deliverable: Structured threat assessment in Word with recommendations.
- ✅ Verification: Includes threat analysis and investigative priorities.
- ✅ Capability demonstration: Reasoning for investigative decisions.
- ✅ Prompt building: 3-4 iterations showing progressive logic.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to analyze threat priorities. What investigative considerations should I include?"
- Valuable for developing operational plans and intelligence briefings.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) List threats, 2) Identify investigative implications, 3) Evaluate priorities, 4) Recommend actions."
- Improves for intelligence reports and operational planning.

**When to Use**
- Complex prompts for multi-factor decisions like resource allocation across field offices.
- Trade-offs: Simple for outlines; complex for in-depth analysis.
- Real-world: Updating threat assessments or operational briefings for FBI leadership.

---

### Scenario 3: Data Analysis & Visualization
**Application:** Excel | **FBI Focus:** Operational Technology Division | **Duration:** 20-25 min

#### Scenario Context
At FBI Los Angeles Field Office, an IT Specialist (GS-11) tracks surveillance equipment and technical assets, while a Technical Operations Supervisor (GS-13) analyzes resource allocation and operational readiness. Use Copilot to interpret equipment logs and operational capability tracking.

#### Copilot Capability Focus
- Primary: Data Analysis & Visualization for insights and chart suggestions.
- Sub-capabilities: Pattern detection, capability gap identification, visualization recommendations.
- Application to FBI: Enhances operational readiness accountability and resource management efficiency.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Analyze this equipment data.
```
- What this prompt does: Gives basic summary.
- Output example: Average operational readiness rates.
- Limitations: No patterns or visuals.

##### Iteration 2: Add Context
```
Analyze this FBI field office surveillance equipment data from Los Angeles Field Office, including asset conditions and maintenance schedules.
```
- How context improves output: Ties to FBI operational technology management.
- Comparison to iteration 1: Identifies specific issues like equipment lifecycle and operational gaps.

##### Iteration 3: Add Specificity
```
Analyze this data: Identify patterns in equipment failures, calculate operational readiness rates, suggest visualizations like bar charts for capability gaps and resource allocation bottlenecks.
```
- Why specificity matters: Directs to actionable operational insights.
- Improved output quality: Includes chart types and explanations.

##### Iteration 4: Final Optimized Prompt
```
As a Technical Operations Supervisor at FBI Los Angeles Field Office, analyze this surveillance equipment data: Detect patterns in equipment failures, provide insights on procurement needs, recommend Excel visualizations (e.g., pie charts) for operational briefings and budget justifications to support investigative operations.
```
- Final refinements: Adds operational briefing context.
- Complete output example: Insights plus chart descriptions.


#### Technical Steps
1. Open Excel with [sample equipment dataset](/FBI/sample%20data/scenario3_equipment_readiness.csv) and review the data.
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
> - Explain benefits: Visuals aid quick operational decisions.

#### Expected Outcomes
- ✅ Deliverable: Analyzed data with charts in Excel.
- ✅ Verification: Insights highlight operational capability gaps.
- ✅ Capability demonstration: Data interpretation for operational readiness management.
- ✅ Prompt building: Iterations refine analysis depth.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to analyze surveillance equipment data. What operational metrics to include?"
- Valuable for operational capability reports and budget justifications.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Calculate readiness rates, 2) Spot patterns, 3) Identify causes, 4) Suggest visuals."
- Improves for asset tracking and operational planning.

**When to Use**
- Complex prompts for trend analysis across multiple field offices.
- Trade-offs: Simple for summaries; complex for visuals.
- Real-world: Quarterly operational readiness reports and equipment procurement justifications.

---

### Scenario 4: Automation & Orchestration
**Application:** Power Automate | **FBI Focus:** Information Technology Branch | **Duration:** 20-25 min

#### Scenario Context
At FBI Chicago Field Office, an IT Support Specialist (GS-9) processes technical support tickets, while an IT Supervisor (GS-12) designs workflow improvements for case system support. Use Copilot to build automations for IT support tickets and CJIS system access requests.

#### Copilot Capability Focus
- Primary: Automation & Orchestration for workflow design.
- Sub-capabilities: Logic optimization, decision branching, process troubleshooting.
- Application to FBI: Streamlines IT service delivery and investigative system administration.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Design a workflow for IT help desk tickets.
```
- What this prompt does: Basic flow outline.
- Output example: Simple steps.
- Limitations: No FBI specifics.

##### Iteration 2: Add Context
```
Design a workflow for FBI field office IT help desk tickets at Chicago Field Office, including routing to IT specialists and case system support.
```
- How context improves output: Adds operational environment elements.
- Comparison to iteration 1: Includes investigative system notification protocols.

##### Iteration 3: Add Specificity
```
Design a Power Automate flow: Trigger on new ticket submission, route based on issue type (unclassified/CJIS/FBI network), send notifications, track resolution times and SLA compliance.
```
- Why specificity matters: Defines triggers and actions.
- Improved output quality: Step-by-step logic.

##### Iteration 4: Final Optimized Prompt
```
As an IT Supervisor at FBI Chicago Field Office, design a Power Automate flow for IT helpdesk: Trigger on email ticket, branch logic for CJIS system access requests, optimize for compliance with FBI IT security policies, troubleshoot potential errors, and track metrics for operational reporting.
```
- Final refinements: Adds compliance and metrics reference.
- Complete output example: Full flow description.


#### Technical Steps
1. Open Power Automate and start a new flow.
2. Upload or paste [ticket sample data](/FBI/sample%20data/scenario4_helpdesk_tickets.csv) into Copilot Chat.
3. Use prompts to generate flow logic and step-by-step pseudocode (Copilot does not directly automate Power Automate flows; users must implement logic manually).
4. Copy Copilot's suggested steps to Power Automate and build the flow.
5. Test basic automation.

#### Facilitation Notes
> 💡 **Tips:**
> - Guide on flow connectors.
> - Checkpoint: Verify branching logic for security requirements.
> - Troubleshooting: If logic fails, refine prompt with error details.
> - Explain benefits: Reduces manual IT service tasks and improves response times.

#### Expected Outcomes
- ✅ Deliverable: Working flow in Power Automate.
- ✅ Verification: Routes tickets correctly based on system type.
- ✅ Capability demonstration: Orchestration for investigative IT processes.
- ✅ Prompt building: Iterations optimize automation.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to design FBI IT ticket workflows. What decision branches for investigative systems should I include?"
- Valuable for Standard Operating Procedure automation.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Define trigger, 2) Add conditions for system types, 3) Set actions and notifications, 4) Test logic."
- Improves for IT service management and operational support.

**When to Use**
- Complex prompts for branched flows with multiple approval levels and security requirements.
- Trade-offs: Simple for basics; complex for optimization.
- Real-world: CJIS system access request processing and investigative system support.

---

### Scenario 5: Search & Retrieval
**Application:** Power BI | **FBI Focus:** Intelligence Analysis | **Duration:** 20-25 min

#### Scenario Context
At FBI New York Field Office, an Intelligence Analyst (GS-11) compiles criminal intelligence data and threat indicators, while a Supervisory Intelligence Analyst (GS-13) organizes threat assessments and intelligence products. Use Copilot to extract information from intelligence dashboards for investigative and analytical products.

#### Copilot Capability Focus
- Primary: Search & Retrieval for data extraction.
- Sub-capabilities: Information organization, key point consolidation, threat indicator identification.
- Application to FBI: Supports analytical reporting, threat assessments, and investigative situational awareness.

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
Find specific criminal and terrorism indicators from this FBI intelligence dashboard data at New York Field Office, focusing on threat developments and investigative leads.
```
- How context improves output: Ties to FBI analytical work.
- Comparison to iteration 1: Groups by threat category.

##### Iteration 3: Add Specificity
```
Extract intelligence indicators: Organize into categories (e.g., terrorism, cybercrime, organized crime), include sources and dates, create a structured intelligence brief with threat prioritization.
```
- Why specificity matters: Formats for easy use in investigative reporting.
- Improved output quality: Tabular extraction with priorities.

##### Iteration 4: Final Optimized Prompt
```
As an Intelligence Analyst at FBI New York Field Office, search this Power BI dashboard data: Retrieve key threat indicators from intelligence reports, organize by investigative priority, extract critical points for an intelligence product per FBI intelligence standards and analytical tradecraft.
```
- Final refinements: Adds priority and FBI analytical standards.
- Complete output example: Structured intelligence summary.


#### Technical Steps
1. Open Power BI with [sample intelligence dataset](/FBI/sample%20data/scenario5_intelligence_data.csv).
2. Copy dashboard metrics or visual descriptions into Copilot Chat (Copilot does not directly extract data from Power BI dashboards; users must manually describe or export data).
3. Use prompts to extract and organize data.
4. Copy organized output back to Power BI notes or intelligence report.
5. Verify extraction accuracy and threat prioritization.

#### Facilitation Notes
> 💡 **Tips:**
> - Describe visuals if not copyable.
> - Checkpoint: Check organized indicators and threat priorities.
> - Troubleshooting: Add more data details if threat categories missed.
> - Explain benefits: Speeds intelligence consolidation for briefings.

#### Expected Outcomes
- ✅ Deliverable: Extracted intelligence brief from dashboard.
- ✅ Verification: Includes key threat indicators with proper categorization.
- ✅ Capability demonstration: Retrieval for analytical and investigative tasks.
- ✅ Prompt building: Iterations enhance organization.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to extract threat intelligence data. What investigative categories to include?"
- Valuable for threat assessments and intelligence products.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Scan data, 2) Identify threat indicators, 3) Categorize by priority, 4) Organize intelligence brief."
- Improves for threat assessments and investigative summaries.

**When to Use**
- Complex prompts for large datasets across multiple intelligence sources.
- Trade-offs: Simple for quick finds; complex for structured intelligence analysis.
- Real-world: Weekly intelligence summaries, threat briefings, or investigative case analysis.

---

### Scenario 6: Personalization & Context Awareness
**Application:** Teams | **FBI Focus:** Executive Management | **Duration:** 20-25 min

#### Scenario Context
At FBI Headquarters, an Executive Assistant (GS-11) uses a Teams meeting transcript to summarize executive leadership meetings, while an Assistant Director generates agendas and action items. Use Copilot to adapt communications to rank and role in FBI headquarters leadership coordination.

#### Copilot Capability Focus
- Primary: Personalization & Context Awareness for adaptive content.
- Sub-capabilities: Terminology adjustment, role-specific suggestions, organizational hierarchy awareness.
- Application to FBI: Ensures appropriate language in executive communications and leadership coordination across divisions.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Summarize this meeting notes.
```
- What this prompt does: General overview.
- Output example: Plain summary.
- Limitations: No FBI adaptation.

##### Iteration 2: Add Context
```
Summarize these FBI leadership meeting notes from Headquarters, including key decisions and action items across divisions.
```
- How context improves output: Adds organizational and operational focus.
- Comparison to iteration 1: Mentions divisions and priorities.

##### Iteration 3: Add Specificity
```
Summarize notes: Use FBI terminology, adapt language for division chiefs and executive leadership, generate follow-up messages aligned with organizational hierarchy and chain of command.
```
- Why specificity matters: Personalizes tone for law enforcement context.
- Improved output quality: Role-appropriate phrasing for FBI leadership.

##### Iteration 4: Final Optimized Prompt
```
As an Executive Assistant at FBI Headquarters, summarize leadership meeting notes: Incorporate FBI operational priorities and strategic objectives, personalize follow-ups by position (e.g., formal for Director and Executive Assistant Directors), demonstrate context awareness of FBI organizational structure, division responsibilities, and reporting relationships.
```
- Final refinements: Adds FBI strategic context and hierarchy.
- Complete output example: Adapted summary and role-specific messages.


#### Technical Steps
1. Open the [sample meeting transcript](/FBI/sample%20data/scenario6_meeting_transcript.txt) and review.
2. Copy or upload sample meeting transcript into Copilot Chat.
3. Apply progressive prompts for refinements.
4. Paste personalized output back to Teams chat or meeting notes.
5. Check context alignment and hierarchical appropriateness.

#### Facilitation Notes
> 💡 **Tips:**
> - Focus on role and rank sensitivity in FBI hierarchy.
> - Checkpoint: Verify tone in follow-ups for different leadership levels.
> - Troubleshooting: Add more operational context if generic.
> - Explain benefits: Enhances leadership coordination and accountability.

#### Expected Outcomes
- ✅ Deliverable: Personalized summary in Teams.
- ✅ Verification: Adapts to FBI organizational hierarchy.
- ✅ Capability demonstration: Context-aware generation for law enforcement leadership.
- ✅ Prompt building: Iterations build personalization.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt for role-appropriate FBI leadership summaries. What operational context to include?"
- Valuable for Director-level briefing preparation.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Review notes, 2) Identify actions by division, 3) Adapt tone for hierarchy, 4) Generate role-specific messages."
- Improves for executive communications and cross-division coordination.

**When to Use**
- Complex prompts for audience-specific leadership tasks across FBI divisions.
- Trade-offs: Simple for basics; complex for personalization and hierarchy awareness.
- Real-world: Executive leadership meeting coordination or Director action item tracking.

---

## Quick Reference

### Summary Table of All 6 Scenarios

| Scenario | Capability | Application | FBI Focus | Duration |
|----------|------------|-------------|------------|----------|
| 1 | Language Understanding & Generation | Outlook | Counterterrorism Division | 20-25 min |
| 2 | Reasoning & Decision Support | Word | Criminal Investigative Division | 20-25 min |
| 3 | Data Analysis & Visualization | Excel | Operational Technology Division | 20-25 min |
| 4 | Automation & Orchestration | Power Automate | Information Technology Branch | 20-25 min |
| 5 | Search & Retrieval | Power BI | Intelligence Analysis | 20-25 min |
| 6 | Personalization & Context Awareness | Teams | Executive Management | 20-25 min |

### Progressive Prompt Building Tips
- Start basic, add context, then specificity.
- Use 3-4 iterations to show improvements.
- Include FBI operational and investigative terminology for relevance.

### Key Talking Points for Each Copilot Capability
- Language Understanding: Focus on tone and drafting for investigative and interagency communications.
- Reasoning: Emphasize decisions and threat assessment frameworks.
- Data Analysis: Highlight insights and visuals for operational readiness and resource planning.
- Automation: Stress logic and optimization for IT and investigative system support.
- Search: Prioritize extraction and organization for intelligence products and threat assessments.
- Personalization: Adapt to organizational context and FBI hierarchy protocols.

### Meta-Prompting and Chain of Reasoning Quick Reference
- **Meta-Prompting Example:** "Help me build a prompt for [task]. Suggest improvements."
- **Chain of Reasoning Example:** "Step by step: 1) Analyze, 2) Recommend, 3) Output."
- Use when outputs need structure or depth.

### Common Questions with Answers
- Q: Why no web search? A: Government cloud environment restricts external grounding for security.
- Q: How to handle vague outputs? A: Iterate prompts with more investigative and operational contextual details.


### Troubleshooting Common Issues
- Copy/paste fails: Check windows focus.
- File upload fails: Use copy/paste as fallback.
- Generic outputs: Add FBI operational context and investigative terminology.
- App access: Verify licenses (Microsoft 365 E5 + Copilot add-on).


### Additional Learning Resources
- [Microsoft Learn: Copilot Fundamentals](https://learn.microsoft.com/en-us/microsoft-copilot/)
- [Microsoft Learn: Prompt Engineering](https://learn.microsoft.com/en-us/training/modules/engineer-copilot-prompts/)
- [Microsoft Learn: Copilot for Government Cloud](https://learn.microsoft.com/en-us/office365/servicedescriptions/office-365-platform-service-description/microsoft-365-copilot#feature-availability)
- FBI-specific: Internal training modules on M365 and investigative communications (if available).