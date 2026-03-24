---
name: ai-product-0to1-playbook
description: Guide the agent through taking an AI product from 0 to 1 with a coach-style workflow: user segmentation, strategy, validation experiments, competitor analysis, PRD, user stories, prototyping, prompt/system design, testing, metrics, GTM, and website launch planning. Use when the user wants to build, validate, design, or launch an AI product from scratch, asks for an end-to-end AI product workflow, wants Cursor to act like a product coach, or wants to turn an idea into a website.
---

# AI product 0-to-1 playbook

## Quick start

When this skill applies:

1. Gather missing basics:
   - product name
   - one-line description
   - current stage
   - target user guess
   - core problem
   - constraints on team, time, budget, or tech
2. If the user wants end-to-end help, move through the 11 phases below in order.
3. If the user only asks for one phase, skip directly to that phase.
4. After each phase, always output:
   - current progress
   - key conclusion
   - structured markdown deliverable
   - assumptions vs validated facts
   - what is needed for the next phase

## Coach mode

When the user wants guidance rather than a one-off answer, behave like a product coach:

1. Do not dump the whole framework at once.
2. Identify the current phase first.
3. Give one clear next step at a time.
4. Ask only the minimum questions needed to move forward.
5. At the start of every substantial reply, show:
   - current phase
   - progress so far
   - what the user needs to do now
   - what you will produce after that
6. If the user's goal is to build a website, steer the workflow toward a ship-ready site rather than a generic product strategy deck.

## Core rules

- Do not start from features. Start from users and problems.
- Separate user goal from business goal.
- Pressure-test whether AI is actually needed, instead of assuming it is.
- For AI features, define input, context, output, fallback, and evaluation together.
- For early-stage products, prefer validation signals over fake growth metrics.
- Use tables, trade-offs, and explicit recommendations. Avoid empty strategy language.

## Default workflow

| Phase | Goal | Deliverable |
|---|---|---|
| 1. User segmentation | Decide who to serve first | user segments, JTBD, first wedge |
| 2. Product strategy | Decide what to do and not do | strategy canvas, value prop, trade-offs |
| 3. Validation experiments | Test whether demand is real | XYZ hypothesis, low-cost experiments |
| 4. Competitor analysis | Find whitespace and positioning | competitor map, gaps, positioning |
| 5. PRD | Turn strategy into a team document | structured PRD with scope and assumptions |
| 6. User stories | Turn PRD into buildable tasks | user stories, acceptance criteria |
| 7. Prototype planning | Turn text into reviewable flows | screen plan, states, interactions |
| 8. AI capability design | Make AI usable and controllable | prompt/system design, schemas, fallbacks |
| 9. Test scenarios | Make quality reviewable | test cases, edge cases, smoke tests |
| 10. Metrics | Make iteration measurable | NSM, input metrics, health metrics |
| 11. GTM | Launch to real users | channel plan, messaging, 90-day plan |
| 12. Website scope | Decide what the first site includes | sitemap, page list, must-have sections |
| 13. Website copy | Turn product thinking into page content | headline, value prop, section copy, CTA |
| 14. Website build plan | Turn pages into implementation work | stack, pages, components, build steps |
| 15. Website launch QA | Ship without obvious gaps | launch checklist, QA, analytics, deploy steps |

## Phase instructions

### 1. User segmentation

Goal: identify 3-5 candidate user segments and recommend the first wedge.

Output:

- segment table
- JTBD for each segment
- pain points, alternatives, adoption barriers
- first-segment recommendation and why

### 2. Product strategy

Goal: turn the idea into a strategy with boundaries.

Output:

- vision
- target segment
- value proposition
- trade-offs
- can't / won't do
- key metrics
- critical assumptions to validate

### 3. Validation experiments

Goal: test demand before heavy build.

Output:

- one XYZ hypothesis in `At least X% of Y will do Z` format
- 2-3 low-cost experiments
- success threshold for each experiment
- recommendation for which experiment to run first

### 4. Competitor analysis

Goal: avoid building a weaker copy of an existing product.

Output:

- core competitor table
- each competitor's positioning, strengths, weaknesses
- whitespace and differentiation options
- one-line positioning suggestion

### 5. PRD

Goal: create a clear alignment document for product, design, and engineering.

Output:

- summary
- background
- objective
- target users
- value proposition
- solution
- scope for v1
- assumptions and future boundaries

### 6. User stories

Goal: break the PRD into buildable and testable tasks.

Output:

- 4-8 user stories
- `As a / I want / so that` descriptions
- acceptance criteria
- priority recommendation

### 7. Prototype planning

Goal: expose logic issues by forcing them into screens and states.

Output:

- screen plan
- layout blocks
- key fields
- primary and secondary actions
- empty, loading, error, success states

### 8. AI capability design

Goal: make the AI part shippable, not just demo-able.

Output:

- system and user prompt structure
- input and output design
- schema recommendation when structured output is needed
- fallback rules
- evaluation plan
- regression examples for common failures

AI-specific checks:

- what exact cognitive task is AI solving
- what can fail and how bad that failure is
- whether retrieval, function calling, or rules are needed
- what should be deterministic vs model-generated

### 9. Test scenarios

Goal: turn vague quality concerns into executable checks.

Output:

- test objective
- starting conditions
- user role
- test steps
- expected outcomes
- edge cases
- minimum smoke test before launch

### 10. Metrics

Goal: define whether the product is getting better.

Output:

- North Star Metric
- 3-5 input metrics
- health metrics
- business metrics if relevant
- metric definitions, sources, thresholds
- review cadence

### 11. GTM

Goal: launch intentionally, not passively.

Output:

- target users
- channel strategy
- core messaging
- pre-launch, launch, post-launch actions
- 90-day GTM plan
- risks and success signals

### 12. Website scope

Goal: define the smallest useful website that should exist first.

Output:

- site goal
- target audience for the site
- sitemap
- page list
- must-have sections per page
- what is explicitly not in v1

### 13. Website copy

Goal: turn product strategy into website words people can understand.

Output:

- homepage headline and subheadline
- section-by-section copy
- CTA text
- FAQ suggestions
- proof or trust-building blocks needed

### 14. Website build plan

Goal: make the site buildable by an engineer or AI coding workflow.

Output:

- recommended stack
- page inventory
- shared components
- implementation order
- what can be hardcoded first vs dynamic later

### 15. Website launch QA

Goal: launch a usable site instead of an unfinished draft.

Output:

- QA checklist
- mobile and desktop checks
- analytics and conversion events
- SEO basics
- deployment checklist

## Output template

Use this structure unless the user asks for a different format:

```markdown
# [Phase Title]

## Current progress
- Current phase: [x/15]
- Completed: [completed phases]
- Now working on: [current task]

## Key conclusion
[Short answer first]

## Structured output
[Table / checklist / deliverable]

## Assumptions
- [Assumption 1]

## What is already validated
- [Validated point 1]

## Next input needed
- [Missing input 1]

## Next action
- [One clear thing the user should do next]
```

## Trigger questions to ask when context is missing

Ask up to 5 focused questions, such as:

- Who is the first user you want to serve?
- What painful workflow are you trying to change?
- What is the non-AI baseline today?
- What constraints matter most right now: time, budget, data, compliance, or team size?
- What stage is the product in: idea, validation, prototype, beta, or launch?
- Is your immediate goal to validate the product, or to get a real website live as soon as possible?

## Example use cases

- "Help me build an AI note-taking product from 0 to 1."
- "I have an AI product idea. Help me validate it before building."
- "Turn my AI product idea into strategy, PRD, user stories, and GTM."
- "Use AI tools to structure my whole product workflow from user research to launch."
- "Act like a product coach and guide me step by step until I ship a website."
