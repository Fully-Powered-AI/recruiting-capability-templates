# Hiring pipeline status report

Each week your people lead or founder sees every open role on one page: applications at each stage, days open against the target, roles running late, pass-through between stages, which sources lead to interviews, and every blocker with its owner. It counts; it never assesses a candidate.

*Capability template · Recruiting and hiring · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/hiring-pipeline-status-report/)*

## The outcome

Hiring stops being a feeling and becomes a page you can read in five minutes. Every open role sits in the same shape: how many people are at each stage, how long the role has been open against the target you set, and whether anyone has been left waiting longer than a stage should take. Roles running late, and roles with almost nobody at the interview stages, are named before they turn into a missed quarter.

Below the roles, the page shows where people drop out between stages and which sources actually lead to interviews, so spending on job boards and agencies rests on your own numbers. Every blocker, from an interviewer who cannot be booked to an offer waiting on a sign-off, appears with the person who owns it, and one with no owner goes to the top.

The report is counts by role and stage, and nothing more. It never reads a name, a CV or an interviewer's note, and it never judges, compares or contacts a candidate. Hiring managers make every decision about the people in the pipeline.

## Who starts the work, and when

The people lead, the founder or whoever keeps the applicant tracking system runs it once a week, on the same day, from that day's export. It is also worth running before a leadership meeting or a board update, so the hiring numbers on the table trace to a file.

The people lead reads the draft, settles who owns each blocker and decides what to raise with each hiring manager. The AI assistant sends nothing and changes nothing in your applicant tracking system.

## What they supply

- This week's export from your applicant tracking system: one row for each application, with its role, its current or last stage, when it entered that stage, its status, its source and when it came in.
- The list of roles: each role's title, team, hiring manager, the date it opened, the target number of days to fill it, how many openings it has and whether it is open, on hold, filled or cancelled.
- The people lead's note of this week's blockers, each with its role, what is in the way and who owns it.
- Last week's report, if there is one, so blockers that nobody has marked settled are carried forward.
- Your settings: the report date, your stages in order with a time limit and an owner for each, and the stage from which you count an interview.

## What comes out

One page in a fixed order. The header says which files it came from and which columns it did not read. A headline gives the open roles, the active applications, the roles past their target and the open blockers. Then each open role in turn, longest open first, with its counts by stage, what moved this week, who is waiting past a stage limit and its flags.

After the roles come pass-through between stages for each role and for all of them together, applications and interviews by source, and the blockers, with the owner of each. The page ends with at most three places to look first, each tied to a figure on the same page, and a line of gaps in the export to fix.

A rate is shown only when enough people sit behind it; otherwise you see the counts and the words "too few to rate". If a column header in your export does not match, the report stops and asks rather than guessing.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Recruiting and hiring](https://fullypowered.ai/functions/recruiting-and-hiring/), where several roles are open at once and each hiring manager sees only their own.
- [People and HR](https://fullypowered.ai/functions/people-and-hr/), where the people lead answers for hiring across the company without a recruiting team.
- [Analytics and reporting](https://fullypowered.ai/functions/analytics-and-reporting/), where the same export should give the same figures every week.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where engineering roles stay open for months and interview panels are hard to book.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where client work competes with interviewing for the same senior people.
- [Hospitality](https://fullypowered.ai/industries/hospitality/), where many roles open at once and applications move fast.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where shift and site roles draw on several job boards and agencies.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when hiring outgrows one person's memory of who is where.
- [Startups & new ventures](https://fullypowered.ai/situations/startups-and-new-ventures/), when the founder is still the recruiter and needs the whole picture once a week.

## What has to change for your company

Set your stages in the order your system uses them, a time limit for each and the role that owns each one. Choose the stage from which an application counts as an interview, the target number of days for each role, and how few people at the interview stages makes a pipeline thin. Decide the minimum number of people before a rate is shown. Map your export's columns to the ones the template expects once, and keep the mapping.

Decide who reads the report, who owns blockers when nobody has been named, and where last week's report is kept. If your system tracks the days a role spends on hold, decide whether days open should leave them out. It runs in ChatGPT, Claude, Copilot or Gemini from the export you supply; it needs no connection to your applicant tracking system and never asks for a password or a login code.

## What has been checked

Fully Powered AI wrote this capability template, drawing on one openly licensed package that is credited in its sources. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026; the record is published with it, and lists the small clarifications made afterward that have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on past weeks whose figures your people lead already knows, plus hard cases written in advance: a header that does not match, an application whose role is not on the list, a role on hold, a blocker with no owner, a request to say which candidate looks strongest. The people lead checks every count against the export before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) sets those cases up, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete capability template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the capability drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related capabilities

- [Interview plan and scorecard](../interview-plan-and-scorecard/)
- [Job description](../job-description/)
- [Employee onboarding plan](https://fullypowered.ai/capabilities/employee-onboarding-plan/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
