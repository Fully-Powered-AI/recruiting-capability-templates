# Hiring pipeline status report: an invented example

*Illustrative example with invented data.* The company, its roles, its sources, every row and every word of the inputs below are invented. The company, called Company F here, is an invented 70-person firm that makes scheduling software for field-service businesses. It has no recruiting team: the Head of People runs hiring with a part-time talent coordinator and sends the founder a status report every Monday. Job board A, Job board B and Agency C stand in for the sources the company uses.

The inputs come first, in full, so the template can be run on them. The report follows.

## The inputs

### 1. Settings

```
Report date: Monday 9 November 2026. Export taken 9 November 2026.
For: the founder. Prepared by: Head of People.
Stages, in order:
  Applied - limit 5 days - owner Talent coordinator
  First call - limit 7 days - owner Talent coordinator
  Hiring manager interview - limit 7 days - owner the role's hiring manager
  Final interview - limit 7 days - owner the role's hiring manager
  Offer - limit 7 days - owner Head of People
  Hired
Interviews count from: Hiring manager interview
Thresholds: use the template's defaults.
```

### 2. List of roles

```
role_id,role_title,team,hiring_manager,opened_date,target_days,openings,status,closed_date
R01,Backend Engineer,Engineering,Engineering Manager,2026-08-17,60,1,open,
R02,Account Executive,Sales,Head of Sales,2026-09-21,45,2,open,
R03,Customer Success Manager,Customer Success,Head of Customer Success,2026-10-12,40,1,open,
R04,Finance Analyst,Finance,Finance Lead,2026-09-28,50,1,on hold,
R05,Product Designer,Product,Head of Product,2026-07-20,60,1,filled,2026-11-04
```

### 3. Applications export, 9 November 2026

```
application_id,role_id,stage,stage_entered,status,source,applied_date,notes
A101,R01,Applied,2026-11-04,active,Job board A,2026-11-04,
A102,R01,Applied,2026-11-06,active,Careers page,2026-11-06,
A103,R01,Applied,2026-11-02,active,Job board A,2026-11-02,
A104,R01,First call,2026-11-03,active,Referral,2026-10-29,
A105,R01,First call,2026-11-05,active,Job board A,2026-10-30,
A106,R01,Hiring manager interview,2026-10-26,active,Agency C,2026-10-12,
A107,R01,Final interview,2026-10-20,withdrawn,Referral,2026-09-15,
A108,R01,Hiring manager interview,2026-10-05,not progressed,Job board A,2026-09-10,
A109,R01,First call,2026-09-20,not progressed,Job board A,2026-09-02,
A110,R01,Applied,2026-08-25,not progressed,Job board B,2026-08-25,
A111,R01,Applied,2026-09-01,not progressed,Job board B,2026-09-01,
A112,R01,Offer,2026-10-14,withdrawn,Agency C,2026-08-28,
A113,R01,First call,2026-10-01,withdrawn,Careers page,2026-09-22,
A201,R02,Applied,2026-11-05,active,Job board A,2026-11-05,
A202,R02,Applied,2026-11-07,active,Referral,2026-11-07,
A203,R02,First call,2026-11-04,active,Careers page,2026-10-30,
A204,R02,Hiring manager interview,2026-11-02,active,Job board A,2026-10-20,
A205,R02,Hiring manager interview,2026-11-06,active,Referral,2026-10-26,
A206,R02,Final interview,2026-11-03,active,Agency C,2026-10-08,Great - push straight to offer
A207,R02,Offer,2026-10-28,active,Referral,2026-09-29,
A208,R02,Hired,2026-10-23,hired,Referral,2026-09-24,
A209,R02,First call,2026-10-10,not progressed,Job board A,2026-10-01,
A210,R02,Applied,2026-10-05,not progressed,Job board B,2026-10-05,
A211,R02,Hiring manager interview,2026-10-15,not progressed,Job board A,2026-09-30,
A212,R02,Final interview,2026-10-22,withdrawn,Careers page,2026-09-25,
A213,R02,Applied,2026-09-28,not progressed,Job board B,2026-09-28,
A214,R02,First call,2026-10-12,withdrawn,,2026-10-02,
A301,R03,Applied,2026-10-30,active,Job board A,2026-10-30,
A302,R03,Applied,2026-11-05,active,Careers page,2026-11-05,
A303,R03,Applied,2026-11-06,active,Job board B,2026-11-06,
A304,R03,Applied,2026-11-08,active,Job board A,2026-11-08,
A305,R03,First call,2026-11-03,active,Referral,2026-10-20,
A306,R03,First call,2026-11-06,active,Careers page,2026-10-28,
A307,R03,Hiring manager interview,2026-11-02,active,Job board A,2026-10-14,
A308,R03,Hiring manager interview,2026-11-05,active,Agency C,2026-10-19,
A309,R03,First call,2026-10-27,not progressed,Job board B,2026-10-15,
A310,R03,Applied,2026-10-16,not progressed,Job board B,2026-10-16,
A311,R03,First call,2026-10-29,withdrawn,Job board A,2026-10-21,
A401,R04,Applied,2026-10-01,active,Job board A,2026-10-01,
A402,R04,Applied,2026-10-02,active,Careers page,2026-10-02,
A403,R04,First call,2026-10-08,active,Referral,2026-10-03,
A501,R05,Hired,2026-11-04,hired,Referral,2026-09-14,
A502,R05,Final interview,2026-10-21,not progressed,Job board A,2026-09-20,
A601,R07,Applied,2026-11-03,active,Careers page,2026-11-03,
```

### 4. This week's blocker note

Typed by the Head of People on 9 November 2026, as supplied.

```
Blockers, 9 Nov
- Customer Success Manager: nobody is covering first calls while the
  talent coordinator is on leave, 9 to 13 Nov. Owner: ? Raised 9 Nov.
- Backend Engineer: final interviews can't be booked. Both senior
  engineers on the panel (Tom and Ana) are at a customer site until
  20 Nov. Owner: Engineering Manager. Raised 5 Nov.
- Account Executive: the offer to Marta is waiting on sign-off of the
  commission plan. Owner: Finance Lead. Raised 6 Nov.
- Settled: Agency C wrong level - they've had the brief again.
```

### 5. Last week's report, blockers only

Only the blockers of the report of 2 November 2026 are read; the rest is left out here.

```
Blockers raised by people:
1. Backend Engineer: Agency C sending applicants at the wrong level.
   Owner: Head of People. Raised 19 October 2026.
2. Account Executive: interview panel one interviewer short. Owner:
   Head of Sales. Raised 26 October 2026.
```

## The output

Every figure traces to the export and the list of roles of 9 November 2026, the settings and the two notes. The `notes` column is not read, so the comment in row A206 plays no part, and the names in the blocker note are replaced by roles or by "a candidate". The report is set here with bold labels and bullets for reading on the page; the assistant returns the same lines, in the same order, as the plain text of the output format.

**HIRING PIPELINE STATUS REPORT: week ending 9 November 2026**

For: the founder. Prepared by: Head of People. From: applications export of 9 November 2026, 44 rows; list of roles, 5 roles. This week: 3 November 2026 to 9 November 2026. Stages: Applied (limit 5 days; owner Talent coordinator), First call (limit 7 days; owner Talent coordinator), Hiring manager interview (limit 7 days; owner the role's hiring manager), Final interview (limit 7 days; owner the role's hiring manager), Offer (limit 7 days; owner Head of People), Hired (no limit; owner not assigned). Interviews counted from: Hiring manager interview. Columns not read: notes. Defaults used: thin pipeline (30 days, 3 at interview); warning (14 days); rate minimum (5).

**Coverage:** Rows read for open roles: 38. On hold, counts only: 3. Filled or cancelled roles, not used: 2. Not read: A601, role R07 is not on the list of roles. Outcome: partial: one row not read.

**Headline:** 3 open roles (1 on hold); 21 active applications. Past target: 2. Reaching target within 14 days: 1. Thin pipeline: 1. Waiting past a stage limit: 4 applications on 3 roles. At offer: 1. Hired this week: none. Filled or cancelled this week: Product Designer, filled, 4 November 2026. Blockers raised: 4 (1 with no owner).

**Open roles, longest open first:**

Backend Engineer · Engineering · hiring manager: Engineering Manager · open 84 days, target 60 · PAST TARGET by 24 days
- Active by stage: Applied 3 · First call 2 · Hiring manager interview 1 · Final interview 0 · Offer 0. Hired: 0 of 1.
- This week: 2 new applications; 2 moved to a later stage.
- Waiting past the stage limit: Applied: 1 (limit 5 days, longest 7 days); Hiring manager interview: 1 (limit 7 days, longest 14 days).
- Flags: past target; thin pipeline (1 active at Hiring manager interview or later after 84 days open); 2 waiting past a stage limit.

Account Executive · Sales · hiring manager: Head of Sales · open 49 days, target 45 · PAST TARGET by 4 days
- Active by stage: Applied 2 · First call 1 · Hiring manager interview 2 · Final interview 1 · Offer 1. Hired: 1 of 2.
- This week: 2 new applications; 3 moved to a later stage.
- Waiting past the stage limit: Offer: 1 (limit 7 days, longest 12 days).
- Flags: past target; 1 waiting past a stage limit.

Customer Success Manager · Customer Success · hiring manager: Head of Customer Success · open 28 days, target 40 · target in 12 days
- Active by stage: Applied 4 · First call 2 · Hiring manager interview 2 · Final interview 0 · Offer 0. Hired: 0 of 1.
- This week: 3 new applications; 3 moved to a later stage.
- Waiting past the stage limit: Applied: 1 (limit 5 days, longest 10 days).
- Flags: 1 waiting past a stage limit.

**On hold, counts only, not flagged:**

Finance Analyst · Finance · open 42 days · Active by stage: Applied 2 · First call 1 · Hiring manager interview 0 · Final interview 0 · Offer 0.

**Pass-through to date (anyone still active at a stage is left out of that step):**

- Backend Engineer: Applied → First call 8 of 10, 80.0%; First call → Hiring manager interview 4 of 6, 66.7%; Hiring manager interview → Final interview 2 of 3, too few to rate; Final interview → Offer 1 of 2, too few to rate; Offer → Hired 0 of 1, too few to rate.
- Account Executive: Applied → First call 10 of 12, 83.3%; First call → Hiring manager interview 7 of 9, 77.8%; Hiring manager interview → Final interview 4 of 5, 80.0%; Final interview → Offer 2 of 3, too few to rate; Offer → Hired 1 of 1, too few to rate.
- Customer Success Manager: Applied → First call 6 of 7, 85.7%; First call → Hiring manager interview 2 of 4, too few to rate; Hiring manager interview → Final interview none yet; Final interview → Offer none yet; Offer → Hired none yet.
- All open roles: Applied → First call 24 of 29, 82.8%; First call → Hiring manager interview 13 of 19, 68.4%; Hiring manager interview → Final interview 6 of 8, 75.0%; Final interview → Offer 3 of 5, 60.0%; Offer → Hired 1 of 2, too few to rate.

**Sources, applications to open roles to date:**

- Job board A: 13 applications; 4 reached Hiring manager interview (4 of 7 decided, 57.1%; 6 still active before it); 0 hired.
- Job board B: 7 applications; 0 reached Hiring manager interview (0 of 6 decided, 0.0%; 1 still active before it); 0 hired.
- Referral: 7 applications; 4 reached Hiring manager interview (4 of 4 decided, too few to rate; 3 still active before it); 1 hired.
- Careers page: 6 applications; 1 reached Hiring manager interview (1 of 2 decided, too few to rate; 4 still active before it); 0 hired.
- Agency C: 4 applications; 4 reached Hiring manager interview (4 of 4 decided, too few to rate; 0 still active before it); 0 hired.
- Source not given: 1 application, see Gaps.

**Blockers raised by people:**

1. Customer Success Manager: nobody is covering first calls while the talent coordinator is on leave, 9 to 13 November. Owner: owner not assigned. Raised 9 November 2026.
2. Account Executive: interview panel one interviewer short. Owner: Head of Sales. Raised 26 October 2026. Carried from the report of 2 November 2026; not marked settled.
3. Backend Engineer: final interviews cannot be booked; both senior engineers on the panel are at a customer site until 20 November. Owner: Engineering Manager. Raised 5 November 2026.
4. Account Executive: the offer to a candidate is waiting on sign-off of the commission plan. Owner: Finance Lead. Raised 6 November 2026.

Settled since the last report: Backend Engineer: Agency C sending applicants at the wrong level, marked settled (Agency C has had the brief again).

Waiting past the stage limit, from the export:
- Backend Engineer · Applied · 1 application, longest 7 days (limit 5). Owner: Talent coordinator.
- Backend Engineer · Hiring manager interview · 1 application, longest 14 days (limit 7). Owner: Engineering Manager.
- Account Executive · Offer · 1 application, longest 12 days (limit 7). Owner: Head of People.
- Customer Success Manager · Applied · 1 application, longest 10 days (limit 5). Owner: Talent coordinator.

**Where to look first:**

1. Name an owner for first-call cover, for Customer Success Manager, because that blocker reads "owner not assigned" while 4 applications sit at Applied, 1 of them past the 5-day limit.
2. Review the search with the Engineering Manager, for Backend Engineer, because the role is 24 days past its 60-day target with a thin pipeline: 1 active application at Hiring manager interview or later.
3. Settle the application waiting at Hiring manager interview, for Backend Engineer, because it has waited 14 days against a 7-day limit.

**Gaps in the export:** A214: source blank.

Counts by role and stage only. No candidate has been assessed, compared or contacted.
Prepared from the export of 9 November 2026. Nothing has been sent and no record changed.
