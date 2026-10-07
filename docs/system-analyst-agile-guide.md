# System Analyst in Agile: A Comprehensive Guide

> Note: the Atlassian task-tracker page and the referenced `x.zip` were not accessible when this
> guide was written. It is based on general Agile practice and the Atlassian Jira/task-tracking
> approach. Please add any zip-specific material.

## 1. Role of the System Analyst in Agile
The System Analyst (SA) bridges business stakeholders and the delivery team. In Agile the SA works
iteratively and collaboratively instead of producing one large up-front specification.

**Responsibilities**
- Elicit, analyze and refine requirements continuously.
- Translate business needs into user stories, acceptance criteria and technical/functional specs.
- Maintain and groom the product backlog together with the Product Owner (PO).
- Model processes, data and integrations (BPMN, UML, ERD, API specs).
- Clarify scope for developers and testers; support estimation and sprint planning.
- Validate delivered increments against requirements in reviews and UAT.

## 2. Task Tracking Fundamentals
A task tracker is the single source of truth for work: what is to be done, by whom, and its status.
(Atlassian: tools like Jira organise work into backlogs, boards and sprints.)

| Concept | Description |
|---|---|
| Epic | Large body of work, split into stories |
| Story | Value from the user's perspective |
| Task | Technical or non-functional unit of work |
| Sub-task | Smaller piece of a story/task |
| Bug | Defect in delivered functionality |
| Spike | Time-boxed research/investigation |

**Good task fields:** title, description, acceptance criteria, assignee, reporter, priority, estimate
(story points), labels/components, sprint, links (dependencies, designs, docs).

### Workflow (example board columns)
`Backlog -> Ready (refined) -> In Progress -> In Review -> In Testing -> Done`

Tips: limit work in progress (WIP), keep statuses few and meaningful, and define Definition of
Ready (DoR) and Definition of Done (DoD).

## 3. Agile Ceremonies and the SA's Contribution
| Ceremony | SA contribution |
|---|---|
| Backlog refinement | Prepare stories, split epics, clarify acceptance criteria, identify dependencies |
| Sprint planning | Explain requirements, help estimate, flag risks |
| Daily stand-up | Unblock questions, update analysis status |
| Sprint review | Demo/verify against acceptance criteria, gather feedback |
| Retrospective | Improve requirement quality and communication |

## 4. Requirements Engineering Workflow
1. **Discover** - interviews, workshops, observation, document analysis, existing-system review.
2. **Analyze** - stakeholder map, process models, gap analysis, constraints, risks.
3. **Specify** - epics -> stories -> acceptance criteria; NFRs (performance, security, usability).
4. **Validate** - walkthroughs with PO, devs, QA; prototypes/wireframes.
5. **Manage** - track changes, traceability, prioritisation (MoSCoW, WSJF, value vs. effort).

## 5. Writing Quality User Stories
**Format:** `As a <role>, I want <capability>, so that <benefit>.`

**INVEST:** Independent, Negotiable, Valuable, Estimable, Small, Testable.

**Acceptance criteria (Given/When/Then):**
```
Given a registered user is on the login page
When they enter valid credentials
Then they are redirected to the dashboard
```

### Story template
```
Title:
Story: As a ..., I want ..., so that ...
Context / Business value:
Acceptance criteria:
  - [ ] ...
Non-functional requirements:
Dependencies:
Out of scope:
Designs / API / Data links:
```

## 6. Modeling and Documentation Toolkit
- Process: BPMN, flowcharts, swimlanes
- Behaviour: use cases, sequence and activity diagrams, state machines
- Data: ERD, data dictionary, data-flow diagrams
- Integration: OpenAPI/Swagger specs, interface contracts
- UI: wireframes, prototypes, user journey/story maps

Keep docs "just enough" and live (e.g. Confluence/Wiki linked from tracker tickets).

## 7. Backlog Management
- Order by value, risk, dependencies.
- Keep top ~2 sprints of items "Ready".
- Use story mapping to see the user journey and plan releases/MVP.
- Regularly prune stale items.
- Estimate with story points / planning poker; track velocity.

## 8. Metrics and Reporting
- Burndown / burnup charts, velocity, cumulative flow diagram.
- Cycle time and lead time; control chart.
- Defect escape rate, requirement churn.

## 9. Collaboration with Roles
| Role | Interaction |
|---|---|
| Product Owner | Priorities, vision, acceptance |
| Developers | Feasibility, technical clarifications |
| QA | Testable criteria, test scenarios |
| UX/UI | Flows and prototypes |
| Scrum Master | Process impediments |
| Stakeholders | Needs, feedback, demos |

## 10. Choosing a Task Tracker
Evaluate: board/backlog support, custom workflows, reporting, integrations (Git, CI/CD,
docs), permissions, automation, cost. Common options: Jira, Trello, Azure DevOps, Asana, GitHub Projects.

## 11. Best Practices Checklist
- [ ] Every ticket has a clear goal and acceptance criteria
- [ ] DoR and DoD agreed by the team
- [ ] Requirements traced to tests and releases
- [ ] Changes communicated and recorded in the tracker
- [ ] Conversations preferred over documents; documents kept lean
- [ ] Regular feedback from stakeholders each sprint

## 12. Common Pitfalls
- Over-documenting or acting as a gatekeeper between PO and team
- Vague stories without acceptance criteria
- Stories too large to finish in a sprint
- Ignoring non-functional requirements
- Letting the tracker go stale
