# M365 Copilot — Talent Acquisition
## Participant Prompt Guide | Bajaj Finance Limited | FY2026–27

*Prepared by Technizer Edge Pvt. Ltd. | Participant Copy*

---

> ### 🧩 The Meta Prompt — Use This First
>
> ```
> Act as a Microsoft 365 Copilot prompt expert for HR and Talent Acquisition teams.
>
> I am a [YOUR ROLE] at [COMPANY].
> I need to [WHAT YOU WANT TO DO] using the data file [FILE NAME] shared with you.
> My audience is [WHO WILL READ THIS OUTPUT].
>
> Write me a detailed, structured Copilot Chat prompt I can use to complete this task.
> The prompt must specify: role, task, data context, output format, tone, and any filters.
> ```
>
> **How to use it:** Paste the meta prompt into M365 Copilot Chat → fill in the blanks → Copilot generates your working prompt → paste that prompt back into Copilot Chat with your file attached via `/`

---

## Dataset Sheets — TA_Copilot_Training_Dataset.xlsx

| Sheet | What It Contains | Stage |
|---|---|---|
| Candidate Pipeline | 15 open reqs — stage, volume, TAT, status | Stage 1 |
| TAT & SLA Dashboard | BU-wise TAT vs SLA targets + breach reasons | Stage 2 |
| Source Effectiveness | 10 sourcing channels — conversion % & cost per hire | Stage 3 |
| Offer & Joining Tracker | 15 candidates — offer, DOJ, drop reasons | Stage 4 |
| JD & Interview Bank | JD status + question bank index + Copilot adoption | Stage 5 |

---

## How to Attach Your File in M365 Copilot Chat

1. Upload `TA_Copilot_Training_Dataset.xlsx` to your OneDrive
2. Open M365 Copilot Chat at `microsoft365.com/chat` or in Microsoft Teams
3. Type `/` in the chat box and select the file from OneDrive
4. Paste your working prompt and press Enter

---

---

## Stage 1 — Pipeline Health Check & At-Risk Flags

**Sheet:** Candidate Pipeline | **Output:** Summary + at-risk requisition table

### Step 1 — Paste this Meta Prompt into Copilot Chat

```
Act as a Microsoft 365 Copilot prompt expert for HR and Talent Acquisition teams.

I am a Talent Acquisition Lead at Bajaj Finance Limited.
I need to review the current hiring pipeline, identify at-risk requisitions, and prepare
a concise summary for the weekly leadership call using the file TA_Copilot_Training_Dataset.xlsx.
My audience is the TA Head and Business HR Partners.

Write me a detailed, structured Copilot Chat prompt I can use to complete this task.
The prompt must specify: role, task, data context, output format, tone, and any filters.
```

### Step 2 — Copilot generates this. Paste it back with your file attached.

```
You are a senior Talent Acquisition analyst at Bajaj Finance Limited.

Using the "Candidate Pipeline" sheet in the attached file:

1. Summarise total open requisitions by status (Active, On Hold, Draft, Closed)
2. Identify requisitions where TAT (Days) exceeds 40 days and flag them as "At Risk"
3. Highlight roles stuck in early stages (L1 Interview or earlier) for more than 30 days
4. Provide a 5-bullet executive summary suitable for a leadership call

Format: One-paragraph overview → At-Risk table (Req ID | Role | BU | Stage | TAT | Flag)
→ 5 action-oriented bullet points.
Tone: Professional, concise, data-driven.
```

---

## Stage 2 — SLA Breach Analysis & Root Cause Narrative

**Sheet:** TAT & SLA Dashboard | **Output:** Breach themes + 30-day action plan

### Step 1 — Paste this Meta Prompt into Copilot Chat

```
Act as a Microsoft 365 Copilot prompt expert for HR and Talent Acquisition teams.

I am the Head of Talent Acquisition at Bajaj Finance Limited.
I need to analyse hiring TAT performance across all Business Units, identify which BUs
are breaching SLA targets, surface root causes, and recommend corrective actions.
The data is in the file TA_Copilot_Training_Dataset.xlsx.
My audience is the CHRO and senior HR leadership team.

Write me a detailed, structured Copilot Chat prompt to complete this task.
The prompt must specify: role, task, data context, output format, tone, and any filters.
```

### Step 2 — Copilot generates this. Paste it back with your file attached.

```
You are a TA Operations Analyst at Bajaj Finance Limited.

Using the "TAT & SLA Dashboard" sheet in the attached file:

1. List all Business Units where SLA % Met is below 70% — label these "Critical"
2. List BUs between 70–85% — label these "Watch"
3. For Critical BUs, extract the "Top Delay Reason" and identify patterns
4. Draft a structured root cause summary: group delay reasons into 3–4 themes
5. Recommend 3 specific interventions the TA Head should prioritise in the next 30 days

Format: Section 1 — BU Performance Table (BU | TAT | SLA Target | SLA % | Flag)
Section 2 — Root Cause Themes (theme + contributing BUs + description)
Section 3 — 30-Day Action Plan (numbered, owner suggested)
Tone: Analytical, strategic, ready for senior leadership consumption.
```

---

## Stage 3 — Sourcing ROI & Channel Recommendation

**Sheet:** Source Effectiveness | **Output:** Channel ranking + Q2 budget recommendation

### Step 1 — Paste this Meta Prompt into Copilot Chat

```
Act as a Microsoft 365 Copilot prompt expert for HR and Talent Acquisition teams.

I am a Talent Acquisition Lead at Bajaj Finance Limited responsible for sourcing strategy.
I need to evaluate the performance of our sourcing channels using Q1 data,
identify the highest ROI channels, and build a recommendation for Q2 budget reallocation.
The data is in the file TA_Copilot_Training_Dataset.xlsx.
My audience is the TA Head and Finance Business Partner.

Write me a detailed, structured Copilot Chat prompt to complete this task.
The prompt must specify: role, task, data context, output format, tone, and any filters.
```

### Step 2 — Copilot generates this. Paste it back with your file attached.

```
You are a Talent Acquisition Sourcing Strategist at Bajaj Finance Limited.

Using the "Source Effectiveness" sheet in the attached file:

1. Rank all sourcing channels by Joining Conversion % (Joined ÷ Applications) highest to lowest
2. Create a 2×2 summary: High Conversion + Low Cost (Invest), High Conversion + High Cost (Optimise),
   Low Conversion + Low Cost (Test), Low Conversion + High Cost (Exit)
3. Identify the top 3 channels to increase investment in Q2 with supporting data
4. Identify the bottom 2 channels and build a case to reduce or exit them
5. Draft a 3-sentence budget reallocation recommendation for the TA Head

Format: Ranked channel table → 2×2 matrix → Top 3 invest channels (data-backed)
→ Bottom 2 exit channels → Final recommendation paragraph.
Tone: Analytical, confident, numbers-backed.
```

---

## Stage 4 — Offer Drop Analysis & Retention Action

**Sheet:** Offer & Joining Tracker | **Output:** Drop patterns + Q2 action plan

### Step 1 — Paste this Meta Prompt into Copilot Chat

```
Act as a Microsoft 365 Copilot prompt expert for HR and Talent Acquisition teams.

I am a Talent Acquisition Specialist at Bajaj Finance Limited.
I need to analyse our Q1 offer and joining data, identify patterns in offer declines and
no-show candidates, understand the key reasons for drops, and build an action plan
to improve our offer-to-joining ratio in Q2.
The data is in the file TA_Copilot_Training_Dataset.xlsx.
My audience is the TA Head and Business HR Partners.

Write me a detailed, structured Copilot Chat prompt to complete this task.
The prompt must specify: role, task, data context, output format, tone, and any filters.
```

### Step 2 — Copilot generates this. Paste it back with your file attached.

```
You are a TA Insights Analyst at Bajaj Finance Limited.

Using the "Offer & Joining Tracker" sheet in the attached file:

1. Calculate: Total offers made, offers accepted, candidates joined, and offer-to-join %
2. List all candidates who accepted offers but did not join — extract their Drop Reason
3. Group drop reasons into themes (Counter Offer, Personal Reasons, Salary Gap, Role Mismatch)
4. Identify which roles, BUs, and recruiters have the highest drop rates
5. Draft 4 specific actions the TA team can take before Q2 to reduce drops

Format: Section 1 — Offer funnel metrics (table) | Section 2 — Drop pattern analysis
(theme + count + example roles) | Section 3 — Risk factors (BU, role level, recruiter)
| Section 4 — Q2 Action Plan (4 bullets, owner suggested)
Tone: Practical, solution-focused, ready for HRBP discussion.
```

---

## Stage 5 — JD Gap Assessment & Copilot Adoption Report

**Sheet:** JD & Interview Bank | **Output:** Gap report + recommendations for CHRO

### Step 1 — Paste this Meta Prompt into Copilot Chat

```
Act as a Microsoft 365 Copilot prompt expert for HR and Talent Acquisition teams.

I am the Head of Talent Acquisition at Bajaj Finance Limited.
I need to assess the completeness of our JD library and interview question bank,
identify gaps that may be affecting hiring quality, and check which roles and HRBPs
have adopted Copilot in their TA workflow.
The data is in the file TA_Copilot_Training_Dataset.xlsx.
My audience is the TA Head and CHRO for a quarterly review.

Write me a detailed, structured Copilot Chat prompt to complete this task.
The prompt must specify: role, task, data context, output format, tone, and any filters.
```

### Step 2 — Copilot generates this. Paste it back with your file attached.

```
You are a TA Quality & Process Analyst at Bajaj Finance Limited.

Using the "JD & Interview Bank" sheet in the attached file:

1. List all roles where JD Status is "Draft" — gaps that could delay time-to-hire
2. List roles with 0 interview questions — flag as "Interview Not Ready"
3. Calculate: % of roles using Copilot for JD/prompt creation (Copilot Prompt Used = Yes)
4. Identify which HRBPs have the highest and lowest Copilot adoption
5. Draft a 3-point recommendation for the CHRO on closing JD and interview readiness gaps

Format: Gap Summary Table (Role | JD Status | No. of Qs | Copilot Used | HRBP Owner)
→ Copilot Adoption Summary (% overall, breakdown by HRBP)
→ 3 Recommendations for CHRO (concise, numbered)
Tone: Strategic, quality-focused, suitable for quarterly review.
```

---

## Bonus — JD & Interview Question Generator

**No file needed | Output:** Full JD + 15-question competency bank

### Step 1 — Paste this Meta Prompt into Copilot Chat

```
Act as a Microsoft 365 Copilot prompt expert for HR and Talent Acquisition teams.

I am a Talent Acquisition Specialist at Bajaj Finance Limited.
I need to create a complete Job Description and a 15-question competency-based
interview question bank for the role of Data Scientist in our Risk Analytics team.
The JD should reflect our company values: customer centricity, integrity, and ownership.
My audience is hiring managers and the final interview panel.

Write me a detailed, structured Copilot Chat prompt to generate both outputs.
The prompt must specify: role, task, context, output format, tone, and structure.
```

### Step 2 — Copilot generates this. Paste it directly into Copilot Chat.

```
You are a Senior HR Content Specialist at Bajaj Finance Limited.

Create the following for the role of Data Scientist — Risk Analytics:

PART 1 — Job Description
Structure: Role Overview | Key Responsibilities (8 bullets) | Required Skills (technical + soft)
| Preferred Qualifications | What We Offer | About Bajaj Finance
Tone: Professional, direct, candidate-friendly. Reflect values: Customer Centricity, Integrity, Ownership.

PART 2 — Interview Question Bank (15 questions)
Organise by competency:
- Technical (Python, ML, SQL): 5 questions with evaluation criteria
- Analytical Thinking: 3 behavioural questions (STAR format prompts)
- Communication & Stakeholder Mgmt: 3 questions
- Culture & Values Fit: 2 questions aligned to BFL values
- Role-Specific Scenario: 2 case questions

Format each question as: Q → Competency → What Good Looks Like (2 lines)
```

---

## RTCFT — Prompt Formula Quick Reference

| Letter | Stands For | Example for Talent Acquisition |
|---|---|---|
| **R** | Role | "You are a Talent Acquisition Lead at Bajaj Finance" |
| **T** | Task | "Analyse the sourcing data and rank channels by conversion" |
| **C** | Context | "Using the Source Effectiveness sheet in the attached Excel file" |
| **F** | Format | "Ranked table → 2×2 matrix → Recommendation paragraph" |
| **T** | Tone | "Data-driven, concise, suitable for TA Head review" |

---

*M365 Copilot for HR Teams — Talent Acquisition Track | FY2026–27*
*Technizer Edge Pvt. Ltd. | Participant Copy*
