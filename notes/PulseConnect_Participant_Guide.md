# M365 Copilot – Meta Prompts Hands-On Guide
## Pulse Connect Feedback Analysis → Business Head Dashboard
**AI for HR Partnering & Operations | Technizer Edge**
**Module 2 – Employee Engagement & Pulse Analysis**

---

## What You Will Learn

By the end of this exercise you will be able to:

- Use the **Meta Prompt Framework** to generate ready-to-use Copilot prompts
- Analyse open-text employee feedback and extract sentiment themes
- Segment pulse scores by team and grade to identify at-risk groups
- Generate a structured Business Head dashboard summary — directly from raw survey data

---

## The Meta Prompt Framework

Instead of writing a Copilot prompt from scratch, you describe your situation and let Copilot write the prompt for you. This is the Meta Prompt technique.

**The template:**

```
Act as a Microsoft Copilot prompt expert.

I am a [YOUR ROLE] at [COMPANY / CONTEXT].
I need to [WHAT YOU WANT TO DO].
My audience is [WHO WILL READ OR USE THE OUTPUT].
The data I have is [BRIEF DESCRIPTION OF YOUR INPUT DATA].

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

**How it works — two steps every time:**

1. Paste the Meta Prompt into Copilot → you get a ready-to-use Copilot prompt
2. Attach your data file and paste that generated prompt → you get your output

> **Tip:** You never need to write a complex prompt yourself. Just fill in the four fields — role, goal, audience, data — and Copilot does the rest.

---

## Your Practice Dataset

Open the file: **`PulseConnect_BH_Dashboard.xlsx`**

It has five sheets. Here is what each one contains:

| Sheet | What it contains |
|---|---|
| Raw Feedback Data | 120 survey responses — grade, team, location, 4 scores, open-text feedback |
| Sentiment Theme Analysis | 10 engagement themes extracted from open feedback |
| Score Summary – Team & Grade | Average scores by team and by grade with risk flags |
| High Risk Flags | 12 employees flagged for priority HRBP follow-up |
| BH Dashboard Summary | Final Business Head ready output — scorecard, themes, action plan |

Start on the **Raw Feedback Data** sheet. The other sheets show you what a well-structured output looks like after Copilot analyses the data.

---

## Exercise 1 — Explore What Copilot Can Do

**Goal:** Generate a list of analyses Copilot can run on your Pulse Connect data.

**Step 1** — Paste this Meta Prompt into M365 Copilot Chat:

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP at Bajaj Finance Limited.
I need to understand what kinds of analysis I can run on a Pulse Connect survey dataset.
My audience is myself — I want to explore what's possible before I start.
The data I have is an Excel file with 120 survey responses including employee grade, team,
location, scores on 4 dimensions (Work Environment, Manager Support, Career Growth,
Work-Life Balance), and open-text feedback.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

**Step 2** — Read the prompt Copilot generates. Attach your Excel file and run it.

**What to notice:** Copilot understood your situation and built the instruction for you. You only had to describe what you have and what you want.

---

## Exercise 2 — Extract Sentiment Themes from Open Feedback

**Goal:** Find out what employees are actually saying — clustered into named themes with sentiment labels.

**Step 1** — Paste this Meta Prompt into M365 Copilot Chat:

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP at a financial services firm.
I need to analyse the open-text feedback column from a Pulse Connect survey of 120 employees
and extract the top engagement themes — what employees are saying, how strongly, and whether
the sentiment is positive, negative, or mixed.
My audience is my Business Head and HR leadership.
The data I have is an Excel sheet with 120 rows. Column L contains open-text feedback
written by employees in their own words.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

**Step 2** — Attach `PulseConnect_BH_Dashboard.xlsx` and run the generated prompt.

**Step 3** — Compare Copilot's output with the **Sentiment Theme Analysis** sheet in the Excel file.

**What to notice:** Copilot read 120 different responses and identified the dominant themes without you manually reading each row. This is qualitative analysis done in minutes.

---

## Exercise 3 — Segment Scores by Team and Grade

**Goal:** Identify which teams and grades have the lowest engagement scores so you know where to focus first.

**Step 1** — Paste this Meta Prompt into M365 Copilot Chat:

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP conducting a Pulse Connect debrief for a 120-person business unit.
I need to segment the survey scores by team and by grade to identify which groups
have the lowest engagement scores and should be flagged for priority HRBP attention.
My audience is my Business Head — the output should be structured for a review meeting.
The data I have is an Excel file with columns for Grade, Team, and 4 score columns
(Work Environment, Manager Support, Career Growth, Work-Life Balance) — each scored 1–5.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

**Step 2** — Attach the Excel file and run the generated prompt.

**Step 3** — Compare the output with the **Score Summary – Team & Grade** sheet.

**What to notice:** You now have a specific, evidence-based answer — not "engagement has dropped" but "Sales and Collections at M1–M2 grade are the most at-risk groups." That precision changes the conversation with your Business Head.

---

## Exercise 4 — Generate the Business Head Dashboard Summary

**Goal:** Produce a complete, leadership-ready dashboard covering key metrics, top themes, high-risk flags, and a Q2 action plan.

**Step 1** — Paste this Meta Prompt into M365 Copilot Chat:

```
Act as a Microsoft Copilot prompt expert.

I am an HRBP preparing for a monthly Business Head review meeting at a financial services firm.
I need to generate a structured dashboard summary of this quarter's Pulse Connect results,
covering: key engagement metrics vs last quarter, top 3 concern themes with grade-level
impact, high-risk employee flags, and a prioritised action plan for Q2 FY26.
My audience is the Business Head — the tone should be crisp, data-led, and actionable.
The data I have is an Excel file with raw survey responses (120 employees), average scores
by team and grade, extracted sentiment themes, and a list of 12 flagged high-risk employees.

Write me a detailed, structured Copilot prompt I can use to complete this task.
The prompt should specify: role, task, context, data format, output format, and tone.
```

**Step 2** — Attach the Excel file and run the generated prompt.

**Step 3** — Compare the output with the **BH Dashboard Summary** sheet.

**Optional — Export to Word:**
After the dashboard is generated, type the following to convert it into a shareable document:

```
Convert this into a formatted Word document with the following structure:
- Title: Pulse Connect – Q1 FY26 Business Head Summary
- Section 1: Engagement Scorecard table
- Section 2: Top 3 Concern Themes (one paragraph each with grade impact and recommended action)
- Section 3: High Risk Employee Summary (table format)
- Section 4: Q2 FY26 People Agenda (action table with owner and timeline)
Format it ready to share with leadership.
```

**What to notice:** You went from 120 rows of raw data to a Business Head ready summary in four prompts. The HRBP's time shifts from data assembly to leadership conversation.

---

## Try It Yourself — Meta Prompt Builder

Use this table to build your own Meta Prompts for other HR tasks:

| I want to… | Role | Task | Output |
|---|---|---|---|
| Extract feedback themes | HRBP / HR Analyst | Identify top engagement themes from open text | Named themes with sentiment and mention count |
| Segment scores | HRBP / People Analytics | Break down scores by grade, team, location | Table with average score and risk flag |
| Flag high-risk employees | HRBP | Identify employees with consistently low scores | Prioritised list with intervention notes |
| Build a BH dashboard | HRBP preparing for leadership review | Synthesise survey results into a dashboard | Scorecard + themes + action plan |
| Draft talking points | HRBP / HR Manager | Prepare speaking notes for engagement debrief | 3–5 bullets per theme, leadership tone |
| Write a follow-up email | HRBP | Communicate Pulse results to team managers | 150-word manager communication with action asks |

**Try changing one thing:** Swap your audience from "Business Head" to "CHRO" and run the same Meta Prompt. Notice how the tone and structure of the generated prompt changes.

---

## Key Takeaways

- The Meta Prompt framework works for any HR scenario — engagement, attrition, onboarding, compliance. The template stays the same; only the four fields change.
- Always attach your data file before running the generated prompt. Copilot needs the file to do the analysis.
- Copilot does not replace your HR judgement. It removes the hours of manual data work so you can focus on the conversations and decisions that matter.
- The High Risk Flags output raises an important question: how do you handle sensitive employee data responsibly? Discuss with your HRBP team before sharing flagged information.

---

*Technizer Edge | AI for HR Partnering & Operations | BFL Engagement Module*
