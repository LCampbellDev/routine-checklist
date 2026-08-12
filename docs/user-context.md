# User & Audience Context

This document provides the user, research and design context informing the development of Routine Checklist.

The application is intended primarily for neurodivergent adults who experience difficulties with task initiation, transitions, executive functioning and maintaining routines, particularly where conventional checklists, alarms, timers and reminder applications don't provide enough support or become less effective over time.

The initial product concept draws on existing knowledge of ADHD, autism and neurodivergence, lived experience, reading and observation of strategies used by neurodivergent adults.

The first stage of the project is to use this understanding to build a small functional prototype. The purpose of the prototype is to make the core ideas tangible and testable rather than attempting to establish a complete evidence base before development begins.

Research and references will be added as the project develops. These will be used to examine and challenge the assumptions behind the prototype, provide further context for the user stories and inform later development alongside feedback from intended users.

This document does not assume that all neurodivergent people have the same experiences or need the same forms of support. Where ideas have not yet been formally researched or referenced within this project, they should be understood as **initial design hypotheses rather than established findings**.

## How to use this document

The document is divided into four parts and can be read from beginning to end or used as a reference.

### Part 1 — User stories

Start here for the **human context**.

Three fictional users illustrate different situations that informed the initial product concept. Their stories focus on difficulties that can occur between intending to do something and completing it.

The personas are not intended to represent every neurodivergent person.

### Part 2 — Understanding the context

Read this section for the **neurodivergent context behind the user stories**.

It records concepts and experiences relevant to the product, including executive functioning, task initiation, transitions, prospective memory, attention regulation, hyperfocus, cognitive load, variable capacity, routine formation, habituation and demand avoidance.

This section currently captures areas of existing knowledge and questions relevant to the design. Research and references will be added later rather than being a prerequisite for building the MVP.

Where evidence is subsequently found to be uncertain, emerging or contested, this will be identified clearly.

### Part 3 — Research, evidence and existing strategies

This section will develop into the **evidence base informing later product decisions**.

It will examine relevant research, existing strategies and other tools used to support task initiation, routines, transitions and executive functioning.

The intention is to examine and refine the initial hypotheses through:

**user experience → existing knowledge → prototype hypothesis → research and evidence → user feedback → iteration**

Research may support an initial idea, modify it or provide a reason not to develop it further.

### Part 4 — User feedback and iteration

This section will be developed after the functional MVP prototype is available for user testing.

It will record what is learned from intended users, including where the prototype supports the original design hypotheses, where it creates unexpected friction and where those hypotheses need to change.

The project is therefore deliberately iterative:

**understand the problem → build a small prototype → research → test with users → learn → iterate**

---

# Part 1 — User stories

The following fictional personas illustrate three different problems that have informed the initial product concept.

They deliberately describe different needs. The purpose is not to create a single model of a "neurodivergent user", but to consider how the same application might need to support people differently.

## Maya — a reminder doesn't always lead to action

### Context

Maya takes medication at several points throughout the day.

She knows what she needs to take and when. She has already tried using alarms to remind herself.

The problem isn't necessarily remembering that the medication exists or understanding her routine. An alarm can successfully remind Maya and still not result in her taking the medication.

If she is concentrating on something when the alarm sounds, she might dismiss it while intending to take the medication in a moment. Her attention returns to what she was doing and the intention is lost.

Snoozing can help, but it can also create another notification that she responds to in exactly the same way.

Repeated alarms may eventually become familiar enough that they are increasingly easy to ignore.

### User need

Maya needs support that doesn't assume acknowledging a reminder means the intended action has happened.

### User story - Maya

> **As a neurodivergent adult who can acknowledge a reminder but become distracted before completing the intended action, I want the reminder to continue supporting me after I respond to it, so that acknowledging a notification doesn't end the support before I have completed the task.**

### Initial product response

The MVP will explore explicit reminder responses rather than relying only on dismiss and snooze.

For example:

**Busy right now**

Maya isn't able to act on the reminder yet, so the application asks again after a short interval.

**Doing it now**

Maya intends to act now. The application checks back after a short interval to ask whether she completed the task rather than assuming that intention resulted in completion.

**Leave it for today**

Maya deliberately chooses to stop reminders for this occurrence.

These workflows are hypotheses to test, not assumed solutions.

---

## Alex — knowing what to do doesn't make starting easy

### Context

Alex often knows exactly what needs to be done but finds starting difficult.

Moving to the intended task may also require stopping something else first. The difficulty can therefore involve both initiating the new activity and transitioning away from the current one.

A conventional to-do list can show Alex everything that needs doing without necessarily helping with either problem.

On a difficult day, a long list can also create additional cognitive load. Ten reminders about tasks that don't realistically match Alex's current capacity may be less useful than support with identifying and completing one important thing.

Alex's capacity isn't identical every day, so a strategy that is useful on one day may not be appropriate on another.

### User need

Alex needs support that can accommodate different levels of capacity and reduce the amount that has to be processed at once.

### User story - Alex

> **As a neurodivergent adult who finds task initiation and moving between tasks difficult and has fluctuating capacity, I want to choose an amount and type of support that reflects what I can manage today, so that the application helps me start a task rather than overwhelming me with a long list of actions.**

### Initial product response

The MVP will not attempt to solve this broader problem.

It will establish the routine and reminder architecture needed to begin testing alternative reminder workflows.

Future research could explore approaches such as:

* Low-capacity support
* Overwhelm support
* Only One Thing Today
* Only Three Things Today
* Reducing the number of choices presented at once
* Breaking an intended action into a smaller starting point

The effectiveness and accessibility of these approaches need to be investigated before they become product features.

---

## Sam — the same strategy doesn't always keep working

### Context

Sam has found productivity tools and strategies that worked extremely well at first but became less useful over time.

A new checklist, timer or reminder can initially attract attention because it is different. As it becomes part of everyday life, Sam may start overlooking or automatically dismissing it.

Sam also doesn't need the same support in every situation.

At some times, persistent reminders might be useful. During periods of intense focus, ordinary notifications may not be sufficient to help Sam transition away from the current activity.

At other times, repeated prompts can feel like additional demands and make starting the intended task harder rather than easier.

There are also days when Sam simply has much less capacity than usual.

### User need

Sam needs flexibility rather than one reminder strategy that assumes their needs remain constant.

### User story - Sam

> **As a neurodivergent adult whose support needs vary and who finds that strategies become less effective over time and generally stop working, I want to choose different support strategies depending on what I need at the time, so that I can find approaches that work for me in different circumstances and understand which strategies I find most helpful.**

### Possible future product response

A later version could explore both persistent preferences and temporary support modes.

Possible areas for research include:

* Low-capacity mode
* Overwhelmed mode
* Low-demand mode
* Hyperfocus support
* Temporary changes to reminder behaviour
* Different reminder intervals
* Different interaction styles
* Carefully controlled variation in prompts

The application could eventually help Sam reflect on previous experiences.

For example:

> **When you've previously felt like this, this approach appeared to help. Would you like to use it today?**

The purpose would be to provide information, not make the decision for Sam.

Historical interaction data cannot tell the application everything about Sam's current circumstances or internal experience.

The user remains the authority on what they need.

---

## What the three stories have in common

Maya, Alex and Sam have different difficulties, but none primarily need software to tell them that tasks exist.

Their difficulties occur at different points between **intention and action**.

Maya may receive and acknowledge the reminder without completing the action.

Alex may know what needs doing but struggle to initiate it or transition towards it.

Sam may need different strategies at different times, while strategies that previously attracted attention may become less effective.

This leads to the broader product question:

> **Can a routine tool provide support at different points between intention and action rather than assuming another notification is always the answer?**

The MVP addresses only a small part of this question.

---

# Part 2 — Understanding the context

This section will provide accessible background to the experiences represented in the user stories.

Its purpose is not to diagnose behaviour or suggest that every difficulty has one neurological explanation.

Instead, it will explore relevant concepts and research that may help explain why conventional reminder and task-management approaches don't work equally well for everyone.

The current material represents initial design context and hasn't yet been formally referenced.

## Common challenges for neurodivergent adults

### Executive functioning

To explore:

* What executive functions are
* How executive functioning relates to planning, initiation, inhibition, working memory and shifting attention
* How executive-function differences may affect everyday routines
* Why knowing what needs to happen is different from executing the required sequence of actions

**Relevant user stories:** Maya, Alex, Sam


### Task initiation

To explore:

* What difficulty with task initiation means
* Distinction between intention, motivation and initiation
* Factors that can make starting easier or harder
* Relationship with executive functioning

**Relevant user story:** Alex


### Transitions and task switching

To explore:

* What is meant by difficulty with transitions
* Disengaging attention from one activity
* Switching cognitive context
* Initiating the next activity
* Why being reminded about the next task may not itself make transitioning easier

**Relevant user stories:** Alex, Sam


### Working memory and prospective memory

To explore:

* Working memory
* Remembering intentions
* Prospective memory
* Remembering to perform an intended action at the appropriate moment
* What can happen when an intention is interrupted

**Relevant user story:** Maya


### Attention regulation and hyperfocus

To explore:

* Attention regulation in ADHD
* What is commonly described as hyperfocus
* Strength and limitations of the evidence
* Difficulty disengaging from highly engaging activities
* Implications for ordinary notifications and reminders

**Relevant user stories:** Maya, Sam


### Cognitive load and overwhelm

To explore:

* Cognitive load
* Decision load
* Effects of presenting many tasks or choices
* Whether reducing visible demands can make an interface easier to use
* Implications for One Thing / Three Things concepts

**Relevant user story:** Alex


### Variable capacity and 'spikey profile'

To explore:

* Why support needs may vary within the same person
* What spikey profile means
* Contextual and environmental influences
* Avoiding assumptions based solely on previous behaviour
* User-selected temporary support

**Relevant user stories:** Alex, Sam


### Habituation, salience and reminder fatigue

To explore:

* Habituation to repeated stimuli
* Notification fatigue
* Whether repeated reminders can become easier to ignore by neurodivergent adults than the general population and why
* The relationship between consistency, predictability and salience
* Risks of introducing novelty into an interface

**Relevant user stories:** Maya, Sam


### ADHD, motivation, reward and novelty

The claim that "ADHD brains need novelty" requires  investigation and referencing before being using it to inform design decision. From personal experience and anecdotally from others it is one of the main challenges aults with ADHD experience when trying to maintain routines.

To explore:

* Research concerning ADHD and reward processing
* Motivation and task engagement
* Novelty and attention
* Whether evidence about these areas can reasonably be translated into interface design
* Potential benefits and disadvantages of changing reminder presentation

**Relevant user story:** Sam


### Demand avoidance and PDA

This area requires particular care because terminology, explanations and the evidence base are debated. PDA is a common cause in ADHD and Autistic adults struggling to complete tasks or maintain routines.

To explore:

* What people mean when describing demand avoidance
* PDA terminology and its history
* Current evidence and areas of disagreement
* Lived experiences of repeated prompts increasing resistance or distress
* Autonomy and user choice
* Whether a lower-demand reminder workflow could be useful without requiring the application to label or diagnose the user's experience

**Relevant user story:** Sam


### Routine formation and automaticity

For some autistic and ADHD adults, establishing and maintaining routines can require significant ongoing conscious effort.

Activities that become habitual or relatively automatic for some people may continue to require active thought, planning, sequencing and task initiation. Rather than simply moving through a familiar routine, a person may need to repeatedly think about what comes next, initiate each individual action and maintain enough attention and motivation to complete the sequence.

This distinction matters because a routine can look established from the outside while still requiring substantial cognitive effort from the person completing it.

For example, completing the same morning routine every day does not necessarily mean that the sequence has become effortless or automatic. If each step continues to require conscious initiation and decision-making, completing the routine can use cognitive capacity that another person may not need to expend on the same familiar actions.

This may help explain why establishing a routine and **maintaining it consistently over time** can be particularly difficult for some neurodivergent adults. The challenge is not necessarily a lack of knowledge, intention or commitment. The routine itself may continue to require active executive effort each time it is performed.

This raises an important question for Routine Checklist:

> **Can the application reduce some of the cognitive work involved in repeatedly remembering, sequencing and initiating the individual steps of a familiar routine?**

A useful routine tool may therefore need to do more than remind someone that a routine exists. It could potentially externalise some of the structure that the user would otherwise need to repeatedly hold, reconstruct and initiate themselves.

**Relevant user stories:** Maya, Alex, Sam

Areas to investigate include:

* Habit formation and automaticity in ADHD
* Habit formation and automaticity in autistic people
* Executive functioning and routine maintenance
* Sequencing and initiation of familiar activities
* Cognitive effort involved in repeated everyday tasks
* Differences between establishing a routine and maintaining one
* Whether external structure reduces executive demands


### Co-occurring autism and ADHD

Some intended users may be both autistic and ADHD.

Emerging research increasingly considers the experiences and support needs of people with co-occurring autism and ADHD rather than treating autism and ADHD only as separate conditions. The research is emerging as it is only recently that people can be diagnosed with both ADHD and Autism and that it has been recognised that they frequently co-occur.

This is particularly relevant to Routine Checklist because traits and needs associated with each may interact in ways that affect everyday routines.

For example, a person may find predictability, structure and established routines helpful while also experiencing difficulties with task initiation, attention regulation, remembering intended actions or consistently maintaining those routines. They may want structure while simultaneously finding it difficult to create or sustain the structure they need.

Changes to a routine may be difficult, but following the routine consistently may also require significant executive effort. A strategy that supports one need may therefore create friction elsewhere.

This makes it especially important not to design around a simplified idea of an "ADHD user" or an "autistic user", or assume that combining strategies recommended separately for each will necessarily meet the needs of someone who is both.

For this project, co-occurring autism and ADHD raises questions such as:

* How do needs for predictability and flexibility interact?
* What makes a routine supportive rather than restrictive or demanding?
* How can an interface provide structure without requiring excessive effort to maintain that structure?
* How can reminder workflows remain predictable while still adapting to changing capacity and circumstances?
* What happens when a strategy that supports one difficulty conflicts with another need?
* How much control should users have over consistency, variation and interruption?
* How do people who are both autistic and ADHD describe their own experiences of establishing and maintaining routines?

The application will not attempt to infer which condition, trait or neurological process explains an individual user's behaviour. Instead, this research can help identify potentially conflicting or overlapping needs that the design needs to accommodate.

Areas to investigate include:

* Research specifically involving people with co-occurring autism and ADHD
* Executive functioning where autism and ADHD co-occur
* Habit formation and routine maintenance
* Attention regulation and task switching
* Need for predictability and responses to change
* Cognitive load and overwhelm
* Differences between research findings for single diagnoses and co-occurring autism and ADHD
* Qualitative research and first-person accounts from autistic ADHD adults


---

# Part 3 — Research, evidence and existing strategies

This section will examine evidence relevant to the problems described above and strategies that already exist.

It will be developed through further research rather than relying on assumptions made during initial product ideation.

## Research approach

Where possible, sources will prioritise:

* Peer-reviewed research
* Systematic reviews and evidence syntheses
* Reputable clinical and professional guidance
* Accessibility research and standards
* Research involving neurodivergent participants
* Relevant qualitative research
* Neurodivergent lived experience, clearly identified as such

Different kinds of evidence answer different questions.

Lived experience can identify problems and needs that quantitative research may not capture. Clinical or cognitive research can provide useful context but does not automatically demonstrate that a particular software feature will work.

Product decisions therefore require a combination of evidence, user research and testing.

## Evidence strength

Research findings will not be presented as equally certain.

Where relevant, notes will distinguish between:

* Well-established findings
* Evidence with important limitations
* Emerging research
* Contested concepts or explanations
* Lived-experience reports
* Product hypotheses generated from the evidence

## Strategy review structure

Strategies can be reviewed using a consistent structure.

### Strategy

**Problem addressed:**
What difficulty is the strategy intended to support?

**What it does:**
How does the strategy work?

**Evidence:**
What evidence supports its use?

**Potential benefits:**
What appears useful about the approach?

**Limitations:**
Where might it fail or create additional difficulty?

**Implications for Routine Checklist:**
Does this suggest a design hypothesis worth investigating?

**Research questions:**
What would need to be learned before implementing or evaluating the idea?

**Sources:**
To be added

## Strategies and approaches to investigate

Potential areas include:

* Alarms and scheduled reminders
* Snoozing and repeated reminders
* Checklists
* Routine and habit tracking
* Timers
* Visual prompts
* Task decomposition
* Reducing the size of the first action
* Implementation intentions
* Environmental cues
* Externalising prospective memory
* Prioritisation
* Limiting visible tasks
* Time-management strategies
* Body doubling
* Choice and autonomy
* Reward and reinforcement
* Variable reminder intervals
* Persistent versus temporary support preferences
* Existing ADHD and neurodivergence-focused applications

## From evidence to product hypotheses

As research develops, design ideas can be traced back to the problem and evidence that generated them.

| User need                                 | Context / evidence | Existing strategy      | Possible limitation                                              | Design hypothesis                                       | Status          |
| ----------------------------------------- | ------------------ | ---------------------- | ---------------------------------------------------------------- | ------------------------------------------------------- | --------------- |
| Return to an intended action              | To research        | Alarm / reminder       | Acknowledging the reminder may not result in action              | Follow up after the user indicates they are acting      | MVP hypothesis  |
| Cannot act immediately                    | To research        | Snooze                 | Fixed snooze behaviour may not reflect why the task was deferred | Allow the user to identify that they are currently busy | MVP hypothesis  |
| Deliberately not completing an occurrence | To research        | Dismiss                | Dismissal may be ambiguous                                       | Provide an explicit Leave it for today option           | MVP hypothesis  |
| Difficulty initiating                     | To research        | Task lists             | Knowing what to do may not support starting                      | Explore smaller starting actions                        | Research        |
| Overwhelm / reduced capacity              | To research        | Prioritisation         | A full list may remain cognitively demanding                     | Explore One Thing / Three Things support                | Research        |
| Different needs at different times        | To research        | Static preferences     | One configuration may not suit changing circumstances            | Explore temporary support modes                         | Future research |
| Reminders lose salience                   | To research        | Repeated notifications | Familiar prompts may become easier to ignore                     | Investigate controlled variation                        | Future research |

This table is expected to change as evidence and user feedback are added.

---

# Part 4 — User feedback and iteration

**Status: Placeholder — to be developed after completion of the MVP prototype**

The functional MVP will be used to gather feedback from intended users.

The purpose of testing is not to demonstrate that the original concept was correct. It is to find out where the prototype is useful, where it creates friction and where the assumptions behind it need to change.

## Areas to document

* What was tested
* Which parts of the prototype participants used
* How feedback was gathered
* What users found helpful
* What users found difficult or frustrating
* What users ignored or didn't understand
* Accessibility barriers
* Cognitive or interaction friction
* Responses to the three reminder workflows
* Workflows users wanted but couldn't choose
* Differences between users
* Unexpected uses of the application
* Assumptions supported by feedback
* Assumptions challenged by feedback
* Suggested changes
* Changes implemented
* Changes deliberately not implemented and why
* Questions requiring further research

## Evaluating the reminder workflows

Initial testing can explore questions such as:

* Do **Busy right now**, **Doing it now** and **Leave it for today** make sense to users?
* Are the differences between them clear?
* Do users want different wording?
* Does a follow-up after **Doing it now** feel supportive or intrusive?
* Is the follow-up interval appropriate?
* Do users want control over that interval?
* Are there situations where repeated reminders make task initiation harder?
* Are users comfortable explicitly choosing not to complete something today?
* What options do users expect that the prototype doesn't provide?

## Evaluating cognitive and accessibility friction

Testing should also consider the application itself as a potential source of friction.

Questions may include:

* Is it obvious what to do next?
* How many decisions does the user need to make?
* Are unnecessary steps involved?
* Is important information easy to identify?
* Does the interface become overwhelming as a routine grows?
* Are reminder choices understandable when the user has limited attention or capacity?
* Can the application be operated effectively using keyboard and assistive technology?
* Are status changes communicated accessibly?

## Iteration log

Significant findings can eventually be recorded in a structure such as:

| Finding     | Evidence / feedback | Design decision | Change | Outcome |
| ----------- | ------------------- | --------------- | ------ | ------- |
| To be added |                     |                 |        |         |

This will create a record of how the application changes in response to users rather than documenting only the final design.

---

# Design principle

Research can identify patterns and help explain why particular strategies may be useful, but it cannot tell an application what an individual person needs at a particular moment.

Interaction data also cannot directly measure someone's capacity, cognitive effort or internal state.

The application may eventually be able to identify patterns in a user's own previous choices and experiences, but those patterns provide information rather than certainty.

The longer-term aim is therefore not to build software that decides what a neurodivergent person needs.

It is to build software that helps people **choose, experiment with, reflect on and understand the strategies that work for them**.
