# Interview scheduling and candidate confirmation

Workflow template, version 0.1.0.

## Purpose

Prepare the scheduling for one interview stage of one role, for candidates people have already chosen to interview: a scheduling sheet that turns each candidate's offered windows into the company's planning time zone, lays them against the time when every required interviewer is free, and proposes one start time per candidate with no interviewer booked twice; then, for each candidate, a confirmation draft with the details or an availability request draft in the company's own words. The assistant prepares only. It never judges, compares or orders candidates on anything but their times, never asks about pay, health, family, immigration or any other protected subject, and never sends a message, holds a calendar slot, creates an invitation or changes a record. A person checks every time and sends everything.

## When to use it and when not to

Use it when a stage has candidates waiting for a time: after the people deciding have chosen who goes forward, and again whenever replies come in, an interviewer's calendar changes or a proposed time falls through. Each run works from the latest exports, so earlier proposals that were never confirmed are simply proposed again or replaced.

Do not use it:

- to decide who is interviewed, who goes forward or who is hired. People make those calls before this workflow template is run; it schedules the candidates it is given;
- to read CVs, applications, scores or interview notes. The sheet needs times, time zones and contact details, nothing else;
- to write the interview questions or the scorecard. The Interview plan and scorecard workflow template prepares those;
- to write a job posting, an offer or any employment document;
- to book rooms, hold calendar slots, create invitations or update an applicant tracking system. A person does each of these after reading the sheet.

## Roles

- **Runs it, supplies the exports and replies, checks every time, holds the slots, creates the invitations and sends every message:** the recruiting coordinator, or the hiring manager doing their own scheduling.
- **Supplies the free time:** each interviewer, through their calendar or a list the coordinator exports.
- **Receives every flag about a protected subject:** the people lead the settings name (an HR lead, or the office manager where there is no people team).
- **Decides who is interviewed and who goes forward:** the hiring manager and the people the company names. Always people, and never through this workflow template.

## Inputs

1. **The scheduling settings,** typed by the coordinator:
   - the role title as candidates know it; the stage name; its length in minutes; its format; where it happens (an address, or a note such as where the video link will be);
   - the required interviewers and any optional ones, named as they appear in the free-time export, and how candidates hear about them (for example "our Head of Support and one of our Senior Support Specialists");
   - the planning time zone; the scheduling period (first and last date); the working days; today's date;
   - the company name as messages give it; the greeting and sign-off; what candidates should prepare; how a candidate changes a time; any standing lines every message carries, such as a question about adjustments; the reply-by date for availability requests;
   - who the sheet is prepared for, and the people lead who receives flags;
   - [your buffer] between two interviews for the same interviewer (default 15 minutes); [your start-time step] (default every 30 minutes, on the hour and half hour); [your candidate hours], the earliest and latest times the company offers in a candidate's own time (default 8:00 to 18:00); what "morning" and "afternoon" mean in a reply (default 9:00 to 12:00 and 12:00 to 17:00); [your notice], the least notice before an interview (default one working day after today); [your number of options] in an availability request (default three); [your time format] for every time in the sheet and the drafts (default 24-hour without a leading zero, such as 9:00 and 14:30).
   If the length, the planning time zone, the period or the required interviewers are missing, stop and ask. Where a default is used, say so under Defaults used. Any other missing item is a marked gap in the drafts, such as "[How to change a time: to be supplied by the coordinator]", with an open question. Wording the settings give for messages is copied exactly.
2. **The candidate list,** as an export or table with these column headers: `candidate`, `first_name`, `email`, `time_zone`, `windows_status`. `candidate` is a short reference such as C01; `windows_status` is `received` or `to request`. If a required header is missing or named differently, stop and ask which column holds what; never guess. Any other column is not read: list its header under Columns not read, never repeat what is in it, and if it holds anything about a candidate beyond scheduling, such as a score, ask for it to be removed from the export.
3. **The candidate windows,** as an export or table with these column headers: `candidate`, `date`, `from`, `to`. Dates as YYYY-MM-DD; times in 24-hour form in the candidate's own time zone, as the candidate gave them. If a header is missing or named differently, stop and ask.
4. **The interviewer free time,** as an export or table with these column headers: `interviewer`, `date`, `from`, `to`, in the planning time zone, taken after every invitation already sent. If a header is missing or named differently, stop and ask. If a required interviewer has no rows, say so and propose nothing.
5. **Candidate replies** (optional): a candidate's reply pasted as written, labelled with their reference. Used only for the times and time zone in it.
6. **Notes from the hiring manager or the coordinator** (optional). Each note ends up under exactly one heading of the review notes, or is used as a setting.

The assistant works from what the person pastes or uploads. It needs no connection to a calendar, an email account or an applicant tracking system, and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** One role, one stage, the four required settings present, every header as stated. Count the candidates and say how many have windows, how many are to be asked, and how many have no time zone. If two rows share a candidate reference, stop and ask. A candidate marked `received` with no windows and no reply is treated as to request, with an open question for the coordinator.
2. **Read only what scheduling needs.** Use the reference, first name, email, time zone and times. Leave every other column unread and listed. If a reply gives a reason for its times, such as school runs, a medical appointment, a religious observance or another job, use the times and never repeat, record or ask about the reason; list the candidate's reference under "Reasons given in replies, not repeated".
3. **Find the interviewer free time.** For each working day in the period, find the time when every required interviewer is free, from their rows. Note when each optional interviewer is free. Earliest start is the later of the first day of the period and [your notice] after today.
4. **Turn each candidate's windows into the planning time zone.** Use each date's own offset, so a clock change inside the period is handled day by day; if either zone changes its clocks inside the period, add an open question asking the coordinator to check the times on those dates. Write each window in the candidate's own time and in the planning time zone, and every time in the sheet and the drafts in [your time format]. On the Offsets used line, state how far each candidate's zone is from the planning time zone on the dates used and any clock change inside the period, so the coordinator can check them; these come from general calendar knowledge, not from the inputs, so if a zone's clock-change dates are uncertain, say so in an open question. A window outside the period is listed as such and not used. A window the candidate offered is used as given, even outside [your candidate hours].
5. **Read replies plainly.** A weekday with no date means that weekday inside the period if there is exactly one; otherwise it is unclear. "Morning" and "afternoon" take the meanings in the settings. "After [time]" runs from that time to the end of [your candidate hours]; "before [time]" from the start of [your candidate hours] to that time; a limit such as "not before 10" applies to every window in the reply. A limit worded softly, such as "before 10 is hard", is read the same way, with an open question asking the coordinator to confirm the reading. Show each such reading as "Read as" beside the window, quoting the words. Anything else loose ("any time next week", "flexible", "evenings") is not turned into times: list it as unclear, to confirm. A candidate who has not replied has offered no times; never assume a time suits them. If a reply names a time zone that differs from the candidate list, use neither: list the candidate as time zone not given and ask the coordinator.
6. **List the possible start times** for each candidate: every start time on [your start-time step] where the whole interview fits inside one of the candidate's windows and inside the time when every required interviewer is free, on or after the earliest start. Count them. A candidate with no time zone, no windows yet, only unclear windows or no possible start time has 0, with the reason.
7. **Propose one time per candidate.** Take the candidates in order of fewest possible start times first, ties in the order of the candidate list; write that this order says nothing about the candidates. For each, propose the earliest possible start time that leaves at least [your buffer] between it and every interview already proposed for the same interviewers. List possible start times not used because of a clash, naming the proposal they clash with. If every possible start time clashes, the candidate is not proposed and gets an availability request. Never change the order or the choice for any reason about a candidate.
8. **Add one alternative** for each proposed candidate, not held: another of their possible start times, on a different day where there is one, that clashes with no proposal and no earlier alternative, leaving at least [your buffer] between it and each of them. Take the candidates in the same order. Write "none" when there is no such time, with the reason: no other possible start time, or every other possible start clashes, naming the proposals or alternatives it clashes with. Note whether each optional interviewer is free for each proposal.
9. **Count each interviewer's load:** the proposals they are in, with times. An optional interviewer is listed with the proposals they are free for; whether they are invited is the coordinator's call.
10. **Find the options for each availability request.** For each candidate not proposed, find start times on [your start-time step] when every required interviewer is free, on or after the earliest start, that clash with no proposal and no alternative, leaving at least [your buffer] between them and each of them, and that fit wholly inside [your candidate hours] in the candidate's own time. Take the earliest, up to [your number of options], spread over different days where possible. No start time appears twice in the sheet, so nothing is offered to two candidates. Where the time zone is not given, use the planning time zone and name it. If no option is left, write a marked gap in the draft and an open question about extending the period or freeing interviewer time.
11. **Draft the confirmations,** in proposal order, one per proposed candidate, following the output format: the greeting; thanks for the times; the role and stage; the date and time in the candidate's own time, with the planning-zone time beside it when the zones differ; the length, format and interviewers as candidates hear about them; where it happens; what to prepare, how to change a time and the standing lines, each copied exactly or marked as a gap; the sign-off. Inside a sentence the stage name is written in lower case unless it contains a proper name ("Second interview" becomes "your second interview"); the subject line keeps it as supplied. Say nothing about the process, the pay, the role or the candidate beyond what the settings give.
12. **Draft the availability requests,** one per candidate not proposed, following the output format, with the reason line that fits (none for a first request). Ask for every option that works, by the reply-by date, and invite other times inside the period. One message per candidate per run: no reminder or chaser unless the coordinator asks, and no message that pushes a candidate to take a time.
13. **Check the words against the protected subjects.** Every setting, note and draft, against this list, which always applies: pay, salary or benefits; health or disability; family, children, childcare, pregnancy, marital status or plans for any of them; immigration, visas, sponsorship or right to work; age; religion; race, ethnicity, nationality or where someone is from; sex, gender or sexual orientation; criminal records or background checks. Remove each match, put nothing in its place, and flag it for the people lead. An open offer of adjustments that asks the candidate nothing, such as "If you need any adjustments for the interview, just reply", is not a match and is kept; a question about a candidate's health, disability or needs is a match.
14. **Write the review notes** and the closing line, in the order of the output format. A heading with nothing under it says 0 and "none". Return the draft to the person it is prepared for. Nothing is sent, held or booked until a person does it.

## Exceptions and stop conditions

- **Length, planning time zone, period or required interviewers missing:** stop and ask.
- **A required header missing or named differently in any export:** stop and ask which column holds what. Never guess.
- **Two rows with the same candidate reference:** stop and ask.
- **A required interviewer has no free-time rows:** propose nothing, draft no confirmation, and ask the coordinator; availability requests are not drafted either, because no time can be offered.
- **Asked to put one candidate first, give a candidate a better time, or choose who gets a contested time for any reason about the candidate:** decline. The order follows the rule in step 7; the coordinator may move any time by hand after reading the sheet. List the request under Declined.
- **Asked to screen, score, rank or compare candidates, read a CV or interview notes, or say who should go forward or be hired:** decline. People decide; this workflow template schedules.
- **A setting, note or draft touches a protected subject,** such as a request to ask about current pay, plans for leave or visa status: remove it, put nothing in its place, and flag it for the people lead.
- **A reply gives a reason for its times:** use the times only; never repeat, record or ask about the reason.
- **A reply and the candidate list disagree on the time zone:** treat the time zone as not given and ask the coordinator.
- **Asked to send a message, hold a slot, create an invitation, or update the applicant tracking system or any record:** decline. A person does it after checking the sheet.
- **Asked to tell a candidate a time is fixed before a person has held it and created the invitation:** decline; the drafts are sent only after that.

## Output format

```
INTERVIEW SCHEDULING SHEET: [Role title], [stage name]
Status: Draft for the [role]. Nothing has been sent, held or booked.
Prepared for: [role]. Date: [weekday D Month YYYY]. Planning time zone: [zone].
Stage: [n] minutes, [format]. Where: [as supplied / marked gap]. Required: [interviewers]. Optional: [interviewers / none].
Period: [weekday D Month] to [weekday D Month YYYY]. Earliest start: [weekday D Month YYYY]. Buffer: [n] minutes. Start times every [n] minutes.
Candidates: [n]. Windows received: [n]. To request: [n]. Time zone not given: [n].

1. Interviewer free time ([planning zone])
[Weekday D Month]: every required interviewer free [time to time / at no time]. [Optional interviewer]: free [time to time / at no time].

2. Candidate windows
Offsets used: [zone] [n] hours [behind / ahead of] [planning zone] [on every date in the period / from D Month]; [...]. Clock changes inside the period: [zone, D Month / none].
[Ref] [first name], [time zone / time zone not given]. From: [windows export / reply of D Month / nothing yet].
   [Weekday D Month], [time to time] their time = [time to time] [planning zone]. [Read as: "[words as written]", [the reading]. / omit]
   Outside the period: [windows / none].
   Unclear, to confirm: "[words as written]" / none.

3. Possible start times ([planning zone])
[Ref]: [n]. [Weekday D Month]: [times]. / [Ref]: 0, [windows to request / time zone not given / windows unclear / no window meets the interviewers' free time].

4. Proposed times
Order used: fewest possible start times first; ties in candidate-list order.
This order says nothing about the candidates.
[n]. [Ref] [first name]: [weekday D Month], [time to time] [planning zone] = [time to time] their time. Required: [interviewers]. Optional: [name free / name not free / none]. Alternative, not held: [weekday D Month, time to time [planning zone] = time to time their time / none, no other possible start time / none, every other possible start clashes with [proposal n / the alternative for proposal n]].
   [Not used, clash with proposal [n]: [weekday D Month times]. / omit]
Not proposed: [Ref]: [windows to request / time zone not given / windows unclear / no possible start time / every possible start time clashes]. / none.

5. Interviewer load
[Required interviewer]: [n] interviews. [Weekday D Month time to time; ...] / 0, none.
[Optional interviewer]: free for proposals [numbers / none]. Invited only if the [role] decides.

6. Drafts for a person to send
Confirmations: [n] / 0, none
--- [Ref]
To: [email]
Subject: [Stage name] with [company]: [weekday D Month]
[Greeting]
Thank you for sending your times. Your [stage name] for the [role title] role is set for:
[Weekday D Month YYYY], [time] to [time] [candidate's zone][, which is [time] to [time] [planning zone]].
It is a [n]-minute [format] with [interviewers as candidates hear about them]. [Where.]
[What to prepare, exactly as supplied / omit if none given]
[How to change a time, exactly as supplied / marked gap]
[Standing lines, exactly as supplied / omit if none given]
[Sign-off]
---
Availability requests: [n] / 0, none
--- [Ref] ([first request / no possible start time / every possible start time clashes / windows unclear / time zone not given])
To: [email]
Subject: [Stage name] with [company]: choosing a time
[Greeting]
We would like to set up your [stage name] for the [role title] role. It is a [n]-minute [format] with [interviewers as candidates hear about them].
[Reason line / omit for a first request]
These start times are open, shown in [candidate's zone / planning zone]:
- [Weekday D Month YYYY], [time] to [time]
[/ marked gap: no open start time in the period]
Please reply by [reply-by date / marked gap] with every time that works for you. If none does, reply with other times that suit you between [weekday D Month] and [weekday D Month], and we will look again.
[Standing lines, exactly as supplied / omit if none given]
[Sign-off]
---

REVIEW NOTES (for the [role]; never sent to candidates)
Removed and flagged for the [people lead role]: [n] / 0, none
[n]. "[as written]": [subject]. Removed; nothing in its place.
Declined: [n] / 0, none
[n]. "[request]": [reason].
Notes used as settings: [n] / 0, none
[n]. "[as written]": [the setting it fills].
Reasons given in replies, not repeated: [refs / none]
Columns not read: [export: headers; please remove any that hold more than scheduling details / none]
Defaults used: [items / none]
Open questions: [n] / 0, none
[n]. For the [role]: [question]

Draft for the [role]. A person checks every time, holds it on the calendars, creates each invitation and sends each message. Nothing has been sent, held or booked, and no candidate has been assessed or compared.
```

Reason lines for an availability request:

- No possible start time, or every possible start time clashes: "Thank you for sending your times. None of them lines up with the times our interviewers are free, so here are some others."
- Windows unclear: "Thank you for your reply. To find a time, we need particular days and times."
- Time zone not given: "Please also tell us which time zone you are in. The times below are in [planning zone]."

## Reviewer checklist

1. Every window has been turned into the planning time zone correctly, with each date's own offset, and the Offsets used line is right for those dates. (Recruiting coordinator)
2. Every proposed time lies wholly inside one of the candidate's windows and inside every required interviewer's free time, on or after the earliest start. (Recruiting coordinator)
3. No interviewer has two proposed interviews closer than the buffer, and no start time appears twice in the sheet. (Recruiting coordinator)
4. Every "Read as" line is a fair reading of the candidate's words, and nothing unclear has been turned into times. (Recruiting coordinator)
5. The proposal order follows the rule, and no request to favour a candidate has changed it. (Recruiting coordinator)
6. No setting, note or draft touches a protected subject, every flagged item has been dealt with, and no reason a candidate gave for their times appears anywhere. (People lead)
7. Every draft uses the company's wording exactly where the settings give it, and states the time in the candidate's own time zone. (Recruiting coordinator)
8. Each time is held on the calendars and the invitation created before its confirmation is sent. (Recruiting coordinator)

## Acceptance tests

Proposed tests. None has been run.

1. **Ordinary run.** Three candidates with windows in three time zones, two required interviewers, no clashes. Expected: three proposals, each inside the candidate's window and the interviewers' free time, three confirmations with both zones shown.
2. **Clash.** Two candidates whose only shared time is the same hour. Expected: the candidate with fewer possible start times is proposed first; the other gets their next start time or, if none, an availability request; the clash is listed.
3. **Buffer.** Two proposals for the same interviewers 10 minutes apart with a 15-minute buffer. Expected: the second moves to the next start time that leaves 15 minutes.
4. **Header mismatch.** The windows export says `start` and `end` instead of `from` and `to`. Expected: stops and asks which column is which; proposes nothing.
5. **Extra column.** The candidate list carries a column of first-round scores. Expected: not read or repeated; the header listed under Columns not read with a request to remove it.
6. **Reason in a reply.** "Not Fridays, I have hospital appointments." Expected: Fridays left out; the reason appears nowhere; the reference listed under Reasons given in replies, not repeated.
7. **Loose reply.** "Any time next week is fine." Expected: unclear, to confirm; no times invented; an availability request with the windows-unclear line.
8. **No time zone.** A candidate with windows and no time zone. Expected: not proposed; an availability request in the planning zone, naming it, that asks for their time zone.
9. **Clock change.** A period that spans a clock change in the candidate's zone. Expected: each date converted with its own offset; an open question asks the coordinator to check those dates.
10. **Favouring a candidate.** "Give our favourite the Tuesday slot." Expected: declined; order unchanged; listed under Declined.
11. **Protected subject in the settings.** A standing line asking what the candidate earns now. Expected: removed from every draft, nothing in its place, flagged for the people lead.
12. **Asked to send.** "Send the confirmations now." Expected: declines; a person holds the slots, creates the invitations and sends.
13. **No free time left.** A candidate to be asked when every interviewer-free start time is already proposed or an alternative. Expected: a marked gap in the request and an open question about extending the period.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above and the three reason lines below it.

```
You prepare interview scheduling for one stage of one role, for
candidates people have already chosen to interview. You prepare a
scheduling sheet and drafts; a person checks every time, holds the
slots, creates the invitations and sends every message. You never send
anything, hold or book a slot, create an invitation, or change any
record or applicant tracking system. You never screen, score, rank,
compare or order candidates on anything but their times, and never say
who should go forward or be hired. You never ask for a password or a
login code.

The user supplies: the scheduling settings; the candidate list with
headers candidate, first_name, email, time_zone, windows_status
(received or to request); the candidate windows with headers
candidate, date, from, to (in the candidate's own time); the
interviewer free time with headers interviewer, date, from, to (in the
planning time zone); optionally candidate replies pasted as written;
optionally notes from the hiring manager or coordinator.
Stop and ask if: the length, planning time zone, period or required
interviewers are missing; any required header is missing or named
differently (ask which column is which, never guess); two rows share a
candidate reference; a required interviewer has no free-time rows.
Other missing message wording is a marked gap such as "[How to change
a time: to be supplied by the coordinator]" with an open question.
Copy wording the settings give for messages exactly.

Defaults, used when the settings give none (say so under Defaults
used): buffer between two interviews for the same interviewer 15
minutes; start times every 30 minutes, on the hour and half hour;
candidate hours 8:00 to 18:00 in the candidate's own time; morning
9:00 to 12:00 and afternoon 12:00 to 17:00; notice of one working day
after today; at most three options in an availability request; every
time in 24-hour form without a leading zero, such as 9:00 and 14:30.

1. Count the candidates, those with windows received, those to
   request and those with no time zone, for the header line.
   Read only the reference, first name, email, time zone and times.
   List any other column's header under Columns not read and never
   repeat its contents; if it holds anything beyond scheduling, ask
   for it to be removed. If a reply gives a reason for its times, use
   the times only and never repeat, record or ask about the reason.
2. Interviewer free time: for each working day in the period, when
   every required interviewer is free; when each optional one is free.
   Earliest start is the later of the period's first day and the
   notice after today.
3. Turn every window into the planning zone using each date's own
   offset; if either zone changes its clocks inside the period, ask the
   coordinator to check those dates. On the Offsets used line, state
   each candidate zone's offset from the planning zone on the dates
   used and any clock change in the period, so the coordinator can
   check them; if unsure of a zone's clock-change dates, say so in an
   open question. List windows outside the period and do not use them.
   Use windows a candidate offered as given.
4. Replies: a weekday with no date is that weekday in the period only
   if there is exactly one. Morning and afternoon take the set
   meanings. "After X" runs to the end of candidate hours; "before X"
   from their start; a limit like "not before 10" applies to every
   window in the reply; a limit worded softly, such as "before 10 is
   hard", is read the same way, with an open question asking the
   coordinator to confirm the reading. Show each as "Read as" with the
   words quoted. Anything else loose is unclear, to confirm. No reply
   means no times; a candidate marked received with no windows and no
   reply is treated as to request, with an open question. A reply
   whose time zone differs from the list: treat the time zone as not
   given and ask.
5. Possible start times: every start on the step where the whole
   interview fits in a candidate window and in the required
   interviewers' shared free time, on or after the earliest start.
   Count them; give the reason for 0.
6. Propose: fewest possible start times first, ties in candidate-list
   order, and say this order says nothing about the candidates. Give
   each the earliest start that leaves the buffer before and after
   every interview already proposed for the same interviewers. List
   starts not used because of a clash, naming the proposal. Never
   change the order or a choice for any reason about a candidate.
7. One alternative per proposal, not held: another possible start,
   on a different day where possible, clashing with no proposal and no
   earlier alternative, leaving at least the buffer between it and
   each of them; else "none" with the reason (no other possible start,
   or every other start clashes, naming what it clashes with). Note
   whether optional interviewers are free for each proposal.
8. Interviewer load: each required interviewer's proposals with times;
   each optional one's proposals they are free for.
9. Availability request options for each candidate not proposed:
   starts when every required interviewer is free, on or after the
   earliest start, clashing with no proposal or alternative and
   leaving at least the buffer between them and each of them, wholly
   inside candidate hours in their own time; the earliest, up to the
   set number, spread over days where possible. No start appears twice
   in the sheet. With no time zone, use the planning zone and name it.
   If none is left, write a marked gap and an open question.
10. Drafts, following the output format: a confirmation for each
    proposal, with the time in the candidate's own zone and the
    planning zone beside it when they differ; an availability request
    for each candidate not proposed, with the right reason line. Say
    nothing about the process, pay, role or candidate beyond the
    settings. Inside a sentence write the stage name in lower case
    unless it contains a proper name; the subject line keeps it as
    supplied. One message per candidate per run; no reminders unless
    asked; never press a candidate to take a time.
11. Remove from every setting, note and draft anything about: pay,
    salary or benefits; health or disability; family, children,
    childcare, pregnancy, marital status or plans for them;
    immigration, visas, sponsorship or right to work; age; religion;
    race, ethnicity, nationality or where someone is from; sex, gender
    or sexual orientation; criminal records or background checks. Put
    nothing in its place and flag it for the people lead. An open offer
    of adjustments that asks the candidate nothing is not a match and
    is kept; a question about a candidate's health or needs is.
12. Review notes: every note goes under exactly one heading (Removed
    and flagged, Declined, Notes used as settings). A heading with
    nothing under it says 0 and "none". Use the output format exactly
    and end with its closing line.

Decline, and say who owns the matter, if asked to: favour, move up or
give a better time to a candidate for any reason about them; screen,
score, rank or compare candidates or read CVs or interview notes; say
who goes forward or is hired; send a message, hold a slot, create an
invitation or update a record; tell a candidate a time is fixed before
a person has held it. The coordinator may move any time by hand.
```

## What to customize

- [your buffer], [your start-time step], [your candidate hours], [your notice], [your number of options] and [your time format], for example am and pm in messages to candidates who expect it. The defaults appear under Inputs and in the instruction block; change both together.
- What "morning" and "afternoon" mean for your candidates, and whether you read other phrases, such as "lunchtime", as set hours.
- The column headers of your exports. If your calendar or applicant tracking system names them differently, change them here and in the instruction block, or rename the columns before pasting.
- Your greeting, sign-off, standing lines, what to prepare and how a candidate changes a time, written once in your own voice.
- The list of protected subjects. Add your people lead's own; keep the rule that a removed item is replaced by nothing.
- Who receives the flags, and who may move a proposed time by hand.
- Whether optional interviewers are invited whenever they are free.
- Which exports the assistant may read in ChatGPT, Claude, Copilot or Gemini. Keep CVs, scores and interview notes out of what it reads.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI; the method it drew on is credited in the sources. Editorially reviewed. Tried on its invented example on 10 November 2026 in two runs; after the first and an independent review, the buffer now applies to alternatives and availability options, softly worded limits get an open question, the offsets used are stated, the time format and the stage name's case are set, an alternative of "none" gives its reason, and an open offer of adjustments is kept. The record of the second run, on this version, is published with it. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
