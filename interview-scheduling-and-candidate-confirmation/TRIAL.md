# Interview scheduling and candidate confirmation: tried on its example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-10
- **Template version:** 0.1.0, as revised on 10 November 2026

The inputs are the invented example in `public/example.md` (Company Q, four invented candidates, invented addresses on reserved example domains). No client data was used. It shows what the template produced once, on one set of inputs. It is not a test in any company's environment.

This is the second run on the example. The first, on the same day, was made by Claude Sonnet 5.5, a model that had not written the template; it agreed with the example on every time, count, order, proposal, alternative, option and draft, and listed the places where the instructions left room to guess. After an independent review, the template was revised to close them (see "The earlier run, and what was changed" below); the example's inputs were not changed. The run recorded here was then made on the revised version by the same model, in the same session, that made the revisions, and that had already read the first run's record and the example. It followed the revised instruction block and output format on the six inputs, and the example's published output was then replaced with this output. It is therefore a check that the revised instructions produce the published result, not an independent trial: the agreement below is expected and is not evidence from a fresh reader.

## Inputs used

All six inputs in `public/example.md`, section "The inputs": the scheduling settings, the candidate list (with its extra `stage_1_score` column), the candidate windows, the interviewer free time, the one candidate reply, and the two notes from the hiring manager.

## What came out

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

## What was observed

- **Every required part was produced.** All six numbered sections with the new Offsets used line, the three confirmations, the one availability request, every review-notes heading and the closing line. Nothing told the run to stop: the four required settings were present, every header matched, no candidate reference was repeated and both required interviewers had rows.
- **The two risky notes were handled as the template says.** The favourite request was declined and the order did not change. The question about family leave was removed from every draft, nothing was put in its place, and it was flagged for the people partner. The standing line offering adjustments asks the candidate nothing, so under the revised step it was kept. The `stage_1_score` column was not read or repeated, and its header was listed with a request to remove it. The reason in the reply was not repeated; only the words "Before 10 is hard" were quoted, and the candidate's reference is listed under reasons not repeated.
- **What the revisions changed in the output.** The times, proposals, alternative and options are the same as in the first run. The differences are where the revised rules apply: an Offsets used line; a reason after each alternative of "none"; the stage name in lower case inside the messages; times without a leading zero (9:00, not 09:00); a sixth item under Defaults used for the time format; and an open question asking the coordinator to confirm the reading of "Before 10 is hard", which the revised step 5 now requires. The buffer was applied to the alternative and to Ines's options, as the revised steps 8 and 10 now say; this gave the same two options as before.
- **Facts not in the inputs.** The output contains no fact about a candidate or the company that is not in the inputs. The offsets and the absence of a clock change in the period come from general calendar knowledge (US clocks changed on 1 November 2026, UK clocks on 25 October), and are now stated in the sheet so the coordinator can check them.
- **Open points that remain.**
  1. "Notice of one working day after today" is still not defined to the hour. It did not matter here because the period starts five days later.
  2. Two options offered to the same candidate may overlap each other (Ines's 11:00 and 11:30). That is correct, since she needs only one, but the template does not say it.
  3. Which open questions beyond the required ones a run asks is left to the run, so another run may ask different ones.
  4. The run needs careful arithmetic across four time zones and a buffer rule, which the template leaves to the assistant. Every figure here was checked by hand against the exports, and the reviewer checklist asks a person to do the same.
- **What this does not show.** It is one run on one invented example, in one product, by the model that revised the template. It does not show how the template behaves on messy exports, a clock change inside a period, a missing header or a longer candidate list. The proposed acceptance tests in the template have not been run.

## The earlier run, and what was changed

The first run, on 10 November 2026 in Claude Code with Claude Sonnet 5.5, used the template as first written and the same inputs. It read only the instruction block, the output format and the six inputs, and read the example's output only afterwards. Its sheet agreed with the example then published on every time, count, order, proposal, alternative, option and draft. It differed in small ways: it kept the stage name as supplied ("Second interview") inside the messages, where the example wrote "second interview"; it wrote times such as 09:00 with a leading zero, where the example did not; its flag line said "family leave" where the example said "family"; and its open questions were different (it asked the coordinator to confirm the reading of "Before 10 is hard" and noted that Ines had only two options, where the example asked about inviting the people partner and about freeing more interviewer time).

It recorded these places where the instructions left room to guess:

1. Step 7 defined a clash with the buffer, but steps 8 and 10 said only "clash", so the buffer's reach over alternatives and availability options was unclear. The run applied it throughout, as the example did.
2. Step 5 covered "not before 10" but gave no rule for softer wording such as "Before 10 is hard".
3. Nothing said whether messages to candidates use 24-hour time or am and pm.
4. Nothing said whether to adjust the case of the stage name inside "Your [stage name]".
5. The output format had nowhere to say why an alternative is "none".
6. Two options for the same candidate may overlap; the template did not say so.
7. "Notice of one working day after today" was not defined to the hour.

It also noted that the template did not say where clock-change dates and zone offsets come from.

Changed after the first run and an independent review, before the run recorded above:

- **Buffer.** The alternative and the availability-request options must leave at least the buffer between them and every proposal and alternative (procedure steps 8 and 10, instruction-block items 7 and 9).
- **Softly worded limits.** Read like the plain limit, with an open question asking the coordinator to confirm the reading (step 5, item 4).
- **Offsets.** A new Offsets used line in section 2 states each zone's offset from the planning zone and any clock change in the period, which come from general calendar knowledge; an uncertain clock-change date becomes an open question (step 4, item 3).
- **Time format.** A new setting with a default: 24-hour form without a leading zero, such as 9:00 and 14:30, in the sheet and the drafts (Inputs, defaults paragraph).
- **Stage name.** Written in lower case inside a sentence unless it contains a proper name; the subject line keeps it as supplied (step 11, item 10).
- **"None" alternatives.** The output format now gives the reason after "none" (step 8, item 7).
- **Adjustments.** An open offer of adjustments that asks the candidate nothing is not a protected-subject match and is kept (step 13, item 11).
- **Instruction block.** Item 1 now carries the header counts from procedure step 1, and a long unwrapped line in item 4 was rewrapped.
- **The example's output** was replaced with the output of the run recorded above. The example's inputs did not change.
