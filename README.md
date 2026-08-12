# Routine Checklist

An accessible TypeScript learning project and functional prototype exploring alternative approaches to routine reminders for neurodivergent adults.

> **Status:** Planning / initial development

## About the project

Routine Checklist is a solo TypeScript learning project and functional prototype designed primarily with neurodivergent adults in mind, particularly people who experience difficulties with task initiation, transitions, executive functioning and maintaining routines.

The project has two purposes:

1. **Technical learning** — to consolidate and apply my TypeScript learning through an independent application build
2. **Product exploration** — to create a functional MVP prototype that can be demonstrated and tested with users before deciding what should be developed further

I am building the initial prototype after completing structured TypeScript learning and before beginning a larger TypeScript project with regular support from a senior developer mentor.

Rather than build a purely instructional project, I wanted to apply what I have learned to a problem I care about and believe is worth exploring.

## The problem

Checklists, alarms, timers and reminder applications can help people establish and maintain routines.

However, for some neurodivergent adults these tools don't provide enough support for the parts that are actually difficult, or they work well initially but become less effective over time.

Knowing that something needs to be done isn't necessarily the same as being able to initiate it.

An alarm can be dismissed without the task being completed. A notification can arrive during hyperfocus, overwhelm or a difficult transition. A checklist can clearly show what needs doing while providing little support with starting it.

A reminder system can therefore work exactly as designed while still failing to support the action it was intended to help with.

The question behind this prototype is not simply:

> **How can an application remind someone to do something?**

It is:

> **How can an application better support someone between intending to do something and actually doing it?**

## Existing tools and what this prototype explores differently

There are already many useful applications for task management, routines, reminders, habit tracking and ADHD support. This project is not based on the assumption that these tools don't work.

Instead, it explores a more specific problem: **what happens when receiving or acknowledging a reminder doesn't lead to completing the intended action?**

Many existing approaches focus on helping users:

* Record what they need to do
* Organise and prioritise tasks
* Establish habits and routines
* Receive reminders at scheduled times
* Track completion and progress
* Use timers to structure periods of activity

Routine Checklist focuses particularly on the interaction **after a reminder appears**.

Rather than treating a notification as a single event that can be completed, dismissed or snoozed, the prototype explores reminder workflows that can continue supporting the user after they respond.

For example, a user might indicate that they are busy, that they are starting the task now, or that they have deliberately decided not to complete it today. The application can then respond differently to each situation.

The longer-term project also explores the idea that the same strategy may not work equally well for one person at all times. Future research may investigate user-selected support modes, changing capacity, reminder habituation and ways of helping users reflect on which strategies work well for them in different circumstances.

These ideas will be treated as design hypotheses. Existing products, relevant research and feedback from neurodivergent users will be reviewed before deciding what further functionality to develop.


## Intended users

The primary intended users are neurodivergent adults who experience difficulties with areas such as:

* Task initiation
* Executive functioning
* Moving between activities
* Maintaining routines
* Remembering recurring activities
* Returning to something after an interruption
* Responding to conventional alarms and notifications
* Reminder or productivity strategies becoming less effective over time

Neurodivergent people are not a homogeneous user group.

The application will not assume that one workflow, interface or reminder strategy works for everyone. An individual person's needs may also change according to their circumstances, environment, attention and capacity.

User choice is therefore central to the longer-term concept.

## The initial concept

Routine Checklist is designed around repeatable routines rather than a conventional general-purpose to-do list.

A routine might involve:

* Taking medication at different times throughout the day
* Completing a morning routine
* Winding down in the evening
* Cleaning and tidying
* Preparing for work
* Completing a recurring administrative routine
* Any other set of activities someone wants help remembering and completing

The initial prototype will support one daily routine containing timed or untimed checklist items.

## MVP prototype

The MVP is deliberately small.

Its purpose is to provide enough functionality to practise TypeScript application development and create something usable enough to demonstrate and test the core reminder-workflow concept with users.

### Routine functionality

* Create one daily routine
* Add routine items
* Edit routine items
* Remove routine items
* Give items an optional scheduled time
* Mark items as complete
* Show relevant item states
* Persist the routine and today's state locally
* Reset daily completion state appropriately

### Initial reminder workflows

Conventional alarms often provide variations of two actions: **dismiss** or **snooze**.

The prototype will experiment with three more explicit responses.

#### Busy right now

The user acknowledges that the reminder has arrived at an inconvenient time.

The task remains active and the application asks again after a short interval.

#### Doing it now

The user indicates that they intend to act on the reminder now.

Rather than treating this acknowledgement as equivalent to completion, the application checks back after a short interval and asks whether the task was completed.

If it wasn't, the task remains active and support can continue.

#### Leave it for today

The user deliberately chooses not to complete that occurrence.

Further reminders for it stop for the day and the item returns as normal for its next occurrence.

These workflows are **prototype hypotheses**.

Their inclusion does not represent a claim that they are the right approaches for neurodivergent users. Part of the purpose of the prototype is to make these ideas testable.

## Example use case — medication routine

Medication is one potential use of a routine:

```text
08:00 — Morning
☐ Medication A
☐ Medication B

12:00 — Midday
☐ Medication C

18:00 — Evening
☐ Medication A

22:00 — Bedtime
☐ Medication D
```

A reminder for the 18:00 item might therefore allow the user to indicate:

```text
Medication A is due

[ Busy right now ]
[ Doing it now ]
[ Done ]
[ Leave it for today ]
```

Medication management is not built into the domain of the initial application. This remains a general-purpose routine tool.

## Why TypeScript?

The project began primarily as a way to embed my TypeScript learning through an independent build.

It provides opportunities to practise concepts including:

* Interfaces
* Type aliases
* Union types
* Optional properties
* Typed collections
* Typed application state
* Function parameter and return types
* State transitions
* Time-based application logic
* Browser APIs
* Local persistence
* Error handling
* Automated testing

The reminder workflows also provide an opportunity to explore modelling behaviour as explicit states and transitions rather than accumulating loosely related boolean values.

## Development approach

This is an independent solo build.

My initial aim is to complete the MVP myself so that I practise translating TypeScript concepts from structured learning into application design, implementation, testing and debugging.

After completing the prototype, I plan to ask a senior developer mentor to review the project.

Significant technical feedback and subsequent changes can then be documented as a post-MVP iteration.

This provides two deliberately different learning stages:

**independent implementation → professional code review → technical iteration**

The project precedes a larger TypeScript project that I will build with regular senior developer mentoring.

## Accessibility and human-centred design

Accessibility is intended to form part of the architecture and design of the prototype rather than being added at the end.

The MVP will consider:

* Semantic HTML
* Keyboard accessibility
* Logical focus behaviour
* Visible focus states
* Appropriate labels and instructions
* Screen-reader accessible status changes
* Status information that doesn't depend on colour alone
* Predictable interaction
* Clear, non-judgemental language
* Reduced cognitive effort
* Graceful behaviour where browser notification permissions aren't available

The interface will aim to be simple to understand and use, minimising unnecessary friction, including amount of steps, decisions and cognitive load.

## Why neurodivergent reminder workflows?

This project is particularly informed by an interest in designing technology for people with ADHD, executive-function differences and other neurodivergent experiences where conventional alarms, notifications and task lists may not always provide effective support.

The aim is not to create a universal "ADHD solution" or assume that everyone with the same diagnosis needs the same support.

Instead, the longer-term idea is to investigate whether people benefit from being able to choose different forms of support depending on what they need at a particular moment.

The MVP begins that investigation with only three reminder workflows.

## User and audience context

The human and research context behind the project will be documented separately in:

**`docs/user-context.md`**

This document will contain four parts.

### Part 1 — User stories

Three fictional user stories will illustrate different experiences involving:

* Reminders that don't lead to action
* Task initiation and transitions
* Overwhelm and variable capacity
* Hyperfocus
* Strategies becoming less effective over time
* Different support needs in different circumstances

### Part 2 — Understanding the context

Accessible explanations will provide further context for concepts relevant to the user stories, potentially including:

* Neurodivergence
* Executive functioning
* Task initiation
* Task switching and transitions
* Working memory
* Prospective memory
* Attention regulation
* Hyperfocus
* Cognitive load
* Overwhelm
* Variable capacity
* Habituation and reminder fatigue
* ADHD, motivation, reward and novelty
* Demand avoidance / PDA, including appropriate discussion of limitations and debate around the concept

Established evidence, emerging explanations and lived-experience-informed ideas will be distinguished where possible.

### Part 3 — Research, evidence and existing strategies

This section will examine relevant research and strategies already used to support these difficulties.

The intention is to trace:

**user experience → context → evidence → existing strategy → limitation → design hypothesis**

Potential product ideas will therefore be treated as hypotheses to investigate rather than assumed solutions.

### Part 4 — User feedback and iteration

After the MVP prototype is complete, it will be demonstrated and tested with users.

This section will document:

* What was tested
* How feedback was gathered
* What users found useful
* What created friction
* Accessibility and usability issues
* Assumptions supported by feedback
* Assumptions challenged by feedback
* Suggested workflows or features
* Changes made as a result
* Ideas deliberately not implemented and why
* Questions requiring further research

Individual feedback will not be treated as representative of all neurodivergent users.

Instead, feedback will contribute to an iterative process alongside research, accessibility principles and further testing.

## Long-term vision

The longer-term vision is to investigate whether Routine Checklist can become a tool that works better for neurodivergent adults for whom conventional checklists, alarms, timers and reminder applications don't work well or work only temporarily.

Rather than simply increasing the number or intensity of reminders, future development could explore different **workflows and modes of support**.

A user might be able to identify what they need at a particular moment rather than having the application attempt to determine their internal state.

Possible areas for research include:

* Low-capacity mode
* Overwhelmed mode
* Low-demand mode
* Hyperfocus support
* Only One Thing Today
* Only Three Things Today
* Persistent preferences
* Temporary modes
* Different reminder intervals
* Different interaction styles

These are research ideas, not planned MVP features.

## Temporary and persistent modes

One future possibility is to distinguish between a user's usual preferences and temporary circumstances.

A person might normally prefer one reminder style but temporarily select something such as:

```text
I have very little capacity today

Use this mode for:

○ 2 hours
○ Rest of today
○ Until I turn it off
```

Temporary modes could automatically expire so that a user doesn't need to remember to restore their normal settings.

This requires substantially more research and user feedback before implementation.

## Personal reflection and insights

A longer-term version could explore whether the application can help users learn more about the strategies that work for them.

With appropriate privacy, consent and user control, useful interaction data might include:

* Strategies selected
* Number of reminders required
* Deferrals
* Completion
* Time between reminder and completion
* Changes between strategies

This could be combined with very lightweight self-report data such as how demanding or useful an approach felt.

Interaction data cannot objectively measure someone's capacity, cognitive effort or internal state.

For example, taking a long time to complete something after a reminder could have many explanations.

The purpose would therefore be **reflection rather than judgement**.

With sufficient evidence, the application might eventually surface observations such as:

> **When you've previously felt like this, this approach appeared to help on 8 out of 10 occasions. Would you like to use it today?**

The user would always remain free to choose something else.

Software can identify patterns in the information available to it. It cannot know the person's complete circumstances or internal experience.

**The user remains the authority on what they need.**

## Novelty, habituation and reminder fatigue

Another future research question concerns strategies becoming less effective as they become familiar.

A reminder that initially attracts attention may eventually become easier to filter out.

Future research could investigate whether carefully controlled variation in wording, presentation or interaction can provide enough novelty to restore salience without creating uncertainty, which could be counterproductive, or additional cognitive load.

This is deliberately a research question rather than an assumed feature.

Consistency can itself be an important accessibility requirement, so introducing novelty would require careful research and testing.

## Possible medication inventory integration

The idea for Routine Checklist originally emerged while I was considering the design of a medication inventory application. I initially thought about checklists and reminders as features within that application, but the underlying problem was broader: the same support could be useful for many different everyday routines.

That led me to separate **routine and reminder support** from **medication inventory management** as distinct areas of responsibility.

Medication is therefore a useful example of a routine within this prototype, but medication-specific functionality is intentionally outside its domain.

In the longer term, these capabilities could potentially form separate services within a larger application or microservice-based architecture:

```text
Routine and reminder service
        │
        ├── routines
        ├── reminders
        ├── workflows
        └── reflection

Medication inventory service
        │
        ├── medications
        ├── quantities
        ├── stock
        └── reorder thresholds

        Optional integration
```

Keeping these responsibilities separate could allow different users to use only the services relevant to them.

Someone might use Routine Checklist to support everyday routines without needing medication management. Another user might need medication inventory functionality without the broader routine support. Someone who needs both could use the services together as part of an integrated application.

A combined experience could eventually connect information across the two domains — for example, a scheduled medication routine could be supported by inventory information about remaining supply and reorder thresholds.

A microservice architecture is **not part of the current MVP**. The initial prototype will remain deliberately simple. This separation instead records a possible future architectural direction if the application grows sufficiently to justify independently developed and deployed services.


## Build principles

* Keep the MVP small and finishable
* Prefer clear TypeScript types and explicit application states
* Separate application logic from presentation where practical
* Build accessibility in from the beginning
* Keep the initial domain general rather than medication-specific
* Test important behaviour rather than implementation details
* Document technical decisions and trade-offs
* Record useful debugging and learning
* Treat assumptions about users as hypotheses
* Use research and user feedback before expanding neurodivergence-specific functionality
* Keep users in control of support choices
* Avoid allowing interesting future ideas to become accidental MVP requirements

## Build notes

Significant technical decisions and debugging will be documented during development.

A simple structure will be used where useful:

**Problem → investigation → cause → solution → learning**

This creates a record both of the project's technical development and of my TypeScript learning.

## Roadmap

### v0.1 — Functional MVP prototype

* [ ] Set up TypeScript project
* [ ] Define routine and reminder domain types
* [ ] Create a daily routine
* [ ] Add, edit and remove routine items
* [ ] Support timed and untimed items
* [ ] Mark items complete
* [ ] Persist data locally
* [ ] Implement upcoming and due states
* [ ] Implement Busy right now workflow
* [ ] Implement Doing it now workflow
* [ ] Implement Leave it for today workflow
* [ ] Build reminder interface
* [ ] Complete accessibility review
* [ ] Add automated tests
* [ ] Deploy prototype

### v0.2 — Review and user feedback

* [ ] Senior developer code review
* [ ] Review TypeScript modelling and architecture
* [ ] Address agreed technical improvements
* [ ] Document significant review findings
* [ ] Conduct prototype usability testing
* [ ] Gather feedback from intended users
* [ ] Record findings in [docs/user-context.md](docs/user-context.md)
* [ ] Compare findings with initial design hypotheses
* [ ] Identify priorities for further research or development

### Future development

Future development will be determined by evidence rather than a fixed feature list.

Potential areas include:

* Additional reminder workflows
* Offline/PWA functionality
* Multiple routines
* Configurable support preferences
* Temporary support modes
* Low-capacity and overwhelm support
* Hyperfocus support
* Personal reflection
* Pattern identification
* Optional strategy recommendations
* Controlled novelty
* Further accessibility improvements
* Optional medication inventory integration

## Project status

**Planning / initial development**

This README intentionally documents both the small initial prototype and the larger problem it is intended to explore.

Only functionality listed under the MVP roadmap is currently planned for the initial build.

Future concepts are included to document the thinking behind the architecture and provide directions for research. They may change substantially, or be rejected entirely, following research, technical learning and feedback from users.
