# M365 Copilot — Employee Attrition Analysis
## Participant Lab Guide
### Bajaj Finance Limited | HRBP Training Session | FY 2026-27
**Technizer Edge Pvt. Ltd. | M365 Copilot Training Series**

---

## 👋 Welcome

This guide is your hands-on companion for today's session. You will use **M365 Copilot Chat** to analyse real employee attrition data — identifying patterns, flagging at-risk employees, and generating leadership-ready outputs — all without writing a single formula or pivot table.

By the end of this session, you will be able to:

- Use the **Meta Prompt** framework to generate powerful, ready-to-use Copilot prompts
- Analyse attrition patterns by department, grade, and month
- Identify at-risk employees and generate prioritised intervention plans
- Produce an executive briefing directly from your data

---

## 🖥️ How to Use Copilot Chat Today

1. Open your browser and go to **microsoft365.com/chat** — or open **Teams** and click the Copilot icon
2. To attach the Excel file, type `/` in the Copilot chat box → select `BFL_Employee_Attrition_Data.xlsx` from OneDrive
3. Paste the prompt from this guide → press Enter
4. Read the output, then try the **Your Turn** exercise at the end of each stage

> **Keep this file open throughout the session.** Every prompt you need is already written here — you just copy, paste, and run.

---

## 🗂️ Your Dataset — `BFL_Employee_Attrition_Data.xlsx`

Before you begin, take 2 minutes to open the Excel file and familiarise yourself with its 5 sheets:

| Sheet | What It Contains |
|---|---|
| **Employee Attrition Data** | 150 employee records — grade, dept, location, engagement score, tenure, exit reason, risk flag |
| **Attrition Dashboard** | Dept-wise and grade-wise attrition %, engagement average, top exit reason |
| **Monthly Trend & Exit Reasons** | 12-month attrition trend (Apr 2025–Mar 2026) + 9 exit reasons ranked |
| **High Risk – Active Employees** | 15 flagged active employees with recommended HR actions |
| **HRBP Scorecard** | KPI summary, risk indicators, and 5-point action plan |

---

## ⚡ The Meta Prompt — Your Master Framework

This is the **one prompt** you use to generate any Copilot working prompt. You fill in four things — Copilot writes the rest.

```
Act as a Microsoft Copilot prompt expert.

I am a [YOUR ROLE] at [COMPANY/CONTEXT].
I need to [WHAT YOU WANT TO DO].
My audience is [WHO WILL READ OR ACT ON THE OUTPUT].
The data I have is [BRIEF DESCRIPTION OF INPUT DATA].

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

### How it works — two steps, every time:

**Step 1** → Paste the Meta Prompt into Copilot Chat → Copilot generates a working prompt

**Step 2** → Attach your Excel file using `/` → Paste the working prompt → Get your output

> You will use this two-step rhythm for all 5 exercises today.

---

## 🃏 RTCFT — Quick Reference

Use this to fill in the Meta Prompt blanks quickly:

| Element | What to Fill In | Example |
|---|---|---|
| **R**ole | Your job title + company | HRBP at Bajaj Finance Limited |
| **T**ask | What you need to do | Analyse attrition by department and grade |
| **C**ontext | Why you need it / who it's for | For CHRO monthly review meeting |
| **F**ormat | How you want the output to look | Table + 3 bullet insights |
| **T**one | Register / style | Professional, executive-ready |

---

## 🎯 LAB EXERCISES — 5 STAGES

---

## Stage 1 — Discovering What Copilot Can Do With Attrition Data

**What you'll learn:** How the Meta Prompt works and how Copilot can suggest analysis options you hadn't thought of.

### Step 1 — Paste this Meta Prompt into Copilot Chat

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP at Bajaj Finance Limited.
I need to understand what kinds of HR analysis I can run on an employee attrition dataset.
My audience is myself — I want to explore what's possible before I start.
The data I have is an Excel file with 150 employee records including grade, department,
location, engagement scores, tenure, performance ratings, exit reasons, and a risk flag
for active employees.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

### Step 2 — What to Expect

Copilot will return a ready-to-use working prompt covering:
- Your role and context as an HRBP
- A list of 8–12 analysis options (trend, dept, grade, engagement, tenure, exit reason, risk)
- Suggested output format and tone

### ✏️ Your Turn

Adapt the Meta Prompt for your own context. Change the role, goal, or data description and run it again. Try:

> *"I am an HR Manager at [your company]. I need to understand what analysis I can run to reduce attrition in my Sales team..."*

---

## Stage 2 — Analysing Attrition by Department and Grade

**What you'll learn:** How to get Copilot to surface attrition patterns across departments and grades — and compare engagement scores between people who left vs. those who stayed.

### Step 1 — Paste this Meta Prompt

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP at Bajaj Finance Limited.
I need to analyse which departments and employee grades have the highest attrition rates,
and understand whether engagement scores are driving the attrition.
My audience is the Chief People Officer — they want a crisp summary with numbers.
The data I have is an Excel file with 150 employee records including grade, department,
engagement score, and a status column showing 'Attrited' or 'Active'.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

### Step 2 — Apply the Working Prompt

Attach `/BFL_Employee_Attrition_Data.xlsx` in Copilot Chat, then paste the prompt Copilot generated above — or use this ready-to-use version:

```
You are an HR Analytics expert supporting an HRBP at Bajaj Finance Limited.

Analyse the attached employee attrition dataset (Sheet: Employee Attrition Data, 150 rows).

Tasks:
1. Calculate attrition rate by Department. Rank departments from highest to lowest attrition %.
2. Calculate attrition rate by Grade (M1 to M5). Note which grade has the highest risk.
3. For each department with attrition > 25%, show the average Engagement Score of
   Attrited vs. Active employees side by side.
4. Identify the top 2 departments where low engagement is the strongest predictor of attrition.

Output format: Structured table with department/grade, headcount, attrited count,
attrition %, and engagement average. Follow with 3 bullet-point insights for the CPO.
Tone: Analytical, precise, executive-ready.
```

### ✏️ Your Turn

After seeing the output, try this follow-up prompt in the same Copilot chat:

> *"Now filter this analysis for only M1 and M2 grade employees. Which department should the HRBP prioritise first?"*

---

## Stage 3 — Spotting Monthly Trends and Exit Reason Patterns

**What you'll learn:** How to read 12-month attrition trends and identify whether exit reasons are systemic (HR can fix them) or market-driven (need a different strategy).

### Step 1 — Paste this Meta Prompt

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP at Bajaj Finance Limited.
I need to identify seasonal attrition trends over 12 months and understand which exit reasons
are most common — so I can recommend HR interventions at the right time of year.
My audience is the HR Head and Department Heads in a monthly review meeting.
The data I have is an Excel file with monthly attrition counts (Apr 2025 to Mar 2026),
engagement averages per month, and a breakdown of 9 exit reasons with counts and percentages.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

### Step 2 — Apply the Working Prompt

Attach the file and paste the prompt Copilot generated — or use this version:

```
You are an HR Analytics expert at Bajaj Finance Limited.

Analyse the attached Excel file using two sheets:
- Sheet "Monthly Trend & Exit Reasons" — rows 3 to 15 (monthly data Apr 2025–Mar 2026)
- Same sheet — rows 20 to 30 (exit reason breakdown)

Tasks:
1. Identify the 3 months with highest attrition. What pattern do you observe
   (post-appraisal, year-end, mid-year)?
2. Compare attrition rate vs. engagement score month by month. Do low engagement months
   predict high attrition the following month?
3. List the top 3 exit reasons by count. For each, identify which grade and department
   is most affected.
4. Flag each exit reason as either a Systemic Issue (e.g., Toxic Manager, No Growth)
   or a Market Issue (e.g., Better Opportunity, Higher Salary).

Output format: Monthly trend narrative (3–4 sentences), followed by an exit reason table
(Reason | Count | Grade | Dept | Issue Type). End with 3 HRBP recommendations.
Tone: Insightful, action-ready, suitable for a leadership review meeting.
```

### ✏️ Your Turn

Try this follow-up:

> *"Based on the exit reasons classified as Systemic Issues, write 2 specific HR policy changes Bajaj Finance should consider implementing in Q1 FY27."*

---

## Stage 4 — Identifying and Prioritising At-Risk Employees

**What you'll learn:** How to use Copilot to rank employees by intervention urgency using weighted criteria — and generate specific, personalised action plans for each.

### Step 1 — Paste this Meta Prompt

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP at Bajaj Finance Limited.
I need to prioritise which at-risk active employees need immediate HR intervention
and generate a recommended action for each — so my team can act this week.
My audience is the HRBP team lead and business HR partners.
The data I have is an Excel file with 15 high-risk active employees showing their
engagement score, absenteeism, performance rating, tenure, promotions, risk level,
and a suggested action column.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

### Step 2 — Apply the Working Prompt

```
You are an HR Business Partner advisor at Bajaj Finance Limited.

Read the sheet "High Risk - Active Employees" in the attached Excel file (15 employees).

Tasks:
1. Rank the 15 employees by urgency of intervention. Use:
   Engagement Score (weight 40%), Absenteeism Days (weight 30%), No Promotion flag (weight 30%).
2. Group them into 3 intervention tiers:
   - Immediate Action (this week)
   - Scheduled Action (next 2 weeks)
   - Monitor & Check-in (30 days)
3. For the top 5 Immediate Action cases, suggest a specific HR intervention —
   not generic. Reference their grade, department, and tenure in each suggestion.
4. Identify if any 2 employees are in the same department — flag as potential team culture risk.

Output format: Tiered priority table with Emp ID, Name, Grade, Dept, Engagement Score,
Urgency Tier, and Action. Follow with the top 5 individual action plans (3 lines each).
Tone: Practical, empathetic, time-sensitive.
```

### ✏️ Your Turn

After reviewing the output, try adjusting the weights:

> *"Re-run the prioritisation with Engagement Score at 50% weight and Absenteeism at 50%. Does the top 5 list change? Which employees move up or down?"*

---

## Stage 5 — Generating the HRBP Executive Brief for Leadership

**What you'll learn:** How to use Copilot to produce a structured, C-suite-ready attrition briefing directly from your scorecard data — in one prompt.

### Step 1 — Paste this Meta Prompt

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP at Bajaj Finance Limited.
I need to prepare an executive briefing on FY 2026-27 attrition for the CHRO and
CPO — covering headline numbers, root causes, business impact, and a 5-point action plan.
My audience is the CHRO, CPO, and two Department Heads — they have 10 minutes for this.
The data I have is an Excel file with a 5-sheet HRBP scorecard covering KPI metrics,
risk indicators, and top action items already structured.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

### Step 2 — Apply the Working Prompt

```
You are a strategic HR advisor preparing a CHRO briefing at Bajaj Finance Limited.

Read the sheet "HRBP Scorecard" in the attached Excel file.

Write an executive attrition briefing with the following structure:

1. SITUATION (2–3 sentences): Overall attrition rate, voluntary vs. involuntary split,
   estimated cost to the organisation.
2. ROOT CAUSES (3 bullets): Top 3 drivers of attrition with the department or grade
   most affected.
3. RISK SPOTLIGHT (2 bullets): Current high-risk active employees — number at risk,
   which departments have clusters.
4. FINANCIAL IMPACT: Estimated cost of attrition (replacement cost × exits).
   Express as ₹ Crore.
5. 5-POINT ACTION PLAN: One action per bullet. Specific. Owner implied by dept.
   Timeline: Q1 FY27 or Q2 FY27.
6. CLOSING STATEMENT (1 sentence): What success looks like if actions are implemented.

Format: Professional business briefing. Use section headers. No bullet overload.
Tone: Confident, data-backed, solution-focused. Suitable for C-suite, 10-minute slot.
```

### ✏️ Your Turn

Try customising the output:

> *"Rewrite the executive briefing in a shorter format — 200 words maximum — suitable for a WhatsApp message to the CHRO before the meeting."*

---

## 🎁 Bonus Exercise — Writing a Retention Email to a Department Head

**What you'll practise:** Using the Meta Prompt for a communication task — not just analysis. This works exactly the same way.

### Meta Prompt

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP at Bajaj Finance Limited.
I need to write an email to the Head of Technology informing them of high attrition
in their team and requesting a 30-minute meeting to discuss a retention plan.
My audience is a senior business leader — they are data-driven and don't appreciate
vague HR communication.
The data I have is the attrition analysis showing Technology has 30% attrition,
the highest in the organisation, driven primarily by Startup Opportunities and Salary.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

### ✏️ Your Turn

Adapt this for your own team or department. Change the department name, the attrition driver, and the audience — run the meta prompt and see what Copilot generates.

---

## 📝 Session Reflection

Before you leave today, take 5 minutes to answer these in your notes:

1. Which stage produced the most useful output for your day-to-day work?
2. Which Meta Prompt would you use first, back at your desk next week?
3. Write one custom Meta Prompt for a real HR task you currently handle:

```
Act as a Microsoft Copilot prompt expert.

I am a _________________________________ at Bajaj Finance Limited.
I need to _________________________________.
My audience is _________________________________.
The data I have is _________________________________.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

---

## 🔧 Quick Troubleshooting

| Situation | What to Do |
|---|---|
| Copilot output is too long | Add: *"Summarise this in 5 bullet points"* |
| Output format is wrong | Add: *"Restructure this as a table with columns: Dept, Attrition %, Insight"* |
| Numbers look wrong | Add: *"Double-check your calculation for [Department] and show me how you got the %"* |
| Need a different tone | Add: *"Rewrite this in a more casual tone suitable for a team meeting"* |
| Want to try a different angle | Add: *"Now repeat this analysis only for M1 and M2 grade employees"* |

---

## 📎 Reference — How to Attach a File in Copilot Chat

1. Open M365 Copilot Chat at **microsoft365.com/chat** or in **Microsoft Teams**
2. In the message box, type `/`
3. A file picker appears — select `BFL_Employee_Attrition_Data.xlsx` from your OneDrive
4. The file name appears as a chip above your message — this confirms it's attached
5. Type or paste your prompt → press **Enter**

> Copilot reads the attached file fresh with every new message. You do not need to re-attach unless you start a new conversation.

---

*Technizer Edge Pvt. Ltd. | M365 Copilot Training Series | FY 2026-27*
*For queries: training@technizeredge.com*
