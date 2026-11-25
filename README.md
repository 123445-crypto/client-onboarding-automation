# Client Intake, Proposal & Onboarding Automation

An end-to-end client automation system built in *Make* that captures new client requests, generates project scope and proposal materials, tracks leads in Airtable, and handles post-approval onboarding automatically.

## Tools Used
- *Make* (workflow automation)
- *Tally* (client intake form)
- *Google Gemini AI* (scope / proposal generation)
- *Airtable* (client database & status tracking)
- *Google Docs* (proposal document creation)
- *Gmail* (proposal delivery, approval reply trigger & onboarding welcome email)
- *ClickUp* (onboarding / project task creation)
- *Slack* (team notifications)

## How It Works

### 1. Client Intake & Proposal Workflow
1. *Tally:* A client submits project details through the intake form.
2. *Google Gemini AI:* Processes the submission to generate structured project scope/proposal content.
3. *Airtable:* Logs a new client record with intake details and generated information.
4. *Google Docs:* Creates/populates a proposal document for the client.
5. *Gmail:* Sends the proposal email to the client so they can review and reply *APPROVED*.

### 2. Post-Approval Onboarding Workflow
1. *Gmail (Watch Emails):* Detects incoming email replies (such as *APPROVED*).
2. *Airtable (Search Records):* Looks up the matching client record by email address.
3. *ClickUp:* Creates an onboarding/project task with the client's details and scope.
4. *Gmail:* Sends a welcome/onboarding email with next steps.
5. *Slack:* Posts an onboarding update to the team channel.

## Key Highlights & Troubleshooting
- Built and tested end-to-end across both scenarios using live test runs and execution log checks.
- Resolved Airtable record lookup formula syntax issues ({Email}='...') and managed Make active-scenario limits cleanly during testing.
-
