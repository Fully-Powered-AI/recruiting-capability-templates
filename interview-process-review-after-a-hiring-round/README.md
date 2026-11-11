# Interview process review after a hiring round

After a hiring round closes, the recruiting lead gets a review of the interview process: questions that gave no usable evidence, competencies nobody covered, inconsistent rubric use, and revisions to approve before the next search. It reviews the process only; no candidate is assessed.

*Capability template · Recruiting and hiring · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/interview-process-review-after-a-hiring-round/)*

## The outcome

The next search starts from what this round taught you instead of from the same interview plan. You see which questions gave interviewers nothing they could write down, which questions were asked twice, which parts of the agreed rubric were never put to anyone, and where interviewers used the rubric differently from one another.

Each finding comes with a proposed change, written as a draft you can accept, edit or drop: a reworded question, a question removed, a question added for an uncovered competency, a change to the feedback form. The recruiting lead decides which revisions go into the next plan. Nothing changes until then.

The review is about the process. It does not say who the strongest candidate was, does not revisit any outcome, and does not compare interviewers as people. It reports by question, by competency and by interview.

## Who starts the work, and when

The recruiting lead, or a recruiter they ask, starts it once a hiring round has closed and the feedback is in, ideally before the interview plan is reused for a comparable search. It suits any role you will hire for again, such as a team lead you recruit every year or a position you fill repeatedly.

The recruiting lead reads the draft, checks the notes the assistant judged unusable, and approves, edits or drops each proposed revision. The AI assistant sends nothing and changes no plan, form or record.

## What they supply

- The agreed rubric for the role: each competency, with what good evidence looks like.
- The interview plan the round used: which question was asked in which interview, and which competency it was meant to cover.
- The panel feedback with candidates and interviewers anonymised: for each question asked, the rating given and the note of what the candidate said or did.
- A short note of any process issues people raised during the round, such as a late start or a missing briefing.
- A few settings: the role, the date the round closed, the rating scale and who reads the review.

## What comes out

One review in a fixed order. It opens with where the files came from and a headline count. Then the questions that gave little usable evidence, the questions repeated across interviews, the coverage of every competency in the rubric, and how the rubric was used: ratings given without a usable note, and ratings for the same competency that sit far apart.

It goes on to the questions that were not asked, each process issue people raised checked against the feedback where the files allow, the list of notes judged unusable so you can check the judgement yourself, and the proposed revisions. Each revision names the finding behind it and waits for the recruiting lead's decision. If a header in a file does not match, the review stops and asks rather than guessing.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Recruiting and hiring](https://fullypowered.ai/functions/recruiting-and-hiring/), after any round that will be run again for a similar role.
- [People and HR](https://fullypowered.ai/functions/people-and-hr/), where the same interview process is reused for several hires and nobody has time to look back at it.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where a small group of partners and senior staff interview for the same few roles year after year.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where a loop of several interviews can end up asking one question twice and another never.
- [Hospitality](https://fullypowered.ai/industries/hospitality/), where repeated hiring for supervisor and manager roles makes a better interview plan pay back quickly.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when you hire in rounds and each round should make the next one better.

## What has to change for your company

Decide what counts as usable evidence for your roles; the template starts with a recorded example, action or figure the candidate gave. Set your rating scale, the number of times a question must be asked before it is judged, and how far apart two ratings must be to count as inconsistent. Agree who sees the review, since it names interviews and questions but never people. Agree who may approve a revision to the plan, and whether the hiring manager also signs off.

The template works from your anonymised feedback export. Remove names and contact details first, and leave out any column that records an outcome or a personal characteristic; the assistant will not read such columns.

## What has been checked

Fully Powered AI wrote this capability template. It was editorially reviewed on 10 November 2026. It was tried on 10 November 2026 on an invented example round in Claude, and that record is published with it. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past round your recruiting lead already knows well, with cases written in advance: a header that does not match, a question asked twice, a competency with no question, a rating with no note. The recruiting lead checks every count against the files, and reads the notes judged unusable, before anyone relies on the review. [Interview plan and scorecard](https://fullypowered.ai/capabilities/interview-plan-and-scorecard/) is the capability for the plan before a round, and [Hiring pipeline status report](https://fullypowered.ai/capabilities/hiring-pipeline-status-report/) covers the pipeline itself.

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
- [Hiring pipeline status report](../hiring-pipeline-status-report/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
