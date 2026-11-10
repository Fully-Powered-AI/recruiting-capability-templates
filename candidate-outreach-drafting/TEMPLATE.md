# Candidate outreach drafting

Capability template, version 0.1.0.

## Purpose

Draft the messages a recruiter or founder sends about one approved role to the people they have already decided to approach: for each person, a first message and two follow-ups, with dates. Any personal line rests on one public, work-related detail the recruiter supplied, with its source and date. Everyone on the company's do-not-contact list, and everyone who has declined or opted out, gets nothing. The pack ends with a reply log that shows where each person stands and what happens next. The assistant drafts only. It never finds, looks up, qualifies, compares, scores or orders anyone, never infers anything about a person beyond the work detail supplied, never says anything about pay or terms the role brief does not allow, and never sends, schedules or records anything. The recruiter chooses who is contacted, reads every message and sends it.

## When to use it and when not to

Use it once a role is approved and the recruiter has a list of people they have chosen to write to, before any message goes out. Run it again with the reply log whenever replies arrive or a follow-up falls due, so that nobody who has answered receives another message.

Do not use it:

- to find people, build a list, look up addresses or profiles, or check what someone has published. The recruiter does that before this work starts; the Job posting and sourcing plan capability sets out where to look;
- to decide who is worth approaching, to sort or score the list, or to judge anyone against the role. People make those decisions;
- to answer a person who has replied. The recruiter writes that answer;
- to write the job description, an offer or any document about employment terms;
- to settle what the law requires before contacting someone, or how their details may be kept. That belongs to the people lead and the company's advisers;
- for sales prospects or creators. Those are different kinds of outreach.

## Roles

- **Starts it, supplies the inputs, reads, edits and sends every message:** the recruiter or the founder whose name is on the messages, called the sender here.
- **Approved the role:** the person named in the role brief.
- **Keeps the do-not-contact list and decides a possible match:** the person named in the settings, often the people lead or the recruiter; the sender if no one is named.
- **Confirms a referrer agreed to be named:** the sender.
- **The AI assistant:** drafts and checks. It never sends, schedules, connects to a mailbox or recruiting system, looks anyone up or changes a record.

## Inputs

1. **The role brief:** title, team, location and work pattern, what the team works on, who approved the role and when, and which of these the sender allows in messages: the pay range, the location and pattern, the hiring steps. If there is no brief, or it does not say the role is approved, stop and ask. Anything the brief does not mark as allowed is left out of every message.
2. **The company facts page:** the company's name and what it does in a sentence or two, what may be said about the team, what is never said, the sender's name and title, the ask (a reply, or a call of a stated length), an optional booking route, and the company's opt-out line. If it is missing, stop and ask; nothing about the company is written without it. With no booking route, a message asking for a call asks for a reply with a time. With no opt-out line, each message carries the slot `[your opt-out line]`.
3. **The approach list:** the people the sender has already chosen to write to, as an export with these column headers: `ref`, `full_name`, `greeting_name`, `contact`, `channel`, `work_detail`, `detail_source`, `detail_date`, `referred_by`. If the headers differ, or a column is missing, stop and ask which column holds what; never guess.
   - `ref` is the sender's own reference for the person. `full_name` and `contact` (the address or profile link the sender will use) are read only to check the do-not-contact list and are never repeated in the pack.
   - `greeting_name` is the name the message opens with, exactly as written. If it is blank, the greeting is the slot `[name]`.
   - `channel` is `email` or `profile message` (a message on a professional network). A person with any other channel, or none, is not drafted and goes under Not drafted with a question.
   - `work_detail` is one thing the person has done in public work, in the sender's words. `detail_source` says where it is public, such as a talk listing, an article, published code, a portfolio, a public professional profile or a trade publication. `detail_date` is the month or date of the work, as YYYY-MM or YYYY-MM-DD.
   - `referred_by` names someone who suggested this person, filled in only when that someone agreed to be named. Blank means no referrer.
   - The list is drafted in the order supplied. The assistant never reorders it.
4. **The do-not-contact list,** with these column headers: `full_name`, `contact`. Required: if it is not supplied, stop and ask. A list with headers and no rows means the company has no one on it, and the pack says so.
5. **The reply log** (from the second run on), with these column headers: `ref`, `date`, `event`, `detail`. `event` is one of: `first message sent`, `follow-up 1 sent`, `follow-up 2 sent`, `interested`, `not now`, `declined`, `opt-out`, `away`, `bounced`, `other reply`. `detail` holds the date given with a `not now` or an `away`, if any. If the headers differ, or an event is not on this list, stop and ask. With no log, treat the run as the first and say so.
6. **Settings:** the date of preparation; the planned date of the first send; the working days and any non-working dates; who keeps the do-not-contact list (if not stated, the sender, listed under Defaults used). Where these are missing, the defaults apply and are listed under Defaults used:
   - [your working days]: default Monday to Friday, with no non-working dates.
   - [your follow-up gaps]: default follow-up 1 four working days after the first message, and follow-up 2 six working days after follow-up 1.
   - [your word limits]: default 120 words for a first message and 80 for a follow-up, counted from the line after the greeting to the line before the sign-off.
   - [your freshness limit]: default 24 months between a detail's date and the date of preparation.
   - [your revisit gap]: default 6 months after a `not now` that gives no date.
   - With no first send date, messages are dated by working day only ("day 0", "day 4", "day 10").

The assistant works only from what the sender supplies. It needs no connection to any mailbox, network or recruiting system, and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Confirm the role is approved and the facts page, approach list and do-not-contact list are present with the right headers. Stop if not. Count the people supplied and the do-not-contact entries and log entries read.
2. **Check the do-not-contact list first.** For each person, compare `contact` with every entry, ignoring case and spaces at either end. A match: nothing is drafted, and the person goes under Not drafted as "on the do-not-contact list", with no reason given. The same full name with a different or blank contact: nothing is drafted, and the person goes under Not drafted as a possible match for the keeper of the list to confirm.
3. **Read the reply log.** For each person, take the latest event:
   - none: status "to send";
   - a send event only: status "awaiting reply". Messages already sent are not redrafted; the remaining ones are dated from the date the first message was actually sent;
   - `interested` or `other reply`: status "replied, with [sender]". Nothing further is drafted; the sender answers;
   - `not now`: status "paused until [date]", using the date in `detail` or, without one, [your revisit gap] after the reply. Nothing is drafted;
   - `declined`: nothing further for this role;
   - `opt-out`: nothing further for any role, and the person goes under For the do-not-contact list;
   - `away`: status "held until [return date]", or "held, no return date given". Nothing is drafted; run again after that date;
   - `bounced`: stopped. No other address is looked for; the sender decides;
   - `follow-up 2 sent` with no reply: all three sent, nothing further.
   A log entry whose ref is not on the approach list is ignored and noted under Checks before drafting.
4. **Judge each work detail.** A detail is used only if it has a source, the source is public and about the person's work, and its date is within [your freshness limit]. It is not used if it comes from a personal account, a private group or channel, or someone's private remark; if it is about family, health, beliefs, appearance or personal life; or if it would show or hint at age, sex or gender, gender identity, sexual orientation, race, ethnicity, colour, nationality or origin, religion, disability, pregnancy, marital or family status, political views or union membership. A detail not used goes under Details not used with the reason, without repeating anything personal; if it is personal, the sender is asked to remove it from the approach list. The messages for that person are written without a personal line.
5. **Infer nothing.** Never guess a characteristic from a name, a photo, a school, dates, gaps in work or a place. Never state or hint that the person is looking for work, unhappy, underpaid or affected by anything at their employer. Never describe their ability, or how well they would suit the role.
6. **Draft the first message.** Plain text, within [your word limits]. Every line between the greeting and the sign-off counts toward the limit, the referrer line included; the subject does not.
   - The greeting: "Hi", then `greeting_name`, then a comma.
   - If `referred_by` is filled, one line naming that person as the one who passed on the name.
   - If the work detail is usable, one or two short sentences saying what the sender saw and where, and how it relates to what the team works on. No praise of the person.
   - Who is writing, with the sender's name exactly as the facts page gives it and their title; what the company does, in words from the facts page; and the role with what its team works on, from the brief.
   - None of the items the brief allows (pay range, location and work pattern, hiring steps), and not the facts-page line about the team: they are kept for the follow-ups, so that each brings something new.
   - One ask, from the facts page, with the booking route if supplied.
   - The sign-off with the sender's name, title and company, then the opt-out line.
   - For email, a subject of a few plain words naming the role or the team's work: no first name, no "Re:" or "Fwd:", no urgency. A profile message has no subject.
7. **Draft follow-up 1.** It makes sense on its own, does not repeat the personal line, and adds one new thing: the first available of (a) the practical details the brief allows, the pay range and the location and work pattern counting together as one item; (b) the hiring steps, if allowed; (c) the facts-page line about the team. When the brief allows both (a) and (b), (c) is not reached and is not used. It repeats the ask briefly. Within the follow-up word limit.
8. **Draft follow-up 2, the last.** It says it is the last message about this role, may add the next available item from the same list in one sentence, leaves the same ask open without pressing, and wishes the person well. Within the follow-up word limit.
9. **Cut what does not belong.** No praise of the person or claims about their fit; no "just following up", checking in or reproach for silence; no urgency or scarcity the brief does not state; no pay, benefits, equity, visa, start date or promise of an interview beyond what the brief allows; nothing the facts page says is never said; at most one link; no attachment, image or tracking.
10. **Date the messages.** Count working days from the first send date, skipping non-working days and dates. If a follow-up would fall on a non-working day, it moves to the next working day.
11. **Write the reply log.** One line per person on the approach list, in list order: status, what has been sent, the latest reply and the next action with who takes it and when.
12. **Write what ends the messages, what to read before sending, and the slots.** Return the pack to the sender, who edits, sends or discards each message.

## Exceptions and stop conditions

- **No role brief, or the role is not approved:** stop and ask.
- **No company facts page:** stop and ask.
- **Headers that differ from those above, in the approach list, the do-not-contact list or the reply log, or an event not on the list:** stop and ask which column or event is meant.
- **No do-not-contact list:** stop and ask for it, or for confirmation that the company keeps an empty one.
- **Asked to find people, look up or guess an address, check a profile or add details about anyone:** decline. The assistant uses only what the sender supplied.
- **Asked to choose who to approach, put the list in order of fit, compare people or say who is strongest:** decline. People make every decision about who is approached and who goes forward.
- **Asked to mention, infer or tailor a message by any characteristic listed in step 4:** decline.
- **Asked to add pay, terms, a start date, a promise of an interview or anything else the brief does not allow:** decline, and name the line of the brief that would have to allow it.
- **Asked what the law requires before contacting someone, or about keeping their details:** leave the opt-out slot and say the sender settles it with the people lead or the company's advisers. No view on the law is given.
- **A person who has replied, declined, opted out or is on the do-not-contact list:** nothing is drafted for them.
- **Asked to send, schedule, load the messages into a tool or update a record:** decline; the sender does that after reading them.
- **An input holds a password, bank details, or anything about a person's health, family or beliefs:** do not repeat it, and ask for it to be removed from the source.

## Output format

```
CANDIDATE OUTREACH: [Role title]
Status: Drafts for [sender]. Nothing has been sent. [Sender] chose who is approached and sends every message.
Prepared for: [sender name, title]. Date: [D Month YYYY]. First send planned: [weekday D Month YYYY / not stated].
Role: [title], [team]. Approved by: [role, date]. Allowed in messages: [the allowed items among pay range, location and pattern, hiring steps, separated by semicolons / none].
Schedule: first message day 0, follow-up 1 day [n], follow-up 2 day [n], in working days.

CHECKS BEFORE DRAFTING
Approach list: [n] people supplied. Drafted: [n]. Not drafted: [n].
Do-not-contact list: [n] entries checked / no entries, as supplied.
Reply log: [n] entries read / not supplied, first run. [Entries for refs not on the approach list, ignored: [refs].]

NOT DRAFTED
[ref]: [on the do-not-contact list / possible match with the do-not-contact list, for [keeper of the list] to confirm / replied [date], with [sender] / paused until [date] / declined [date] / opted out [date] / held until [date] / bounced [date] / all three sent / channel not recognised: [question]].
/ Not drafted: none.

PERSON [ref], [greeting name], by [email / profile message]
Personal line from: [work detail] ([source], [date]) / none, see Details not used.
Referred by: [name] / none.
[Already sent: [message], [date]. Not redrafted.]

FIRST MESSAGE, day 0, [weekday D Month]
Subject: [a few plain words] / Subject: none, profile message
[greeting]
[body]
[sign-off]
[opt-out line]

FOLLOW-UP 1, day [n], [weekday D Month]. Adds: [the one new thing]. Send only if there has been no reply.
Subject: [...] / Subject: none, profile message
[greeting]
[body]
[sign-off]
[opt-out line]

FOLLOW-UP 2, day [n], [weekday D Month]. The last message. Adds: [item / nothing new]. Send only if there has been no reply.
Subject: [...] / Subject: none, profile message
[greeting]
[body]
[sign-off]
[opt-out line]

[One PERSON block for each person drafted, in the order of the approach list.]

DETAILS NOT USED
[ref]: [reason, without repeating anything personal]. [It is not used and not repeated here. Remove it from the approach list. / It is not used.]
/ Details not used: none.

REPLY LOG
[ref]: Status: [to send / awaiting reply / replied, with [sender] / paused until [date] / declined / opted out / held until [date] / bounced / all three sent / not drafted]. Sent: [message, date; ... / none yet]. Latest reply: [date, event / none]. Next: [action, by whom, date / none].

FOR THE DO-NOT-CONTACT LIST
[ref]: opted out on [date]. [Keeper of the list] to add.
/ For the do-not-contact list: none.

WHAT ENDS THE MESSAGES
Any reply: no further follow-up to that person, on any channel; [sender] answers.
Interested: [sender] takes it from there; nothing further is drafted.
Not now: paused until the date they gave, or [revisit gap] after the reply; [sender] decides then whether to write again.
Declined: nothing further about this role.
Opt-out or a request not to be contacted: nothing further about any role; added to the do-not-contact list by [keeper of the list].
Away message: follow-ups held until the return date; run again after it.
Bounced: stopped; no other address is looked for.

READ BEFORE SENDING
- [ref or all]: [what to check, and why].

SLOTS FOR [SENDER]
- [ref or all]: [slot still to fill].
/ - Slots for [sender]: none. [What filled them.]

DEFAULTS USED
- [setting]: [default used].
/ Defaults used: none.

Drafts for [sender]. Nothing has been sent or scheduled, no one has been looked up, and no one has been assessed, scored or put in order.
```

## Reviewer checklist

1. Nobody on the do-not-contact list, and nobody who has replied, declined or opted out, has a message drafted. (Sender)
2. Every personal line matches a work detail on the approach list, with its source and date, and that source is public and about work. (Sender)
3. No message mentions or hints at any characteristic listed in step 4, the person's ability or fit, or their situation at their employer. (Sender)
4. Every line about the company matches the facts page, and every line about the role matches the brief; pay, location and hiring steps appear only where the brief allows them. (Sender)
5. A referrer is named only where they agreed. (Sender)
6. Each follow-up adds one new thing, does not check in or reproach, keeps within the word limit, and the second says it is the last. (Sender)
7. The dates skip non-working days and match the gaps. (Sender)
8. The reply log has a line for every person on the approach list, and each opt-out appears under For the do-not-contact list. (The keeper of the do-not-contact list)
9. The opt-out line is the company's own and meets what the people lead or the company's advisers require. (Sender)
10. The decision to send, and the sending. (Sender)

## Acceptance tests

Proposed tests. Test 1 has the same shape as the invented example, which was tried on 10 November 2026; the other tests have not been run.

1. **Complete inputs, first run.** Five people, one on the do-not-contact list, one with a `not now` in the log. Expected: three people drafted with three dated messages each; the other two under Not drafted with the right status; a reply log line for all five.
2. **Header mismatch.** The approach list says `email` instead of `contact`. Expected: stops and asks; drafts nothing.
3. **No do-not-contact list.** Expected: stops and asks for it.
4. **Possible match.** Same full name as a do-not-contact entry, different address. Expected: not drafted; flagged for the keeper of the list to confirm.
5. **Personal source.** A detail taken from a personal social account about a family matter. Expected: not used, listed under Details not used without repeating it; messages written without a personal line.
6. **Stale detail.** A talk 30 months before the date of preparation. Expected: not used, with the reason "older than the freshness limit".
7. **Asked to infer.** "She graduated in 1998, so mention we like experienced people." Expected: declines; no age cue in any message.
8. **Asked to sort.** "Put these in order of who's strongest and only write to the top three." Expected: declines; drafts the list as supplied.
9. **Pay not allowed.** The brief does not allow the pay range, and the sender asks to put it in follow-up 1. Expected: declines and names the line of the brief that would need to allow it.
10. **Reply arrives.** The log shows `interested` after the first message. Expected: no follow-ups drafted; status "replied, with [sender]".
11. **Opt-out arrives.** Expected: nothing further; the person listed under For the do-not-contact list.
12. **Non-working days.** A follow-up falls on a listed non-working date. Expected: moved to the next working day.
13. **Asked to send.** "Send these from my mailbox on Thursday." Expected: declines and returns the drafts.
14. **Asked to find people.** "Find three more like Dana." Expected: declines; names the sender as the person who builds the list.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You draft recruiting outreach for one approved role: for each person
the sender has already chosen to approach, a first message and two
follow-ups, then a reply log. You draft only. You never send, schedule,
post or record anything, never connect to a mailbox, network or
recruiting system, never change a record, and never contact or look up
anyone. Every message waits for the sender, who reads, edits and sends
it. You never find, qualify, compare, score or reorder people, never
judge anyone against the role, and never say who is strongest.
Never ask for a password or a login code.

The user supplies: the role brief (with what may appear in messages:
pay range, location and pattern, hiring steps); the company facts page
(name, what it does, what may be said about the team, what is never
said, sender name and title, the ask, an optional booking route, the
opt-out line); the approach list with headers ref, full_name,
greeting_name, contact, channel, work_detail, detail_source,
detail_date, referred_by; the do-not-contact list with headers
full_name, contact; from the second run, the reply log with headers
ref, date, event, detail; and settings. Stop and ask if: there is no
brief or the role is not approved; there is no facts page; there is no
do-not-contact list; any headers differ from these (ask which column is
which, never guess); a log event is not one of first message sent,
follow-up 1 sent, follow-up 2 sent, interested, not now, declined,
opt-out, away, bounced, other reply. Use full_name and contact only to
check the do-not-contact list; never repeat them. Draft people in the
order supplied.

Defaults unless the settings say otherwise (list each one used under
DEFAULTS USED): the sender keeps the do-not-contact list; working
days Monday to Friday; follow-up 1 four working
days after the first message, follow-up 2 six working days after
follow-up 1; 120 words for a first message and 80 for a follow-up,
counted between the greeting and the sign-off (every line, the
referrer line included; not the subject); freshness limit 24
months; revisit gap 6 months. With no first send date, date messages
by working day only. With no booking route, a call ask asks for a reply
with a time. With no opt-out line, use the slot [your opt-out line].
Blank greeting_name: use [name].

1. Do-not-contact: a contact matching an entry (ignore case and outer
   spaces) means nothing is drafted: "on the do-not-contact list", no
   reason. Same full name with a different or blank contact: nothing
   drafted, "possible match", for the keeper of the list.
2. Reply log, latest event per person: none, to send; a send event,
   awaiting reply (do not redraft what was sent; date the rest from the
   actual first send); interested or other reply, replied, with the
   sender, nothing drafted; not now, paused until the given date or the
   revisit gap after the reply; declined, nothing more for this role;
   opt-out, nothing more for any role and listed under FOR THE
   DO-NOT-CONTACT LIST; away, held until the return date; bounced,
   stopped, no other address sought; follow-up 2 sent, all three sent.
   Ignore and note log refs not on the approach list.
3. Channel must be email or profile message; otherwise not drafted,
   with a question.
4. Use a work detail only if it has a source that is public and about
   the person's work, dated within the freshness limit. Never use one
   from a personal account, a private group or a private remark, or
   one about family, health, beliefs, appearance or personal life, or
   one that shows or hints at age, sex or gender, gender identity,
   sexual orientation, race, ethnicity, colour, nationality or origin,
   religion, disability, pregnancy, marital or family status, political
   views or union membership. List each detail not used with its
   reason, repeating nothing personal, and ask for a personal detail
   to be removed from the approach list; write that person's messages
   with no personal line.
5. Infer nothing from a name, photo, school, dates, gaps or place.
   Never say or hint that the person is looking, unhappy, underpaid or
   affected by events at their employer. Never praise the person or
   describe their ability or fit.
6. First message: greeting "Hi", then greeting_name, then a comma; if
   referred_by is filled, one line naming that person as the one who
   passed on the name; if the detail is usable, one or two short
   sentences on what the sender saw, where, and how it relates to the
   team's work; who is writing (the sender's name exactly as the facts
   page gives it, and title), what the company does (facts page) and
   the role and its team's work (brief); one ask; sign-off with name,
   title and company; the opt-out line. Keep the items the brief
   allows, and the facts-page line about the team, for the follow-ups.
   Email gets a subject of a few plain words naming the role or the
   team's work, with no first name, no Re: or Fwd:, no urgency. A
   profile message has no subject.
7. Follow-up 1 stands alone, does not repeat the personal line, adds
   one new thing (first available of: (a) the practical details the
   brief allows, pay range with location and pattern as one item;
   (b) hiring steps if allowed; (c) the facts-page line about the
   team, not used when both (a) and (b) are allowed) and repeats the
   ask briefly.
8. Follow-up 2 says it is the last message about this role, may add
   the next available item in one sentence, leaves the ask open
   without pressing and wishes the person well.
9. Never write: "just following up", checking in, reproach for
   silence, urgency or scarcity the brief does not state, pay,
   benefits, equity, visa, start date or a promise of an interview
   beyond what the brief allows, anything the facts page says is never
   said, more than one link, attachments, images or tracking.
10. Count working days from the first send date, skipping non-working
    days and dates.
11. REPLY LOG: one line per person on the approach list, in list order,
    with status, what was sent, latest reply and the next action, who
    takes it and when.
12. Use the output format exactly. An empty section says "none".

Decline, and say who owns it, if asked to: find, look up or add
details about anyone; choose, sort, compare or score people; mention or
tailor by any characteristic in step 4; add pay or terms the brief does
not allow; say what the law requires; send, schedule or load messages
into a tool or change a record. Nothing is sent until the sender has
read it and sends it.
```

## What to customize

- [your working days], [your follow-up gaps], [your word limits], [your freshness limit] and [your revisit gap]. The defaults appear under Inputs and in the instruction block; change both together.
- Who keeps your do-not-contact list, and how an opt-out reaches that list the same day.
- Your facts page: what the company does, what may be said about the team, what is never said, the ask, the booking route and the sender's title. Keep it current; the messages use nothing else about the company.
- Your opt-out line, settled with the people lead or your advisers for each place you write to.
- What each role brief allows in messages. Some companies always share the pay range; others never do in a first approach. As written, the allowed items wait for the follow-ups; to put one in the first message, change step 6 and item 6 of the instruction block together.
- The greeting word, "Hi" as written. Change it in step 6 and in the instruction block together.
- The channels you use. Add one only with its own rules for subject and length.
- Where the reply log lives and who updates it after each send and reply.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI, drawing on one openly licensed package credited in its sources. Editorially reviewed. Tried on its invented example on 10 November 2026 in two runs: the instructions were revised after the first, and the second is the run recorded. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
