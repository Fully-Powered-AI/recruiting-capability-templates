# Candidate outreach drafting: a trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-10
- **Template version:** 0.1.0

This is a record of one run of the workflow template on its own invented example. The company, the role, the people and every note are invented, and no client data was used. It shows what the template produced once, on one set of inputs. It is not a test in any company's environment.

This is the second run on the same example. An earlier run the same day showed where the instructions left room to guess; the instructions and the example were revised, and the run recorded here was made on the revised instructions. What the earlier run found, and what was changed, is at the end.

## The inputs used

The inputs are exactly the six in `public/example.md`, under "The inputs": the role brief for the senior data engineer at Company A, the company facts page, the approach list of five invented people, the two-entry do-not-contact list, the two-line reply log and the settings. No client data was used.

The run was a fresh session started from Claude Code with no tools, no access to any file and its customizations switched off. Its instructions were the fenced instruction block and the output format from `member/template.md`, exactly as they now stand; its one message was the six inputs, copied from `public/example.md`. It saw neither the example's output nor the earlier run, and it did not write or revise the template. The revisions after the earlier run were made in a separate session of the same model.

## What came out

The complete output, as returned:

```
CANDIDATE OUTREACH: Senior data engineer
Status: Drafts for Sam R. Nothing has been sent. Sam R. chose who is approached and sends every message.
Prepared for: Sam R., co-founder and CEO. Date: 10 November 2026. First send planned: Thursday 12 November 2026.
Role: Senior data engineer, Data platform. Approved by: the board, 3 November 2026. Allowed in messages: pay range; location and pattern; hiring steps.
Schedule: first message day 0, follow-up 1 day 4, follow-up 2 day 10, in working days.

CHECKS BEFORE DRAFTING
Approach list: 5 people supplied. Drafted: 3. Not drafted: 2.
Do-not-contact list: 2 entries checked.
Reply log: 2 entries read.

NOT DRAFTED
P3: on the do-not-contact list.
P5: paused until 31 March 2027.

PERSON P1, Dana, by email
Personal line from: wrote about rebuilding a check for late-arriving data in a parcel-tracking pipeline (article on Blog B, a public engineering blog, June 2026).
Referred by: none.

FIRST MESSAGE, day 0, Thursday 12 November
Subject: Senior data engineer role
Hi Dana,
I read your article on Blog B about rebuilding a check for late-arriving data in a parcel-tracking pipeline. It relates closely to what our data platform team works on: the pipelines that turn delivery scans and GPS pings into the arrival estimates drivers see.
I'm Sam R., co-founder and CEO of Company A. We build route-planning software for regional delivery firms; about 140 of them use it every day. We're hiring a senior data engineer for that team of four data engineers and an analyst.
Would you be open to a 30-minute call? If so, reply with a time that suits you.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

FOLLOW-UP 1, day 4, Wednesday 18 November. Adds: pay range, with location and pattern. Send only if there has been no reply.
Subject: Senior data engineer role
Hi Dana,
I wrote recently about a senior data engineer role at Company A, where we build route-planning software for regional delivery firms. The data platform team runs the pipelines that turn delivery scans and GPS pings into the arrival estimates drivers see. The pay range is $165,000 to $185,000 a year; the role is remote within the US, with two team days a month in Denver.
If a 30-minute call would help, reply with a time that suits you.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

FOLLOW-UP 2, day 10, Monday 30 November. The last message. Adds: hiring steps. Send only if there has been no reply.
Subject: Senior data engineer role
Hi Dana,
This is my last message about the senior data engineer role on Company A's data platform team, which builds the pipelines behind the arrival estimates drivers see. For reference, the hiring steps are a 30-minute call, a paid take-home task, then a half-day with the team.
If you'd ever like to talk, reply with a time that suits you. Either way, I wish you well.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

PERSON P2, Luis, by profile message
Personal line from: none, see Details not used.
Referred by: none.

FIRST MESSAGE, day 0, Thursday 12 November
Subject: none, profile message
Hi Luis,
I'm Sam R., co-founder and CEO of Company A. We build route-planning software for regional delivery firms; about 140 of them use it every day. We're hiring a senior data engineer for our data platform team, four data engineers and an analyst who build the pipelines that turn delivery scans and GPS pings into the arrival estimates drivers see.
Would you be open to a 30-minute call? If so, reply with a time that suits you.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

FOLLOW-UP 1, day 4, Wednesday 18 November. Adds: pay range, with location and pattern. Send only if there has been no reply.
Subject: none, profile message
Hi Luis,
I wrote recently about a senior data engineer role at Company A, where we build route-planning software for regional delivery firms. The data platform team runs the pipelines that turn delivery scans and GPS pings into the arrival estimates drivers see. The pay range is $165,000 to $185,000 a year; the role is remote within the US, with two team days a month in Denver.
If a 30-minute call would help, reply with a time that suits you.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

FOLLOW-UP 2, day 10, Monday 30 November. The last message. Adds: hiring steps. Send only if there has been no reply.
Subject: none, profile message
Hi Luis,
This is my last message about the senior data engineer role on Company A's data platform team, which builds the pipelines behind the arrival estimates drivers see. For reference, the hiring steps are a 30-minute call, a paid take-home task, then a half-day with the team.
If you'd ever like to talk, reply with a time that suits you. Either way, I wish you well.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

PERSON P4, Amara, by email
Personal line from: maintains an open-source library for validating GPS data (the library's public code repository, August 2026).
Referred by: Jo P.

FIRST MESSAGE, day 0, Thursday 12 November
Subject: Senior data engineer role
Hi Amara,
Jo P., one of our data engineers, passed on your name.
I saw the open-source library you maintain for validating GPS data, in its public code repository. GPS data is part of what our data platform team works on: the pipelines that turn delivery scans and GPS pings into the arrival estimates drivers see.
I'm Sam R., co-founder and CEO of Company A. We build route-planning software for regional delivery firms; about 140 of them use it every day. We're hiring a senior data engineer for that team of four data engineers and an analyst.
Would you be open to a 30-minute call? If so, reply with a time that suits you.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

FOLLOW-UP 1, day 4, Wednesday 18 November. Adds: pay range, with location and pattern. Send only if there has been no reply.
Subject: Senior data engineer role
Hi Amara,
I wrote recently about a senior data engineer role at Company A, where we build route-planning software for regional delivery firms. The data platform team runs the pipelines that turn delivery scans and GPS pings into the arrival estimates drivers see. The pay range is $165,000 to $185,000 a year; the role is remote within the US, with two team days a month in Denver.
If a 30-minute call would help, reply with a time that suits you.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

FOLLOW-UP 2, day 10, Monday 30 November. The last message. Adds: hiring steps. Send only if there has been no reply.
Subject: Senior data engineer role
Hi Amara,
This is my last message about the senior data engineer role on Company A's data platform team, which builds the pipelines behind the arrival estimates drivers see. For reference, the hiring steps are a 30-minute call, a paid take-home task, then a half-day with the team.
If you'd ever like to talk, reply with a time that suits you. Either way, I wish you well.
Sam R.
Co-founder and CEO, Company A
If you'd rather not hear from Company A about roles, reply "no thanks" and we won't contact you again.

DETAILS NOT USED
P2: the detail comes from a personal account and is about personal life, not work. It is not used and not repeated here. Remove it from the approach list.

REPLY LOG
P1: Status: to send. Sent: none yet. Latest reply: none. Next: Sam R. sends the first message, Thursday 12 November 2026.
P2: Status: to send. Sent: none yet. Latest reply: none. Next: Sam R. sends the first message, Thursday 12 November 2026.
P3: Status: not drafted. Sent: none yet. Latest reply: none. Next: none.
P4: Status: to send. Sent: none yet. Latest reply: none. Next: Sam R. sends the first message, Thursday 12 November 2026.
P5: Status: paused until 31 March 2027. Sent: first message, 2 November 2026. Latest reply: 4 November 2026, not now. Next: Sam R. decides whether to write again, on or after Wednesday 31 March 2027.

FOR THE DO-NOT-CONTACT LIST
For the do-not-contact list: none.

WHAT ENDS THE MESSAGES
Any reply: no further follow-up to that person, on any channel; Sam R. answers.
Interested: Sam R. takes it from there; nothing further is drafted.
Not now: paused until the date they gave, or 6 months after the reply; Sam R. decides then whether to write again.
Declined: nothing further about this role.
Opt-out or a request not to be contacted: nothing further about any role; added to the do-not-contact list by Sam R.
Away message: follow-ups held until the return date; run again after it.
Bounced: stopped; no other address is looked for.

READ BEFORE SENDING
- all: follow-up dates assume the first message goes on Thursday 12 November and skip Thursday 26 and Friday 27 November. If the first send moves, the follow-up dates need redoing.
- all: send each follow-up only if there has been no reply on any channel. A "no thanks" reply means stop and add the person to the do-not-contact list.
- P1: the message says "I read your article". Send it only if you have read it yourself, or change the wording.
- P4: the message says "I saw the library" and names Jo P. Check that you have looked at the repository yourself and that Jo P. is happy to be named.
- P2: remove the personal detail from the approach list. The messages contain no personal line. Check the profile site's message length limit. The opt-out line must stay in.
- P3: nothing drafted. Leave this person out of any later approach list for this role.
- P5: your hand-written first message was sent on 2 November and is not redrafted. No follow-ups go out while the pause runs to 31 March 2027.

SLOTS FOR SAM R.
- Slots for Sam R.: none. The facts page gave the opt-out line, and each person drafted has a greeting name.

DEFAULTS USED
- Follow-up gaps: follow-up 1 four working days after the first message, follow-up 2 six working days after follow-up 1.
- Word limits: 120 words for a first message, 80 for a follow-up, counted between the greeting and the sign-off.
- Freshness limit: 24 months.
- Revisit gap: 6 months.
- Booking route: none on the facts page, so the call ask asks for a reply with a time.

Drafts for Sam R. Nothing has been sent or scheduled, no one has been looked up, and no one has been assessed, scored or put in order.
```

Word counts, from the line after the greeting to the line before the sign-off, with every line counted (P4's referrer line included), counted by a small script after the run: first messages 102 (P1), 76 (P2) and 112 (P4); each follow-up 1 is 78 words and each follow-up 2 is 65. All are within the default limits of 120 and 80.

## What was observed

- **Every required part was produced.** All sections of the output format are present, in order, and the empty one says "none". Three people were drafted with three dated messages each. P3 was left out as an exact do-not-contact match, with no reason given. P5 was left out as paused until 31 March 2027, the date in the log, and the first message Sam R. sent by hand is shown under Sent and not redrafted. All five people have a reply log line. No stop condition applied, and nothing was sent.
- **The revised rules were followed.** The header lists the allowed items separated by semicolons. Each greeting is "Hi" with the greeting name. The body names the sender as "Sam R.", as the facts page gives it. The first messages carry none of the items the brief allows. Follow-up 1 adds the pay range with the location and pattern as one item, follow-up 2 adds the hiring steps, and the facts-page line about the team is not used because the brief allows both. P4's personal line runs to two sentences, which the revised step allows.
- **The same decisions as the published example.** Who was drafted and who was not, the dates (day 0 Thursday 12 November, day 4 Wednesday 18 November, day 10 Monday 30 November, with the 26 and 27 November non-working dates skipped), which details were used, what each follow-up added and the defaults used all match.
- **Differences from the published example.** All are wording or layout, none is a rule difference:
  - The run gave all three email messages the same subject, "Senior data engineer role". The example uses three different subjects.
  - The run's follow-ups restate what the company does and what the team works on before adding the new item, so they run to 78 and 65 words against the example's 51 and 49.
  - The run's last messages end "Either way, I wish you well"; the example's end "Wishing you a good end to the year".
  - For P2 the run gives the reason "is about personal life, not work"; the example says "is not about work". Both repeat nothing of the detail itself.
  - The run's reply log gives only the first send date as the next action; the example adds the follow-up dates.
  - "Read before sending" differs. The run asks Sam R. to send P1's and P4's messages only if Sam R. has read the article and looked at the repository in person, since the messages say so, and lists notes for P2, P3 and P5. The example asks for the article and the repository to be checked as still public and for the "about 140" figure to be checked as still true.
  - The run lists the missing booking route under Defaults used, although it is a rule under the facts page rather than a setting; the example mentions it under Slots instead.
- **Things in the output that are not in the inputs.** "It relates closely to what our data platform team works on" (P1) is a judgement the inputs support only loosely; the example's "which is close to the pipeline work our data platform team does" is the same kind of judgement. The note under Read before sending for P3, "leave this person out of any later approach list for this role", understates the do-not-contact list, which applies to every role. The note to check the profile site's message length is advice the inputs do not give. In the example, "Wishing you a good end to the year" assumes a calendar context. Every other line in both outputs traces to the inputs.

### Where the template still leaves room to guess

- **Subjects.** The template does not say whether a follow-up's subject should differ from the first message's. The run used one subject for all three.
- **What a follow-up repeats.** Step 7 says a follow-up stands alone, but not how much of the company and team it restates. The run restated both, which brought follow-up 1 close to its limit.
- **Defaults used.** It is not said whether the no-booking-route rule belongs under Defaults used; the run put it there.
- **Reply log, next action.** It is not said whether the follow-up dates belong in the next action. The run gave only the first send.

### Shortcomings

- No instruction was misleading, and no stop condition was hit. The output format and the instruction block agree with each other.
- The P3 note "for this role" is a small slip by the run, not a gap in the template: the template says the do-not-contact list means nothing is drafted, without limit to one role. A sender reading the pack should take the list as covering every role.
- This is one run, by one model, on an invented example. It shows the revised instructions can be followed to a complete and consistent pack. It does not show the template works in a real hiring setting, in other products, or on messy real exports. Of the acceptance tests in the template, only test 1 has the shape of this example; the others were not run.

## The earlier run, and what was changed

**First run** (Claude Sonnet 5.5, 10 November 2026, a session that had not written the template; it read the template and the example's inputs, produced its output, and only then read the example's output). It produced every part of the pack and made the same decisions as the example: the same people drafted and not drafted, the same dates, the same details used and the same item added by each follow-up. It found these gaps:

- the template did not give the word before the greeting name, and the model added "Hi";
- the facts page gives "Sam R.", and the template did not say which form of the name the body uses; the example then said "I'm Sam";
- it was not said whether a first message may carry the location and pattern the brief allows;
- it was not said whether the pay range and the location and pattern count as one new thing in follow-up 1;
- the facts-page line about the team was never reached when the brief allows both the practical details and the hiring steps, and the template did not say so;
- it was not said whether a referrer line counts toward the word limit;
- the step asked for "one sentence" for the personal line, which both the run and the example exceeded once the link to the team's work was added;
- the output format's header listed the allowed items with slashes while the example used semicolons;
- the example's subject "delivery data platform" was not in the inputs, and its reason for P2, "about family life, not work", repeated more than needed;
- the version notes still said the template had not been tried.

It also noted points that were left as they were: whether the schedule's day numbers count skipped dates (they do not), how to treat a team fact the facts page restricts, whether a pause or reply date is shown under Not drafted, and whether the reply log's next action repeats a request to remove a personal detail.

**What was changed after it.** The procedure and the instruction block now say: the greeting is "Hi", then the greeting name and a comma; the body names the sender exactly as the facts page gives it, with their title; the personal line may be one or two short sentences; the first message carries none of the items the brief allows and not the facts-page line about the team; in follow-up 1 the pay range and the location and pattern count together as one item; the facts-page line about the team is not used when the brief allows both other items; and every line between the greeting and the sign-off counts toward the word limit, the referrer line included, the subject not. The output format's header now asks for the allowed items separated by semicolons. In the example, the two subjects became "Senior data engineer, data platform team", the body says "I'm Sam R.", the reason for P2 became "is not about work", and the word counts were redone. The version notes and the profile now say the template was tried. The run above was then made on the revised instructions.
