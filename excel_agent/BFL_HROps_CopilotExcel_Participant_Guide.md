# Copilot in Excel — Participant Exercise Guide
### Formulas & Pivot Tables for HR Operations
**Bajaj Finance Limited | M365 Copilot Training**
**File:** `BFL_HROps_Copilot_Demo.xlsx`

---

## Before You Begin

- Use **Copilot agent** to open the agent in the Copilot panel
- Add `BFL_HROps_Copilot_Demo.xlsx` from OneDrive
- Keep the Copilot panel open throughout all exercises
- The file has **25 rows of HR operations data** — one sheet, no formula columns yet
- Columns N–Q are intentionally blank — you will fill these using Copilot

### Dataset Overview

| Column | Field | Description |
|--------|-------|-------------|
| A | Request ID | Unique HR request reference (HRO-001 to HRO-025) |
| B | Department | Department where the request was raised |
| C | Dept Code | Short department identifier |
| D | Region | West / Central |
| E | HR Request Type | Onboarding, Payroll Query, Document Update, Separation, Grievance |
| F | HR BP Owner | HR Business Partner handling the request |
| G | Request Date | When the request was logged |
| H | Resolved Date | When it was resolved (blank if still open) |
| I | TAT (Days) | Actual turnaround time in days |
| J | SLA Limit (Days) | Benchmark TAT for that request type |
| K | Employee Band | M3, M4, M5, M6, M7 |
| L | Priority | Normal, High, Urgent |
| M | Status | Closed, Pending, Escalated |
| **N–Q** | *(blank)* | **You will add these using Copilot** |

---

## Exercise 1 — Add a Formula Column: Escalation Flag

### Your Turn
Type into the Copilot panel:

```
In column N, add a formula that flags each request as "Escalate" or
"OK" based on its Priority and Status:
- "Escalate" if Priority is "Urgent" OR Status is "Escalated"
- "OK" for all other cases
Label the column "Escalation Flag". Apply to all 25 rows.
```

### What Copilot Will Produce
```excel
=IF(OR(L3="Urgent",M3="Escalated"),"Escalate","OK")
```
Copilot will name the column, write the formula, and fill it down to N27.

> **Discussion Point:** Which HR request types are most likely to attract an Urgent or Escalated status? What does this tell us about HRBP workload?

---

## Exercise 2 — Add a Formula Column: SLA Breach

### Your Turn
Type into the Copilot panel:

```
In column O, add a formula that checks whether each HR request
breached its SLA. Compare the TAT in column I against the SLA
Limit in column J. If TAT is greater than the SLA Limit, return
"Breach". Otherwise return "On Time". If TAT is blank (request
still open), return "Pending".
Label the column "SLA Breach". Apply to all 25 rows.
```

### What Copilot Will Produce
```excel
=IF(I3="","Pending",IF(I3>J3,"Breach","On Time"))
```

> **Discussion Point:** Payroll Queries show the most SLA breaches. What upstream factors in the HR process might cause this pattern?

---

## Exercise 3 — Add a Formula Column: Pending Days

### Your Turn
Type into the Copilot panel:

```
In column P, calculate the number of days each HR request has been
open. If the request is already resolved (column H has a date),
return 0. If it is still open, return the number of days since
the request was received (column G) up to today.
Label the column "Pending Days". Apply to all 25 rows.
```

### What Copilot Will Produce
```excel
=IF(H3<>"",0,TODAY()-DATEVALUE(G3))
```
Resolved requests show 0. Open requests show how many days they have been waiting.

> **Discussion Point:** Which open requests are ageing the most? Are there specific HRBPs or departments where pending cases are clustering?

---

## Exercise 4 — Add a Formula Column: TAT Category

### Your Turn
Type into the Copilot panel:

```
In column Q, classify each resolved HR request into a TAT
performance category based on how the actual TAT (column I)
compares to the SLA Limit (column J):
- "Fast" if TAT is 50% or less of the SLA Limit
- "Within SLA" if TAT is within the SLA Limit
- "Moderate Breach" if TAT exceeds SLA by up to 50%
- "Critical Breach" if TAT exceeds SLA by more than 50%
- "Pending" if TAT is blank
Label the column "TAT Category". Apply to all 25 rows.
```

### What Copilot Will Produce
```excel
=IF(I3="","Pending",IF(I3<=J3*0.5,"Fast",IF(I3<=J3,"Within SLA",IF(I3<=J3*1.5,"Moderate Breach","Critical Breach"))))
```

---

## Exercise 5 — Ask Copilot to Explain a Formula

### Your Turn
Copy the formula from cell **Q3** and paste it into the Copilot panel:

```
Explain this formula to me in simple terms. What does each part do?
```

### What Copilot Will Explain
> *"This formula first checks if the TAT in I3 is blank — if so, the request is still Pending. Then it checks if TAT is at most half the SLA limit, which means the HRBP resolved it very Fast. Next it checks if TAT is within the full SLA Limit — that's Within SLA. If TAT went over the limit but not by more than 50%, it's a Moderate Breach. Anything beyond 150% of the SLA Limit is a Critical Breach. Each IF only runs when the previous condition wasn't true."*

---

## Exercise 6 — Create a Pivot Table: Requests by HR Request Type and Status

### Your Turn
Type into the Copilot panel:

```
Create a pivot table that shows the count of HR requests for each
Request Type, broken down by Status (Closed, Pending, Escalated).
I want to see which HR request types have the most unresolved or
escalated cases.
```

### What Copilot Will Produce
A new sheet with a Pivot Table:
- **Rows:** HR Request Type (Onboarding, Payroll Query, Document Update, Separation, Grievance)
- **Columns:** Status (Closed, Pending, Escalated)
- **Values:** Count of Request ID

> **Discussion Point:** Grievances show a high Escalated ratio relative to volume. What does that signal about the current grievance resolution process?

---

## Exercise 7 — Create a Pivot Table: Average TAT by HRBP

### Your Turn
Type into the Copilot panel:

```
Now create a pivot table showing the average TAT in days for each
HR BP Owner, broken down by HR Request Type. I want to identify
which HRBPs or request types are taking the longest to resolve.
```

### What Copilot Will Produce
- **Rows:** HR BP Owner (Pooja Nair, Rahul Sharma, Anita Desai, Vikram Joshi, Ravi Kumar)
- **Columns:** HR Request Type
- **Values:** Average of TAT (Days)

> **Discussion Point:** Which HRBP has the highest average TAT on Payroll Queries? Which request type consistently breaches SLA across multiple owners?

---

## Exercise 8 — Bonus: Ask Copilot for Insights

### Your Turn
Type into the Copilot panel:

```
Look at the data in this sheet. Which departments have the most SLA
breaches? Summarise the key risk areas for the HR Ops team
in 3 bullet points.
```

### What to Expect
Copilot will scan the data and generate a natural-language summary — no formula needed. This shows how Copilot moves from *calculation* to *analysis* to *insight* within the same Excel session.

---

*Bajaj Finance Limited | AI Academy — HR Operations | Microsoft Copilot Training Programme*
