# PawPal+ Project Reflection

## 1. System Design

**a. Initial design**

#### 1. What Pet Owners Actually Struggle With

Before designing the app, it's worth naming the real pain points, because they shape what the scheduler needs to *do*, not just what it needs to *store*.

| Pain Point | Why It Happens | Design Implication |
|---|---|---|
| Forgetting time-sensitive tasks (meds, allergy shots) | No single source of truth; mental load competes with work/kids | Meds/fixed-time tasks must be treated as non-negotiable anchors, not just "high priority" |
| Multi-pet households feel unfair or chaotic | Owner mentally juggles 2-4 pets' separate needs with one calendar | Plan must be per-pet aware, not just a flat task list |
| "I don't know if I'm doing enough" guilt/anxiety | No visibility into whether enrichment/grooming is being neglected vs. just deferred | Plan should explain *why* something was skipped, not just drop it silently |
| Time-crunched days cause silent task-skipping | When the day gets busy, lowest-effort tasks (walks, play) get cut first, often the most behaviorally important ones | Scheduler needs explicit priority + duration trade-off logic, with a visible "what got cut and why" |
| Inconsistent caregivers (partner, sitter, dog walker) | Tasks done twice or missed because there's no shared record | Core data model (Owner, Pet, Task) should not assume a single human actor forever |
| Income/tech-access variance | Not everyone has a smart feeder, smartwatch, or always-on phone | App should work as a simple manual entry tool, no hardware dependency |
---

## 2. Scope

1. Owner + Pet profile entry
2. Task CRUD (type, duration, priority, optional fixed time window, optional frequency)
3. Daily constraint input (available minutes / time blocks for the day)
4. Plan generation: sorts/allocates tasks into time slots given constraints
5. Plan display with reasoning ("Scheduled because...", "Deferred because...")
6. Unit tests for core scheduling rules

---

**b. Design changes**

- Did your design change during implementation?
- If yes, describe at least one change and why you made it.

---

## 2. Scheduling Logic and Tradeoffs

**a. Constraints and priorities**

- What constraints does your scheduler consider (for example: time, priority, preferences)?
- How did you decide which constraints mattered most?

**b. Tradeoffs**

- Describe one tradeoff your scheduler makes.
- Why is that tradeoff reasonable for this scenario?

---

## 3. AI Collaboration

**a. How you used AI**

- How did you use AI tools during this project (for example: design brainstorming, debugging, refactoring)?
- What kinds of prompts or questions were most helpful?

**b. Judgment and verification**

- Describe one moment where you did not accept an AI suggestion as-is.
- How did you evaluate or verify what the AI suggested?

---

## 4. Testing and Verification

**a. What you tested**

- What behaviors did you test?
- Why were these tests important?

**b. Confidence**

- How confident are you that your scheduler works correctly?
- What edge cases would you test next if you had more time?

---

## 5. Reflection

**a. What went well**

- What part of this project are you most satisfied with?

**b. What you would improve**

- If you had another iteration, what would you improve or redesign?

**c. Key takeaway**

- What is one important thing you learned about designing systems or working with AI on this project?
