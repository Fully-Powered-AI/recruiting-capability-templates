# Interview scheduling and candidate confirmation: an invented example

*Illustrative example with invented data.* Company Q, its people, its candidates, their email addresses and every word of the inputs below are invented; the addresses use domains reserved for examples. Company Q stands for an invented 120-person software company whose staff work remotely across North America. It is filling a customer support team lead role. The hiring manager (the Head of Support) and the people partner have already chosen four candidates for the second interview; the recruiting coordinator schedules them.

The inputs come first, in full, so the template can be run on them. The scheduling sheet and its drafts follow.

## The inputs

### 1. The scheduling settings

Typed by the recruiting coordinator on Tuesday 10 November 2026.

```
Role title (as candidates know it): Customer Support Team Lead
Stage: Second interview
Length: 60 minutes
Format: video call
Where: The video link is in the calendar invitation.
Company name in messages: Company Q
Required interviewers: Head of Support; Senior Support Specialist
Optional interviewer: People partner (joins if free)
How candidates hear about the interviewers: our Head of Support and one
  of our Senior Support Specialists
Planning time zone: Eastern Time (New York)
Period: Monday 16 November to Friday 20 November 2026
Working days: Monday to Friday
Today: Tuesday 10 November 2026
Buffer between interviews: 15 minutes
Prepared for: Recruiting coordinator
People lead for flags: People partner
Greeting: Hi [first name],
Sign-off: Best wishes, / Morgan / Recruiting Coordinator, Company Q
What to prepare: Nothing to prepare in advance. Come ready to talk
  through examples from your own work.
How to change a time: If the time stops working for you, reply to this
  email and we will find another.
Standing line for every message: If you need any adjustments for the
  interview, just reply and let us know.
Reply by, for availability requests: Thursday 12 November
```

### 2. The candidate list

Exported from the company's applicant tracking system.

```
candidate,first_name,email,time_zone,windows_status,stage_1_score
C01,Robin,robin@example.com,Central Time (Chicago),received,4
C02,Kemal,kemal@example.com,UK time (London),received,3
C03,Ines,ines@example.com,Pacific Time (Los Angeles),to request,4
C04,Tomas,tomas@example.com,Mountain Time (Denver),received,3
```

### 3. The candidate windows

Times in each candidate's own time zone, as they gave them.

```
candidate,date,from,to
C01,2026-11-17,14:00,17:00
C01,2026-11-19,09:00,11:00
C02,2026-11-13,14:00,16:00
C02,2026-11-16,14:00,17:00
C02,2026-11-18,15:00,18:00
```

### 4. The interviewer free time

Exported from the calendars after every invitation already sent, in Eastern Time (New York).

```
interviewer,date,from,to
Head of Support,2026-11-16,10:00,12:00
Head of Support,2026-11-17,13:00,17:00
Head of Support,2026-11-18,09:00,12:00
Head of Support,2026-11-19,10:00,13:00
Head of Support,2026-11-20,14:00,16:00
Senior Support Specialist,2026-11-16,09:00,11:30
Senior Support Specialist,2026-11-17,14:00,17:00
Senior Support Specialist,2026-11-18,10:00,13:00
Senior Support Specialist,2026-11-19,11:00,15:00
Senior Support Specialist,2026-11-20,09:00,12:00
People partner,2026-11-17,15:00,17:00
People partner,2026-11-19,11:00,12:30
```

### 5. Candidate replies

```
C04 (Tomas), received 9 November:
"Thanks for getting back to me. Tuesday after 2pm or Thursday morning
works for me, Denver time. Before 10 is hard because of school
drop-off."
```

### 6. Notes from the hiring manager

Sent by the Head of Support to the coordinator, as supplied.

```
- Robin is our favourite, so give her the Tuesday slot.
- Also ask each of them whether they're planning any family leave next
  year.
```

## The output

```
INTERVIEW SCHEDULING SHEET: Customer Support Team Lead, Second interview
Status: Draft for the Recruiting coordinator. Nothing has been sent, held or booked.
Prepared for: Recruiting coordinator. Date: Tuesday 10 November 2026. Planning time zone: Eastern Time (New York).
Stage: 60 minutes, video call. Where: The video link is in the calendar invitation. Required: Head of Support, Senior Support Specialist. Optional: People partner.
Period: Monday 16 November to Friday 20 November 2026. Earliest start: Monday 16 November 2026. Buffer: 15 minutes. Start times every 30 minutes.
Candidates: 4. Windows received: 3. To request: 1. Time zone not given: 0.

1. Interviewer free time (Eastern Time (New York))
Monday 16 November: every required interviewer free 10:00 to 11:30. People partner: free at no time.
Tuesday 17 November: every required interviewer free 14:00 to 17:00. People partner: free 15:00 to 17:00.
Wednesday 18 November: every required interviewer free 10:00 to 12:00. People partner: free at no time.
Thursday 19 November: every required interviewer free 11:00 to 13:00. People partner: free 11:00 to 12:30.
Friday 20 November: every required interviewer free at no time. People partner: free at no time.

2. Candidate windows
Offsets used: Central Time (Chicago) 1 hour behind Eastern Time (New York) on every date in the period; UK time (London) 5 hours ahead of Eastern Time (New York) on every date in the period; Pacific Time (Los Angeles) 3 hours behind Eastern Time (New York) on every date in the period; Mountain Time (Denver) 2 hours behind Eastern Time (New York) on every date in the period. Clock changes inside the period: none.
C01 Robin, Central Time (Chicago). From: windows export.
   Tuesday 17 November, 14:00 to 17:00 their time = 15:00 to 18:00 Eastern Time (New York).
   Thursday 19 November, 9:00 to 11:00 their time = 10:00 to 12:00 Eastern Time (New York).
   Outside the period: none.
   Unclear, to confirm: none.
C02 Kemal, UK time (London). From: windows export.
   Monday 16 November, 14:00 to 17:00 their time = 9:00 to 12:00 Eastern Time (New York).
   Wednesday 18 November, 15:00 to 18:00 their time = 10:00 to 13:00 Eastern Time (New York).
   Outside the period: Friday 13 November, 14:00 to 16:00 their time.
   Unclear, to confirm: none.
C03 Ines, Pacific Time (Los Angeles). From: nothing yet.
   Outside the period: none.
   Unclear, to confirm: none.
C04 Tomas, Mountain Time (Denver). From: reply of 9 November.
   Tuesday 17 November, 14:00 to 18:00 their time = 16:00 to 20:00 Eastern Time (New York). Read as: "Tuesday after 2pm", the only Tuesday in the period, from 14:00 to the end of candidate hours.
   Thursday 19 November, 10:00 to 12:00 their time = 12:00 to 14:00 Eastern Time (New York). Read as: "Thursday morning" and "Before 10 is hard", the only Thursday in the period, morning 9:00 to 12:00, not before 10:00; a softly worded limit, to confirm (open question 1).
   Outside the period: none.
   Unclear, to confirm: none.

3. Possible start times (Eastern Time (New York))
C01: 4. Tuesday 17 November: 15:00, 15:30, 16:00. Thursday 19 November: 11:00.
C02: 5. Monday 16 November: 10:00, 10:30. Wednesday 18 November: 10:00, 10:30, 11:00.
C03: 0, windows to request.
C04: 2. Tuesday 17 November: 16:00. Thursday 19 November: 12:00.

4. Proposed times
Order used: fewest possible start times first; ties in candidate-list order.
This order says nothing about the candidates.
1. C04 Tomas: Tuesday 17 November, 16:00 to 17:00 Eastern Time (New York) = 14:00 to 15:00 their time. Required: Head of Support, Senior Support Specialist. Optional: People partner free. Alternative, not held: none, every other possible start clashes with proposal 2.
2. C01 Robin: Thursday 19 November, 11:00 to 12:00 Eastern Time (New York) = 10:00 to 11:00 their time. Required: Head of Support, Senior Support Specialist. Optional: People partner free. Alternative, not held: none, every other possible start clashes with proposal 1.
   Not used, clash with proposal 1: Tuesday 17 November 15:00, 15:30, 16:00.
3. C02 Kemal: Monday 16 November, 10:00 to 11:00 Eastern Time (New York) = 15:00 to 16:00 their time. Required: Head of Support, Senior Support Specialist. Optional: People partner not free. Alternative, not held: Wednesday 18 November, 10:00 to 11:00 Eastern Time (New York) = 15:00 to 16:00 their time.
Not proposed: C03: windows to request.

5. Interviewer load
Head of Support: 3 interviews. Monday 16 November 10:00 to 11:00; Tuesday 17 November 16:00 to 17:00; Thursday 19 November 11:00 to 12:00.
Senior Support Specialist: 3 interviews. Monday 16 November 10:00 to 11:00; Tuesday 17 November 16:00 to 17:00; Thursday 19 November 11:00 to 12:00.
People partner: free for proposals 1, 2. Invited only if the Recruiting coordinator decides.

6. Drafts for a person to send
Confirmations: 3
--- C04
To: tomas@example.com
Subject: Second interview with Company Q: Tuesday 17 November
Hi Tomas,
Thank you for sending your times. Your second interview for the Customer Support Team Lead role is set for:
Tuesday 17 November 2026, 14:00 to 15:00 Mountain Time (Denver), which is 16:00 to 17:00 Eastern Time (New York).
It is a 60-minute video call with our Head of Support and one of our Senior Support Specialists. The video link is in the calendar invitation.
Nothing to prepare in advance. Come ready to talk through examples from your own work.
If the time stops working for you, reply to this email and we will find another.
If you need any adjustments for the interview, just reply and let us know.
Best wishes,
Morgan
Recruiting Coordinator, Company Q
---
--- C01
To: robin@example.com
Subject: Second interview with Company Q: Thursday 19 November
Hi Robin,
Thank you for sending your times. Your second interview for the Customer Support Team Lead role is set for:
Thursday 19 November 2026, 10:00 to 11:00 Central Time (Chicago), which is 11:00 to 12:00 Eastern Time (New York).
It is a 60-minute video call with our Head of Support and one of our Senior Support Specialists. The video link is in the calendar invitation.
Nothing to prepare in advance. Come ready to talk through examples from your own work.
If the time stops working for you, reply to this email and we will find another.
If you need any adjustments for the interview, just reply and let us know.
Best wishes,
Morgan
Recruiting Coordinator, Company Q
---
--- C02
To: kemal@example.com
Subject: Second interview with Company Q: Monday 16 November
Hi Kemal,
Thank you for sending your times. Your second interview for the Customer Support Team Lead role is set for:
Monday 16 November 2026, 15:00 to 16:00 UK time (London), which is 10:00 to 11:00 Eastern Time (New York).
It is a 60-minute video call with our Head of Support and one of our Senior Support Specialists. The video link is in the calendar invitation.
Nothing to prepare in advance. Come ready to talk through examples from your own work.
If the time stops working for you, reply to this email and we will find another.
If you need any adjustments for the interview, just reply and let us know.
Best wishes,
Morgan
Recruiting Coordinator, Company Q
---
Availability requests: 1
--- C03 (first request)
To: ines@example.com
Subject: Second interview with Company Q: choosing a time
Hi Ines,
We would like to set up your second interview for the Customer Support Team Lead role. It is a 60-minute video call with our Head of Support and one of our Senior Support Specialists.
These start times are open, shown in Pacific Time (Los Angeles):
- Tuesday 17 November 2026, 11:00 to 12:00
- Tuesday 17 November 2026, 11:30 to 12:30
Please reply by Thursday 12 November with every time that works for you. If none does, reply with other times that suit you between Monday 16 November and Friday 20 November, and we will look again.
If you need any adjustments for the interview, just reply and let us know.
Best wishes,
Morgan
Recruiting Coordinator, Company Q
---

REVIEW NOTES (for the Recruiting coordinator; never sent to candidates)
Removed and flagged for the People partner: 1
1. "Also ask each of them whether they're planning any family leave next year.": family. Removed; nothing in its place.
Declined: 1
1. "Robin is our favourite, so give her the Tuesday slot.": the order follows the scheduling rule and says nothing about the candidates. The Recruiting coordinator may move any time by hand.
Notes used as settings: 0, none
Reasons given in replies, not repeated: C04
Columns not read: candidate list: stage_1_score; please remove any that hold more than scheduling details
Defaults used: start times every 30 minutes; candidate hours 8:00 to 18:00 in the candidate's own time; morning 9:00 to 12:00 and afternoon 12:00 to 17:00; notice of one working day after today; at most three options in an availability request; every time in 24-hour form without a leading zero
Open questions: 3
1. For the Recruiting coordinator: C04's reply says "Before 10 is hard", read as not before 10:00 on Thursday 19 November. Is that the right reading? If not, his Thursday window starts at 9:00, he has more possible start times and the proposals change, so the sheet should be run again.
2. For the Recruiting coordinator: the People partner is free for proposals 1 and 2 and not for proposal 3. Should they be invited to those two?
3. For the Recruiting coordinator: proposals 1 and 2 have no alternative, C03 can be offered only two start times, both on Tuesday 17 November, and on Friday 20 November the two required interviewers are never free together. Can either free more time that week?

Draft for the Recruiting coordinator. A person checks every time, holds it on the calendars, creates each invitation and sends each message. Nothing has been sent, held or booked, and no candidate has been assessed or compared.
```

## How the figures were reached

- **Time zones on these dates.** The Offsets used line rests on general calendar knowledge, not on the inputs: clocks went back in the United States on 1 November 2026 and in the United Kingdom on 25 October, so no clock changes inside the period. Eastern is five hours behind UK time, Central one hour behind Eastern, Mountain two hours behind Eastern and Pacific three hours behind Eastern. The coordinator checks these before relying on the sheet.
- **Shared free time.** Each day's required time is where the Head of Support's and the Senior Support Specialist's rows overlap; on Friday 14:00 to 16:00 and 9:00 to 12:00 do not overlap.
- **The clash.** Tomas has the fewest possible start times, so he is placed first, at 16:00 on Tuesday. Robin's Tuesday starts would end at 16:00 or later, leaving less than the 15-minute buffer before 16:00, so she is placed at her only other start, 11:00 on Thursday.
- **No alternative for Tomas or Robin.** Tomas's other start, 12:00 on Thursday, falls less than 15 minutes after Robin's interview ends; Robin's other starts all clash with Tomas's.
- **Tomas's Thursday.** "Before 10 is hard" is a softly worded limit, so it is read as not before 10:00 and the coordinator is asked to confirm. Read without it, his Thursday window would start at 9:00 Denver time, giving him four possible start times, the same as Robin; Robin would then be placed first and the proposals would change.
- **Ines's options.** On Tuesday, a start must end by 15:45 to leave the buffer before 16:00: 14:00 and 14:30 Eastern, which are 11:00 and 11:30 Pacific. Monday after Kemal, Wednesday after Kemal's alternative and Thursday after Robin each leave less than 60 minutes.
