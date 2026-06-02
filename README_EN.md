# Tech Career Mentor AI

<a href="https://github.com/sthefanyalaminos/tech-career-mentor/blob/main/README.md">Traduzir para Português</a>

> A technology career guidance system with two chained AI agents — from self-discovery to an action plan.

---

## About the Project

**Tech Career Mentor AI** is a multi-agent system that guides users from discovering their professional profile to creating a personalized technology career study roadmap.

The project was developed as part of a learning journey in systems development and artificial intelligence, using two specialized agents that work in sequence:

| Agent | Role |
|-------|------|
| **Agent 1 — Interviewer** | Conducts a structured 7-question interview and suggests the 3 best tech careers for the user's profile |
| **Agent 2 — Planner** | Receives the profile from Agent 1 and generates a complete study plan with a 90-day roadmap, portfolio project, and interview guide |

---

## System Flow

```
User
   │
   ▼
┌─────────────────────────────────┐
│         AGENT 1                 │
│        Interviewer              │
│                                 │
│  • 7 structured questions       │
│  • Profile analysis             │
│  • Ranking of 3 careers         │
└────────────────┬────────────────┘
                 │  handoff with profile data
                 ▼
┌─────────────────────────────────┐
│         AGENT 2                 │
│          Planner                │
│                                 │
│  • Day-to-day overview          │
│  • Skills map                   │
│  • 90-day roadmap               │
│  • Portfolio project            │
│  • Interview guide              │
│  • Recommended DIO track        │
└─────────────────────────────────┘
```

---

## Features

### Agent 1 — Career Interviewer

- Conversational interview with 1 question at a time;
- Covers: motivations, prior experience, availability, work preferences, and goals;
- Applies an internal decision matrix (0–20 points) to rank careers;
- Presents the 3 careers with advantages, challenges, and market context;
- Performs a structured data handoff to Agent 2.

### Agent 2 — Roadmap Planner

- Receives profile data and personalizes the plan based on:
  - Hours available per week;
  - Experience level (none / beginner / some);
  - Goal (first job / career transition / current role growth).
- Generates:
  - Day-to-day overview of the chosen career;
  - Map of essential and complementary skills;
  - Detailed 90-day roadmap (week by week);
  - Portfolio project with deliverables and acceptance criteria;
  - Interview guide with 5 questions and how to answer them;
  - Recommended DIO learning track with next steps.

---

## Technologies & Concepts

- **Prompt Engineering** — Structured prompt design with behavioral instructions, conditional flow, and output formatting.
- **Multi-Agent Architecture** — Two agents with separate responsibilities communicating via data handoff.
- **Conversational UX** — Sequential question flow for a better user experience.

---

## How to Use

1. Paste the **Agent 1** prompt into your preferred AI environment (ChatGPT, Claude, Gemini, etc.).
2. Answer the 7 interview questions.
3. Choose one of the 3 suggested careers.
4. Paste the **Agent 2** prompt into a new conversation, along with the handoff data.
5. Receive your personalized study plan.

---

## Author

Developed by Sthefany Alaminos during the CI&T Bootcamp — From Prompt to Agent, hosted by DIO.