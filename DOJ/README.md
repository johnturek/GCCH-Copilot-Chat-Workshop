# Department of Justice Copilot Chat Hands-On Workshop: Proctor Guide

## 6 Copilot Capabilities Across Real-World Department of Justice Scenarios (GCC-High Cloud, Web Grounding Disabled)

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

This guide provides facilitators with the structure and technical steps to facilitate a hands-on workshop for U.S. Department of Justice personnel on using standalone Copilot Chat. The workshop demonstrates six independent scenarios, each highlighting a unique Copilot capability in authentic legal, prosecutorial, and administrative contexts at DOJ headquarters, U.S. Attorneys' Offices, and DOJ components.


### Training Objectives
- Demonstrate how to use Microsoft 365 Copilot Chat (with web grounding disabled by admin policy) to enhance productivity in Microsoft 365 applications.
- Build skills in progressive prompt building, meta-prompting, and chain of reasoning for effective Copilot interactions.
- Apply Copilot capabilities to real-world Department of Justice tasks relevant to both Entry-level (GS-7/GS-9, Paralegals, Legal Assistants) and Mid-level (GS-11/GS-13, Trial Attorneys, Assistant U.S. Attorneys) personas.
- Ensure participants can copy/paste and/or upload files between Copilot Chat and M365 apps in a secure government cloud environment.

### Target Audience Description
- **Personas:** Entry-level (Paralegals, Legal Assistants, Staff Attorneys) and Mid-level (Trial Attorneys, Assistant U.S. Attorneys, Senior Counsel).
- **Skill Level:** L100-L200 (beginner to intermediate familiarity with M365 apps and basic prompting).
- **Environment:** DOJ headquarters, U.S. Attorneys' Offices, and DOJ components (Civil Division, Criminal Division, National Security Division, etc.), focusing on legal research, case management, litigation support, and administrative work.

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
- Sample data files (e.g., mock legal memoranda, case documents, discovery materials) pre-loaded in M365 apps.
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
- Prepare sample datasets: Mock Department of Justice documents (e.g., legal memoranda, case files, discovery documents) compliant with UNCLASSIFIED handling.
- Test workflows: Copy/paste between Copilot Chat and M365 apps.
- Setup attendee accounts: Ensure participants have access to required apps.
- Change mouse pointer size and color.


### Technical Environment Verification
- Confirm **web search grounding is disabled**: Copilot Chat is configured by admin policy to not use web search.
- Verify GCC-High cloud environment: Confirm government tenant (web-only Copilot Chat experience).
- Check Copilot license assignments: All participants have Microsoft 365 Copilot add-on licenses.
- Check app versions: Outlook, Word, Excel, Power Automate, Power BI, Teams (latest government-approved).
- Validate security: All activities on DOJ network or equivalent.


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
- Understanding of Department of Justice organizational structure (Main Justice divisions, U.S. Attorneys' Offices, components).
- Familiarity with legal terminology (e.g., pleadings, discovery, motions, legal memoranda).

---

## Scenario Modules

### Introduction

- Team Introduction
    - Bonus points: Use M365 Copilot to introduce yourself with this prompt and play the response on the room's speakers:  
    ```
    "Hi Copilot, I'm giving a workshop on Copilot Chat to Department of Justice personnel. Please introduce me to the participants in 100 words or less."
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
**Application:** Outlook | **DOJ Focus:** U.S. Attorney's Office - Criminal Division | **Duration:** 20-25 min

#### Scenario Context
At the U.S. Attorney's Office for the District of Columbia, a Paralegal Specialist (GS-9) coordinates discovery responses and case communications, while an Assistant U.S. Attorney (GS-14) oversees case strategy and litigation. Use Copilot to handle email correspondence on criminal case coordination, discovery requests, and court filing deadlines. This demonstrates efficient communication in federal prosecution.

#### Copilot Capability Focus
- Primary: Language Understanding & Generation for summarization and drafting.
- Sub-capabilities: Tone adjustment, content rewriting, action item extraction.
- Application to DOJ: Streamlines litigation support, ensuring professional legal tone aligned with Federal Rules of Criminal Procedure and DOJ policies.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Summarize this email thread about discovery requests.
```
- What this prompt does: Provides a simple overview of the thread.
- Output example: A short paragraph listing key points.
- Limitations: Lacks DOJ context, may miss court deadlines or legal requirements.

##### Iteration 2: Add Context
```
Summarize this email thread about discovery requests in a federal criminal case, including defendant information and court-imposed deadlines.
```
- How context improves output: Incorporates DOJ specifics like case numbers, discovery categories, and court deadlines.
- Comparison to iteration 1: More detailed, identifies action items like document production and privilege reviews.

##### Iteration 3: Add Specificity
```
Summarize this email thread about criminal discovery in a structured format: Key defendants and case numbers, main action items, court deadlines, and draft a response email using professional legal tone.
```
- Why specificity matters: Ensures formatted output for easy pasting into Outlook.
- Improved output quality: Includes bullet points and a drafted response.

##### Iteration 4: Final Optimized Prompt
```
As an Assistant U.S. Attorney in the District of Columbia, summarize this email thread on criminal discovery: List defendants by case number and charge type, extract action items and court-ordered deadlines, then draft a response email with formal legal language, ensuring compliance with Federal Rules of Criminal Procedure and Brady disclosure requirements.
```
- Final refinements: Adds legal procedural references for authenticity.
- Complete output example: Structured list plus full email draft.


#### Technical Steps
1. Open the [sample email thread](/DOJ/sample%20data/scenario1_email_thread.txt) on discovery coordination and review the contents.
2. Either upload the [sample email file](/DOJ/sample%20data/scenario1_email_thread.txt) to Copilot Chat or copy and paste the thread content into the chat interface.
3. Enter progressive prompts (iterations 1-4) one by one, observing improvements with each iteration.
4. Review Copilot's output (summary and draft response). Note that in a real-world scenario, this output could be used to reply to the actual email thread.
5. Verify tone adjustment for internal vs. external (defense counsel) communications.

#### Facilitation Notes
> 💡 **Tips:**
> - Watch for copy/paste errors between windows.
> - Checkpoint: Ask participants to share one improved action item.
> - Troubleshooting: If output is vague, remind to add DOJ legal context.
> - Explain benefits: Progressive prompts reduce revisions in litigation workflows.

#### Expected Outcomes
- ✅ Deliverable: Summarized thread and drafted email in Outlook.
- ✅ Verification: Output matches legal professional tone and includes court deadlines.
- ✅ Capability demonstration: Clear language generation for legal correspondence.
- ✅ Prompt building: Participants iterate prompts 3-4 times.

#### Discussion Points

**Meta-Prompting**
- Enhance by asking Copilot to refine prompts: "Help me create an effective prompt to summarize discovery coordination emails. What DOJ legal details should I include?"
- Valuable when starting complex tasks like multi-defendant discovery management or privilege log preparation.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Identify key emails, 2) Extract case numbers and deadlines, 3) Generate summary, 4) Draft response."
- Improves quality for detailed litigation support communications.

**When to Use**
- Use complex prompts for high-stakes communications like court filings or formal legal notifications.
- Trade-offs: Simple prompts for quick tasks; complex for accuracy in federal litigation.
- Real-world: Drafting Brady disclosure letters or responding to defense discovery requests.

---

### Scenario 2: Reasoning & Decision Support
**Application:** Word | **DOJ Focus:** Civil Rights Division | **Duration:** 20-25 min

#### Scenario Context
At DOJ Main Justice in Washington D.C., a Trial Attorney (GS-13) drafts legal memoranda and case analysis, while a Senior Trial Attorney reviews briefs for pattern or practice investigations. Use Copilot to structure legal documents and resolve conflicts in legal analysis and recommendations.

#### Copilot Capability Focus
- Primary: Reasoning & Decision Support for legal analysis and recommendations.
- Sub-capabilities: Legal issue identification, precedent analysis, comparative legal arguments.
- Application to DOJ: Aids in efficient legal memorandum development, ensuring alignment with DOJ litigation standards and civil rights enforcement priorities.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Draft a legal memorandum on civil rights violations.
```
- What this prompt does: Generates a generic outline.
- Output example: Basic document structure.
- Limitations: Ignores DOJ specifics like legal memo format or case law requirements.

##### Iteration 2: Add Context
```
Draft a legal memorandum on police misconduct pattern or practice for DOJ Civil Rights Division, including key legal issues and applicable federal statutes.
```
- How context improves output: Adds division focus and legal framework.
- Comparison to iteration 1: Includes realistic legal considerations and statutory citations.

##### Iteration 3: Add Specificity
```
Draft a legal memorandum in standard DOJ format: Include sections for issues presented, legal analysis, case precedents; identify potential litigation challenges; suggest enforcement strategies based on Section 14141 pattern or practice authority.
```
- Why specificity matters: Structures output per DOJ legal memorandum standards.
- Improved output quality: Provides reasoned legal recommendations with case citations.

##### Iteration 4: Final Optimized Prompt
```
As a Trial Attorney in DOJ Civil Rights Division, draft a legal memorandum: Structure with standard DOJ memo format, analyze conflicts between competing legal theories, recommend litigation strategies based on pattern or practice precedents (U.S. v. Ferguson, U.S. v. Cleveland), and suggest evidence requirements for successful enforcement action under 34 U.S.C. § 12601.
```
- Final refinements: Incorporates statutory and case law references.
- Complete output example: Full legal memorandum with analytical framework.


#### Technical Steps
1. Open [sample document](/DOJ/sample%20data/scenario2_training_data.txt) for the legal memorandum.
2. Upload the sample data file or paste sample legal analysis data (e.g., civil rights investigation findings) into Copilot Chat.
3. Input progressive prompts, refining based on outputs.
4. Optional: Copy legal analysis and recommendations into a new Word document.
5. Edit for final formatting, demonstrating legal reasoning application.

#### Facilitation Notes
> 💡 **Tips:**
> - Monitor for prompt overload; break into steps.
> - Checkpoint: Verify legal analysis and case citations in output.
> - Troubleshooting: If recommendations are off, add more statutory or case law context.
> - Explain benefits: Builds logical decision-making in civil rights enforcement.

#### Expected Outcomes
- ✅ Deliverable: Structured legal memorandum in Word with litigation recommendations.
- ✅ Verification: Includes legal analysis, case citations, and enforcement priorities.
- ✅ Capability demonstration: Reasoning for civil rights litigation decisions.
- ✅ Prompt building: 3-4 iterations showing progressive legal logic.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to analyze legal theories for pattern or practice case. What statutory elements should I include?"
- Valuable for developing litigation strategies and enforcement memoranda.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) List investigation findings, 2) Identify applicable statutes, 3) Evaluate precedents, 4) Recommend enforcement action."
- Improves for consent decree drafting and appellate brief preparation.

**When to Use**
- Complex prompts for multi-factor decisions like consent decree negotiations.
- Trade-offs: Simple for case summaries; complex for in-depth legal analysis.
- Real-world: Updating enforcement priorities or preparing technical assistance letters.

---

### Scenario 3: Data Analysis & Visualization
**Application:** Excel | **DOJ Focus:** Executive Office for U.S. Attorneys (EOUSA) | **Duration:** 20-25 min

#### Scenario Context
At DOJ EOUSA headquarters, a Management Analyst (GS-11) tracks district resource allocation and caseload statistics, while a District Administrator (GS-14) analyzes prosecutorial workload data. Use Copilot to interpret district performance metrics and budget allocation.

#### Copilot Capability Focus
- Primary: Data Analysis & Visualization for insights and chart suggestions.
- Sub-capabilities: Pattern detection, resource bottleneck identification, caseload trend analysis.
- Application to DOJ: Enhances prosecutorial resource accountability and operational efficiency across 94 U.S. Attorneys' Offices.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Analyze this district caseload data.
```
- What this prompt does: Gives basic summary.
- Output example: Average case filings per district.
- Limitations: No patterns or visuals.

##### Iteration 2: Add Context
```
Analyze this U.S. Attorneys' Office caseload data across districts, including case type distributions and resource allocation per AUSA.
```
- How context improves output: Ties to DOJ district operations.
- Comparison to iteration 1: Identifies specific issues like prosecutorial staffing gaps.

##### Iteration 3: Add Specificity
```
Analyze this data: Identify patterns in caseload trends by district, calculate prosecutor-to-case ratios, suggest visualizations like bar charts for resource allocation disparities and staffing needs.
```
- Why specificity matters: Directs to actionable budgetary insights.
- Improved output quality: Includes chart types and resource explanations.

##### Iteration 4: Final Optimized Prompt
```
As a District Administrator at EOUSA, analyze this caseload and staffing data: Detect patterns in prosecutorial workload across districts, provide insights on resource allocation needs for criminal vs civil divisions, recommend Excel visualizations (e.g., stacked bar charts, trend lines) for DAG briefings and budget justifications.
```
- Final refinements: Adds leadership briefing context.
- Complete output example: Insights plus chart descriptions for budgetary decision-making.


#### Technical Steps
1. Open Excel with [sample district caseload dataset](/DOJ/sample%20data/scenario3_equipment_readiness.csv) and review the data.
2. Create a table in Excel: Select the data range, then click **Insert > Table** (or press Ctrl+T) and confirm the range includes headers.
3. **Option A - Copy/Paste:** Copy the table data range and paste into Copilot Chat.
   **Option B - Drag/Drop:** First save the file as an Excel workbook (.xlsx) with **File > Save As**, then drag and drop the .xlsx file into Copilot Chat.
4. Use progressive prompts to generate insights.
5. Copy suggestions back to Excel to create charts.
6. Verify patterns match data and prosecutorial resource allocation.

#### Facilitation Notes
> 💡 **Tips:**
> - Ensure data is pasted accurately.
> - Checkpoint: Participants create one recommended chart.
> - Troubleshooting: If insights miss, add row/column details for districts or case types.
> - Explain benefits: Visuals aid quick prosecutorial resource decisions.

#### Expected Outcomes
- ✅ Deliverable: Analyzed data with charts in Excel.
- ✅ Verification: Insights highlight prosecutorial staffing gaps and caseload trends.
- ✅ Capability demonstration: Data interpretation for district resource management.
- ✅ Prompt building: Iterations refine analysis depth.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to analyze district caseload data. What metrics to include?"
- Valuable for EOUSA budget execution and staffing reports.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Calculate prosecutor-to-case ratios, 2) Spot caseload patterns, 3) Identify resource causes, 4) Suggest visuals."
- Improves for district resource planning and budget justifications.

**When to Use**
- Complex prompts for trend analysis across 94 districts.
- Trade-offs: Simple for summaries; complex for comparative visuals.
- Real-world: Annual EOUSA resource allocation reviews and DAG budget briefings.

---

### Scenario 4: Automation & Orchestration
**Application:** Power Automate | **DOJ Focus:** Case Management Systems | **Duration:** 20-25 min

#### Scenario Context
At a U.S. Attorney's Office, a Paralegal Specialist (GS-9) processes case filing requests, while a Litigation Technology Specialist (GS-12) designs workflow improvements. Use Copilot to build automations for case intake and PACER filing workflows.

#### Copilot Capability Focus
- Primary: Automation & Orchestration for workflow design.
- Sub-capabilities: Logic optimization, decision branching, case routing troubleshooting.
- Application to DOJ: Streamlines case management and electronic filing in federal courts.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Design a workflow for case filing requests.
```
- What this prompt does: Basic flow outline.
- Output example: Simple steps.
- Limitations: No DOJ specifics.

##### Iteration 2: Add Context
```
Design a workflow for U.S. Attorney's Office case intake requests, including routing to Criminal or Civil Division AUSAs.
```
- How context improves output: Adds prosecutorial environment elements.
- Comparison to iteration 1: Includes division-specific notification protocols.

##### Iteration 3: Add Specificity
```
Design a Power Automate flow: Trigger on new case referral submission, route based on case type (criminal/civil), send notifications to assigned AUSA, track filing deadlines.
```
- Why specificity matters: Defines triggers and actions for case management.
- Improved output quality: Step-by-step logic with deadline tracking.

##### Iteration 4: Final Optimized Prompt
```
As a Paralegal Specialist at a U.S. Attorney's Office, design a Power Automate flow for case intake: Trigger on email referral, branch logic for criminal vs civil cases, optimize for compliance with LION case management requirements, troubleshoot potential errors in PACER filing workflows.
```
- Final refinements: Adds LION and PACER compliance references.
- Complete output example: Full flow description for prosecutorial workflows.


#### Technical Steps
1. Open Power Automate and start a new flow.
2. Upload or paste [case intake sample data](/DOJ/sample%20data/scenario4_helpdesk_tickets.csv) into Copilot Chat.
3. Use prompts to generate flow logic and step-by-step pseudocode (Copilot does not directly automate Power Automate flows; users must implement logic manually).
4. Copy Copilot's suggested steps to Power Automate and build the flow.
5. Test basic automation with case routing logic.

#### Facilitation Notes
> 💡 **Tips:**
> - Guide on flow connectors and SharePoint integration.
> - Checkpoint: Verify branching logic for criminal vs civil routing.
> - Troubleshooting: If logic fails, refine prompt with case type errors.
> - Explain benefits: Reduces manual case intake tasks and filing delays.

#### Expected Outcomes
- ✅ Deliverable: Working flow in Power Automate.
- ✅ Verification: Routes case referrals correctly by division.
- ✅ Capability demonstration: Orchestration for case management processes.
- ✅ Prompt building: Iterations optimize automation.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to design case intake workflows. What decision branches to include?"
- Valuable for LION and PACER filing automation.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Define trigger, 2) Add conditions, 3) Set actions, 4) Test logic."
- Improves for case management efficiency.

**When to Use**
- Complex prompts for branched flows with multiple approval levels.
- Trade-offs: Simple for basics; complex for optimization.
- Real-world: Grand jury subpoena processing and discovery management automation.

---

### Scenario 5: Search & Retrieval
**Application:** Power BI | **DOJ Focus:** Legal Research & Case Files | **Duration:** 20-25 min

#### Scenario Context
At a U.S. Attorney's Office, a Legal Research Specialist (GS-11) compiles case law and precedents, while an AUSA (GS-14) organizes trial preparation materials. Use Copilot to extract information from case databases and legal research platforms for trial briefs.

#### Copilot Capability Focus
- Primary: Search & Retrieval for data extraction.
- Sub-capabilities: Case law organization, key precedent consolidation, legal issue identification.
- Application to DOS: Supports analytical reporting and situational awareness without classified access.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Find key legal precedents in this data.
```
- What this prompt does: Lists basic case names.
- Output example: Unstructured list.
- Limitations: No organization by legal issue.

##### Iteration 2: Add Context
```
Find specific legal precedents from this case law database for a criminal RICO prosecution, focusing on enterprise elements and predicate acts.
```
- How context improves output: Ties to DOJ prosecutorial work.
- Comparison to iteration 1: Groups by RICO elements.

##### Iteration 3: Add Specificity
```
Extract case precedents: Organize into categories (e.g., enterprise definition, pattern of racketeering, forfeiture), include circuit splits and key holdings, create a structured trial brief outline.
```
- Why specificity matters: Formats for easy use in litigation.
- Improved output quality: Tabular extraction with holdings.

##### Iteration 4: Final Optimized Prompt
```
As an AUSA preparing for RICO trial, search this case database: Retrieve key precedents on enterprise elements, organize by circuit and relevance, extract critical holdings for trial brief per DOJ Criminal Resource Manual standards.
```
- Final refinements: Adds circuit analysis and DOJ manual references.
- Complete output example: Structured case law summary.


#### Technical Steps
1. Open Power BI with [sample case law dataset](/DOJ/sample%20data/scenario5_intelligence_data.csv).
2. Copy case metrics or precedent summaries into Copilot Chat (Copilot does not directly extract data from Power BI dashboards; users must manually describe or export data).
3. Use prompts to extract and organize legal precedents.
4. Copy organized output back to Power BI notes or Word trial brief.
5. Verify extraction accuracy and case citations.

#### Facilitation Notes
> 💡 **Tips:**
> - Describe case holdings if not copyable.
> - Checkpoint: Check organized precedents by legal issue.
> - Troubleshooting: Add more circuit or case details if missed.
> - Explain benefits: Speeds legal research consolidation.

#### Expected Outcomes
- ✅ Deliverable: Extracted case law summary for trial brief.
- ✅ Verification: Includes key precedents with holdings.
- ✅ Capability demonstration: Retrieval for legal research tasks.
- ✅ Prompt building: Iterations enhance case organization.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt to extract case law precedents. What legal elements to include?"
- Valuable for trial briefs and appellate arguments.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Scan cases, 2) Identify holdings, 3) Categorize by element, 4) Organize brief."
- Improves for litigation preparation and legal research memoranda.

**When to Use**
- Complex prompts for large case databases across multiple circuits.
- Trade-offs: Simple for quick finds; complex for structured legal analysis.
- Real-world: Trial preparation research or appellate brief drafting.

---

### Scenario 6: Personalization & Context Awareness
**Application:** Teams | **DOJ Focus:** Executive Leadership | **Duration:** 20-25 min

#### Scenario Context
At DOJ Main Justice, a Confidential Assistant (GS-11) uses a Teams meeting transcript to summarize senior leadership meetings, while a Deputy Assistant Attorney General (SES) generates agendas. Use Copilot to adapt communications to rank and role in DOJ executive coordination.

#### Copilot Capability Focus
- Primary: Personalization & Context Awareness for adaptive content.
- Sub-capabilities: Terminology adjustment, role-specific suggestions, organizational hierarchy awareness.
- Application to DOJ: Ensures appropriate language in executive communications and component coordination.

#### Progressive Prompt Building

##### Iteration 1: Basic Prompt
```
Summarize this meeting notes.
```
- What this prompt does: General overview.
- Output example: Plain summary.
- Limitations: No DOS adaptation.

##### Iteration 2: Add Context
```
Summarize these senior leadership meeting notes from DOJ Main Justice, including key enforcement decisions and policy action items.
```
- How context improves output: Adds organizational and legal focus.
- Comparison to iteration 1: Mentions component responsibilities vaguely.

##### Iteration 3: Add Specificity
```
Summarize notes: Use DOJ legal terminology, adapt language for Assistant Attorney Generals and DAAG, generate follow-up messages aligned with organizational hierarchy.
```
- Why specificity matters: Personalizes tone for executive leadership.
- Improved output quality: Role-appropriate phrasing for SES-level recipients.

##### Iteration 4: Final Optimized Prompt
```
As a Confidential Assistant at DOJ Main Justice, summarize senior leadership meeting notes: Incorporate Attorney General priorities, personalize follow-ups by position (e.g., formal for AAG and DAAG), demonstrate context awareness of DOJ organizational structure and component reporting relationships.
```
- Final refinements: Adds AG priority references.
- Complete output example: Adapted summary and executive messages.


#### Technical Steps
1. Open the [sample meeting transcript](/DOJ/sample%20data/scenario6_meeting_transcript.txt) and review.
2. Copy or upload sample meeting transcript into Copilot Chat.
3. Apply progressive prompts for refinements.
4. Paste personalized output back to Teams chat or meeting notes.
5. Check context alignment and hierarchy appropriateness.

#### Facilitation Notes
> 💡 **Tips:**
> - Focus on role and rank sensitivity for SES recipients.
> - Checkpoint: Verify tone in follow-ups to AAG/DAAG.
> - Troubleshooting: Add more DOJ organizational context if generic.
> - Explain benefits: Enhances senior leadership collaboration.

#### Expected Outcomes
- ✅ Deliverable: Personalized summary in Teams.
- ✅ Verification: Adapts to DOJ organizational hierarchy.
- ✅ Capability demonstration: Context-aware generation.
- ✅ Prompt building: Iterations build personalization.

#### Discussion Points

**Meta-Prompting**
- Enhance: "Help me create a prompt for role-appropriate summaries. What DOJ organizational context to include?"
- Valuable for Attorney General-level briefing preparation.

**Chain of Reasoning**
- Apply: "Let's work through this step by step: 1) Review notes, 2) Identify actions, 3) Adapt tone, 4) Generate messages."
- Improves for executive communications and component coordination.

**When to Use**
- Complex prompts for audience-specific legal and executive tasks.
- Trade-offs: Simple for basics; complex for personalization.
- Real-world: Senior leadership meeting coordination or Attorney General action requests.

---

## Quick Reference

### Summary Table of All 6 Scenarios

| Scenario | Capability | Application | DOJ Focus | Duration |
|----------|------------|-------------|------------|----------|
| 1 | Language Understanding & Generation | Outlook | U.S. Attorney's Office - Criminal Division | 20-25 min |
| 2 | Reasoning & Decision Support | Word | Civil Rights Division | 20-25 min |
| 3 | Data Analysis & Visualization | Excel | Executive Office for U.S. Attorneys (EOUSA) | 20-25 min |
| 4 | Automation & Orchestration | Power Automate | Case Management Systems | 20-25 min |
| 5 | Search & Retrieval | Power BI | Legal Research & Case Files | 20-25 min |
| 6 | Personalization & Context Awareness | Teams | Executive Leadership | 20-25 min |

### Progressive Prompt Building Tips
- Start basic, add context, then specificity.
- Use 3-4 iterations to show improvements.
- Include DOJ legal terminology for relevance.

### Key Talking Points for Each Copilot Capability
- Language Understanding: Focus on tone and drafting for consular and diplomatic communications.
- Reasoning: Emphasize decisions and policy frameworks.
- Data Analysis: Highlight insights and visuals for management and budgeting.
- Automation: Stress logic and optimization for IT and administrative processes.
- Search: Prioritize extraction and organization for analytical products.
- Personalization: Adapt to organizational context and diplomatic protocols.

### Meta-Prompting and Chain of Reasoning Quick Reference
- **Meta-Prompting Example:** "Help me build a prompt for [task]. Suggest improvements."
- **Chain of Reasoning Example:** "Step by step: 1) Analyze, 2) Recommend, 3) Output."
- Use when outputs need structure or depth.

### Common Questions with Answers
- Q: Why no web search? A: Government cloud environment restricts external grounding for security.
- Q: How to handle vague outputs? A: Iterate prompts with more diplomatic and contextual details.


### Troubleshooting Common Issues
- Copy/paste fails: Check windows focus.
- File upload fails: Use copy/paste as fallback.
- Generic outputs: Add DOS context and diplomatic terminology.
- App access: Verify licenses (Microsoft 365 E5 + Copilot add-on).


### Additional Learning Resources
- [Microsoft Learn: Copilot Fundamentals](https://learn.microsoft.com/en-us/microsoft-copilot/)
- [Microsoft Learn: Prompt Engineering](https://learn.microsoft.com/en-us/training/modules/engineer-copilot-prompts/)
- [Microsoft Learn: Copilot for Government Cloud](https://learn.microsoft.com/en-us/office365/servicedescriptions/office-365-platform-service-description/microsoft-365-copilot#feature-availability)
- DOS-specific: Internal training modules on M365 and diplomatic communications (if available).