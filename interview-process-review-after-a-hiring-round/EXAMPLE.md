# Interview process review after a hiring round: an invented example

*Illustrative example with invented data.* The company, the role, the interviews, every question and every word of the feedback below are invented. The company, called Company K here, is an invented 45-person firm that makes booking software for restaurants. It has just closed a round for a Customer Operations Manager, with three candidates interviewed. The recruiting lead asked an operations coordinator to prepare the review. Candidates and interviewers appear only as codes (K1 to K3 and P1, P2, P4).

The inputs come first, in full, so the template can be run on them. The review follows.

## The inputs

### 1. Settings

```
Role: Customer Operations Manager. Round closed: Friday 6 November 2026.
Review date: Tuesday 10 November 2026.
For: the recruiting lead. Prepared by: operations coordinator.
Rating scale: 1 to 4.
Thresholds: use the template's defaults.
```

### 2. Agreed rubric

```
criterion_id,criterion,what_good_evidence_looks_like
C1,Handles escalations and fixes causes,"A specific escalation the person led, what they did first, and what they changed afterwards"
C2,Plans team cover,"How cover was built from volume, and a case where it fell short"
C3,Coaches individuals,"A kind of coaching given to a named type of person, and what changed"
C4,Uses data to decide,"A metric they tracked, what it showed and the action they took"
C5,Works with product and engineering,"A joint piece of work with dates and who agreed"
C6,Writes clear customer guidance,"A piece of customer-facing writing they produced and what they removed or changed"
```

### 3. Interview plan

```
interview_id,interview_name,question_id,question,criterion_id
I1,Hiring manager conversation,Q1,"Tell us about the last serious escalation you handled. What did you do first, and what changed afterwards?",C1
I1,Hiring manager conversation,Q2,How do you coach people on your team?,C3
I1,Hiring manager conversation,Q3,How do you plan cover for your team?,C2
I2,Operations panel,Q3,How do you plan cover for your team?,C2
I2,Operations panel,Q4,"Which support metric do you watch most closely, and what did you do the last time it moved?",C4
I2,Operations panel,Q5,How comfortable are you with numbers?,C4
I3,Cross-team conversation,Q6,How do you work with product and engineering?,C5
I3,Cross-team conversation,Q7,Describe a repeat complaint you traced to its cause.,C1
```

### 4. Panel feedback (anonymised)

```
candidate_ref,interview_id,interviewer_ref,question_id,rating,evidence_note
K1,I1,P1,Q1,3,"Described a billing outage; paged the on-call engineer within ten minutes, wrote the customer update personally and later got the retry rule changed."
K1,I1,P1,Q2,3,Strong coaching instincts.
K1,I1,P1,Q3,2,"Builds the rota from ticket volume by hour; had a gap on Sundays that was covered personally."
K1,I2,P2,Q3,3,Same rota example as the first interview; nothing new.
K1,I2,P2,Q4,4,"Cut the reopen rate from 14% to 9% by splitting two macros; checks it weekly."
K1,I2,P2,Q5,3,Good with numbers.
K1,I3,P4,Q6,3,"Worked with product to retire a confusing setting; gave the dates and who agreed."
K1,I3,P4,Q7,4,"Traced repeat refund complaints to one unclear policy line and got it reworded within a week."
K2,I1,P1,Q1,3,"Walked through a delayed-shipment complaint; phoned the customer, then asked the warehouse to change the label check."
K2,I1,P1,Q2,3,Seemed keen on developing people.
K2,I1,P1,Q3,3,"Uses last quarter's ticket counts to plan cover; no example of a shortfall."
K2,I2,P2,Q3,,NOT ASKED
K2,I2,P2,Q4,2,"Tracks first-reply time in a spreadsheet; could not say what was done when it rose."
K2,I2,P2,Q5,2,Seemed unsure.
K2,I3,P4,Q6,2,Said engineers are easy to work with.
K2,I3,P4,Q7,3,"Found a repeat complaint came from a policy wording and got it changed."
K3,I1,P1,Q1,4,"Described a data-loss complaint; worked with the customer through the weekend and set up a checklist afterwards."
K3,I1,P1,Q2,,NOT ASKED
K3,I1,P1,Q3,2,"Plans cover with a shared calendar and asks people to swap shifts two weeks ahead."
K3,I2,P2,Q3,4,Gave the same shared-calendar answer; nothing new.
K3,I2,P2,Q4,3,"Compares weekly ticket tags to find the top three causes; named the three found."
K3,I2,P2,Q5,3,Strong analytical thinker.
K3,I3,P4,Q6,3,Said product is a close working partner.
K3,I3,P4,Q7,1,Answer was general; no specific case.
```

### 5. Process issues noted during the round

```
1. Operations coordinator: the second interview for K2 started 20 minutes late and ran short.
2. Recruiting coordinator: the feedback form has a rating box and a comment box but no place for an example.
3. Recruiting coordinator: the cross-team interviewer did not see the level descriptions for C5 before the round.
```

## The review

```
INTERVIEW PROCESS REVIEW: Customer Operations Manager, round closed 6 November 2026

For: the recruiting lead. Prepared by: operations coordinator. Review date: 10 November 2026. From: rubric, 6 criteria; interview plan, 8 rows, 3 interviews, 7 questions; feedback, 24 rows, 3 candidates; process issues note supplied. Scale: 1 to 4. Columns not read: none. Defaults used: question minimum (2); spread threshold (2); candidate minimum (3).

Coverage: Feedback rows read: 24. Not read: none. Outcome: complete.

Headline: 7 questions in the plan; 4 interview-question pairs gave little usable evidence. Repeated across interviews: 1. Criteria: 3 covered, 1 thin, 1 asked with no usable evidence, 0 planned but never asked, 1 with no question. Rated rows with no usable note: 10 of 22. Ratings 2 or more points apart: 2 of 5 compared. Not asked: 2. Process issues noted: 3.

1. Questions with little usable evidence (asked 2 or more times, fewer than half of the notes usable)
Q5 · Operations panel · C4: 0 usable of 3 asked. Judged not usable: impression only 3.
Q2 · Hiring manager conversation · C3: 0 usable of 2 asked. Judged not usable: impression only 2.
Q3 · Operations panel · C2: 0 usable of 2 asked. Judged not usable: repeat of an earlier answer 2.
Q6 · Cross-team conversation · C5: 1 usable of 3 asked. Judged not usable: general statement 2.

2. Repeated questions
Q3 (C2) is in the Hiring manager conversation and the Operations panel. First: 3 usable of 3 asked. Later: 0 usable of 2 asked; 2 notes repeated the earlier answer.

3. Criteria coverage
C1 Handles escalations and fixes causes: covered. 3 of 3 candidates with usable evidence; Q1, Q7.
C2 Plans team cover: covered. 3 of 3 candidates with usable evidence; Q3.
C3 Coaches individuals: asked, no usable evidence. 0 of 3 candidates with usable evidence; Q2.
C4 Uses data to decide: covered. 3 of 3 candidates with usable evidence; Q4, Q5.
C5 Works with product and engineering: thin. 1 of 3 candidates with usable evidence; Q6.
C6 Writes clear customer guidance: no question in the plan. 0 of 3 candidates with usable evidence; no question.

4. Rubric use
Rated with no usable note, by interview: Hiring manager conversation 2 of 8 rated; Operations panel 5 of 8; Cross-team conversation 3 of 6. All interviews: 10 of 22.
Ratings 2 or more points apart where two or more interviewers rated the same criterion for a candidate: C1, 1 of 3 comparisons, largest gap 3 (K3 · I1 · Q1 and K3 · I3 · Q7); C2, 1 of 2 comparisons, largest gap 2 (K3 · I1 · Q3 and K3 · I2 · Q3).
Outside the scale: none.
These gaps may come from the ratings resting on different questions, so they are a reason to read the rows, not a finding about anyone. Each interview here had one interviewer, so an interview code identifies that person; keep this section to those who need it.

5. Questions not asked
1. K2 · I2 · Q3 (C2, the only question for C2): see process issue 1.
2. K3 · I1 · Q2 (C3, the only question for C3): no process issue noted.

6. Process issues noted
1. Operations coordinator: the second interview for K2 started 20 minutes late and ran short. The files show something related: one question not asked in that interview (K2 · I2 · Q3). Start time and length are not in the files.
2. Recruiting coordinator: the feedback form has a rating box and a comment box but no place for an example. The files show something related: 10 of 22 rated rows with no usable note. The form itself is not in the files.
3. Recruiting coordinator: the cross-team interviewer did not see the level descriptions for C5 before the round. The files show something related: 1 usable note of 3 for Q6, the only question for C5. What the interviewer was given beforehand is not in the files.

7. Notes judged not usable, for the recruiting lead to check
K1 · I1 · Q2 · impression only
K1 · I2 · Q3 · repeat of an earlier answer
K1 · I2 · Q5 · impression only
K2 · I1 · Q2 · impression only
K2 · I2 · Q5 · impression only
K2 · I3 · Q6 · general statement
K3 · I2 · Q3 · repeat of an earlier answer
K3 · I2 · Q5 · impression only
K3 · I3 · Q6 · general statement
K3 · I3 · Q7 · general statement

8. Proposed revisions (all drafts; each waits for the recruiting lead)
R1. Reword Q2 (C3, Hiring manager conversation) to ask for one past case. Because: finding 1, 0 usable of 2 asked. Draft wording: "Tell us about someone you coached. What was the gap, what did you do, and what changed?" Decision: awaiting the recruiting lead.
R2. Remove Q3 from the Operations panel. Because: findings 1 and 2; both notes repeated the first interview, and C2 is covered 3 of 3 there. Decision: awaiting the recruiting lead.
R3. Remove Q5 (C4, Operations panel). Because: finding 1, 0 usable of 3 asked; C4 is covered 3 of 3 by Q4. Decision: awaiting the recruiting lead.
R4. Reword Q6 (C5, Cross-team conversation) to ask for one joint piece of work, and ask the rubric's owners for the C5 level descriptions, which the files do not hold, so that interviewer has them before the round. Because: finding 1, 1 usable of 3; process issue 3. Draft wording: "Tell us about something you changed together with product or engineering. Who was involved, and when?" Decision: awaiting the recruiting lead.
R5. Add a question for C6 to the Operations panel, where R2 and R3 remove two questions. Because: finding 3, C6 has no question. Draft wording: "Describe a reply or help article you wrote that you are proud of. What did you leave out, and why?" Decision: awaiting the recruiting lead.
R6. Add a required "example or quote" field before the rating box on the feedback form. Because: finding 4, 10 of 22 rated rows had no usable note; process issue 2. Decision: awaiting the recruiting lead.
R7. Look with the panel at the rows named in finding 4 before the next search, and hold a short session on the C1 and C2 rubric levels if the gaps come from the levels rather than from different questions. Because: finding 4, ratings 2 or more points apart on 1 of 3 comparisons for C1 and 1 of 2 for C2; the C1 gap compares Q1 with Q7, so it may reflect different evidence. Decision: awaiting the recruiting lead.
R8. Put the only question for a criterion first in its interview, and agree in advance what to drop if time runs short. Because: finding 5, the only question for C3 was not asked for one candidate (K3 · I1 · Q2) and the only question for C2 was not asked for another (K2 · I2 · Q3); process issue 1 concerns the second. Decision: awaiting the recruiting lead.

9. Gaps in the files
None. Repeats are checked by question ID only.

The review of Customer Operations Manager looks at the process only. No candidate has been assessed, scored or compared, and no outcome has been reopened. Nothing has been sent and no record changed; every revision waits for the recruiting lead.
```
