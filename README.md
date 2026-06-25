# design-hiring-persona-generator
Turn any job description into an interview sparring partner. Generates hiring manager and recruiter personas you can use for portfolio critique, mock interviews, and offer negotiation practice.

A copy-paste prompt for designers preparing for job interviews. Give it a job description and whatever intel you have. It generates a `persona.md` — a realistic hiring manager and recruiter you can load into Claude or Gemini to practice portfolio reviews, mock interviews, and salary negotiation.

No app. No account. No API costs on your end beyond your normal Claude/Gemini usage.

---

## What it generates

Two personas from a single prompt:

**Hiring manager** — calibrated to company size, AI maturity, and role seniority. Used for portfolio review, mock interviews, and generating strong questions to ask in your next round.

**Recruiter** — focused on comp, process, and offer dynamics. Used for offer call simulation and salary negotiation practice.

The personas adapt based on signals in the job description:
- A hiring manager at a 20-person AI-native startup reads portfolios differently than one at a 2,000-person enterprise
- A Staff-level role gets screened for org-level impact, not execution quality
- Companies where AI is the product expect you to have opinions about AI UX — companies using AI to build faster care more about your output velocity

---

## How to use it

### Step 1 — Open a new conversation

Go to [Claude](https://claude.ai) or [Gemini](https://gemini.google.com). Start a new chat.

### Step 2 — Paste the prompt

Copy the full contents of [`PROMPT.md`](./PROMPT.md) and paste it as your first message.

### Step 3 — Answer 4 questions

The prompt will ask you:

1. Is this an active opportunity or a dream company?
2. Paste your job description (or describe the role and company)
3. Any intel on the hiring manager? (optional)
4. Any intel on the recruiter or comp? (optional)
5. Archetype mode or immersive mode? (see below)
6. Which scenarios do you want? (portfolio review, mock interview, questions to ask, offer call, salary negotiation, or all)

### Step 4 — Save your persona.md

Copy the generated file and save it as `persona.md`. You'll reuse it across sessions.

### Step 5 — Activate a scenario

Open a **new** conversation. Paste your full `persona.md` as the first message. Then use one of the scenario prompts at the bottom of the file to start.

---

## Archetype mode vs. Immersive mode

| | Archetype | Immersive |
|---|---|---|
| **What it is** | Representative persona, explicitly labeled as inferred | Named persona with backstory, specific opinions, invented-but-realistic details |
| **Best for** | Exploring what a role type generally looks like, early research | Practicing actual conversations when you're in the process |
| **Accuracy** | Honest about uncertainty | Confident extrapolation — not a prediction about any real person |

If you're not sure which to pick: use **archetype** when you don't have a JD, **immersive** when you do.

---

## Example output

See [`example-persona.md`](./example-persona.md) — a Staff Product Designer role at Linear, immersive mode, all scenarios activated.

---

## What makes a better persona

More input = more useful output. The most impactful things to provide:

- **Job description** — even a rough one. The language companies use reveals what they actually care about.
- **Company stage** — seed vs. Series B vs. public changes the hiring manager profile significantly.
- **Role level** — mid, senior, staff, and principal are screened for completely different things.
- **Any hiring manager context** — even knowing their title and how long they've been at the company helps.

You can generate a useful persona with just a job description. You can generate a generic one with nothing — but it'll be a less precise mirror.

---

## Scenarios

### Portfolio Review
Share a case study. The hiring manager reviews it in character — asks clarifying questions, pushes back where they'd push back, tells you what's landing and what isn't.

### Mock Interview
Culture fit, behavioral, or portfolio presentation round. The hiring manager asks one question at a time and stays in character. Useful for practicing answers under mild pressure without getting coached mid-answer.

### Questions to Ask
The hiring manager generates the 6–8 most signal-rich questions you should ask them — ranked by how much they reveal about fit for you as a candidate evaluating the role.

### Offer Call Simulation
The recruiter calls to extend an offer. They give realistic numbers based on company stage and role level. You practice responding in the moment.

### Salary Negotiation
You push back on the offer. The recruiter stays in character, works within their constraints, and doesn't fold immediately. Practice the real back-and-forth.

---

## Tips

**Use a fresh conversation for each scenario.** The persona.md is the system context — don't run portfolio review and salary negotiation in the same thread or the model gets confused about who it's supposed to be.

**Give the scenario prompt real details.** "My counter is $175K base" works better than "I want more money." The more specific you are, the more realistic the simulation.

**Archetype personas are starting points.** If the generated persona doesn't feel right for what you know about the company, tell it: "This company is more design-immature than this persona suggests — adjust accordingly."

**Regenerate for different roles.** You're not locked to one persona per company. Generate a hiring manager persona for the role you're interviewing for, and a separate archetype persona for the same company at a different level to understand what growth looks like there.

---

## Contributing

This is an open-source prompt, not an app. Contributions welcome:

- Better calibration tables (company size, industry, role type)
- New scenarios (e.g., reference check simulation, take-home critique)
- Translations or adaptations for non-design roles
- Example personas for common company archetypes

Open a PR or file an issue.

---

## License

MIT. Use it, fork it, adapt it for your own job search or share it with your designer community.
