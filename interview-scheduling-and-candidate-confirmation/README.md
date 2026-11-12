# Interview scheduling and candidate confirmation

For candidates your team has already chosen to interview, the recruiting coordinator gets one scheduling sheet that lines up each candidate's offered times, in their own time zone, with the interviewers' free time, plus a ready confirmation or availability request for each. A person sends every message and invitation.

*Workflow template · Recruiting and hiring · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/interview-scheduling-and-candidate-confirmation/)*

## The outcome

Scheduling stops being days of back-and-forth email. Every candidate's offered times sit beside the interviewers' calendars in one time zone, with each candidate's own time shown next to it, so a slot that works at 10:00 in New York is plainly also 15:00 in London. Each candidate gets one proposed time, no interviewer is booked twice, and the gaps between interviews are kept.

Candidates hear back quickly, in your company's own words: a confirmation with the date, the time in their own zone, who they will meet and how to change it, or a short request with open times when nothing they offered fits.

It schedules and nothing more. It takes candidates in a fixed order that turns only on how many times each has offered, never on anything about the person, and it declines any request to favour one. It keeps questions about pay, family, health, immigration and other protected subjects out of every message, and it never repeats a reason a candidate gave for their times. A person checks every time, holds the slots, creates the invitations and sends each message.

## Who starts the work, and when

The recruiting coordinator starts it, or the hiring manager who does their own scheduling, once the people deciding have chosen who goes to a stage. Run it again whenever replies arrive, a calendar changes or a proposed time falls through. The coordinator reads the sheet, holds each time on the calendars, creates the invitations and then sends the drafts.

## What they supply

- The stage settings: role title, stage, length, format, where it happens, the interviewers, the planning time zone, the dates to schedule in, and your wording for greetings, sign-off and anything every candidate should hear.
- The candidate list from your applicant tracking system: reference, first name, email, time zone and whether their times are in.
- The times each candidate offered, in their own time zone, or their replies pasted as written.
- The interviewers' free time, exported from their calendars.
- Any notes from the hiring manager.

## What comes out

One scheduling sheet in a fixed order: the time when every required interviewer is free, each candidate's windows in both time zones, the possible start times, one proposed time per candidate with an alternative where there is one, and each interviewer's load. Loose phrases in replies, such as "Thursday morning", are shown with how they were read, so the coordinator can check them.

Then the drafts: a confirmation for each proposed time and an availability request for everyone else, offering only times nobody else has been given. Review notes list anything removed or declined, columns in the export that were left unread, the defaults used, and the open questions. If an export's columns are not the ones expected, it stops and asks rather than guessing.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Recruiting and hiring](https://fullypowered.ai/functions/recruiting-and-hiring/), where a coordinator juggles several candidates and several interviewers' calendars for every stage.
- [Executive and office support](https://fullypowered.ai/functions/executive-and-office-support/), where an office manager or executive assistant schedules interviews alongside everything else.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where candidates and interviewers sit in different time zones and a mistaken hour costs a candidate.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where interviewers are billing client work and their free time is scarce.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/), where senior staff interview between site visits and project deadlines.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when several roles are open at once and scheduling takes over someone's week.
- [Startups & new ventures](https://fullypowered.ai/situations/startups-and-new-ventures/), where the founder or hiring manager does their own scheduling.

## What has to change for your company

Write your wording once: the greeting, the sign-off, what candidates should prepare, how they change a time and any line every candidate hears, such as an offer of adjustments. Set the gap between interviews, how often a start time can fall, the earliest and latest hours you will offer a candidate, and how much notice you give.

Match the column names to what your calendar and applicant tracking system export, and keep scores, CVs and interview notes out of what the assistant reads. Add your people lead's own list of subjects never raised to the one the template always applies. Decide who may move a proposed time by hand and whether optional interviewers are invited whenever they are free. It runs in ChatGPT, Claude, Copilot or Gemini from the exports you supply, and needs no connection to your calendar, email or applicant tracking system.

## What has been checked

Fully Powered AI wrote this workflow template, drawing on one openly licensed method that is credited in its sources. It was editorially reviewed on 10 November 2026. It was tried on its invented example on 10 November 2026 in two runs; the template was revised after the first, and the record of the second, made on the revised version, is published with it. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a stage you have already scheduled, where the coordinator knows which times worked, plus hard cases written in advance: candidates in three time zones, two candidates wanting the same hour, a reply that gives a personal reason for its times, an export with a score column, a note asking to favour one candidate. The coordinator checks every time against the calendars before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) sets those cases up, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete workflow template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the workflow template drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related workflow templates

- [Interview plan and scorecard](../interview-plan-and-scorecard/)
- [Job posting and sourcing plan](../job-posting-and-sourcing-plan/)
- [Employee onboarding plan](https://fullypowered.ai/workflows/employee-onboarding-plan/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
