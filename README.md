# Career Planning

A Claude Code and OpenAI Codex skill for guiding thoughtful, structured career planning conversations and turning the result into a personalized career direction poster.

## What This Does

Career Planning helps people who feel unclear, stuck, or curious about their next career move think through their direction with structure.

Instead of jumping straight to advice, it walks the user through a 9-stage framework: current situation, motivation, strengths, possible directions, market reality, gaps, career narrative, and next actions. The assistant acts as a facilitator, not a decision-maker. The goal is not to tell the user what to do, but to help them see their own situation more clearly.

At the end, the skill generates a self-contained local HTML poster summarizing the user's career direction, core assets, gaps, recommendation, next steps, and success signal.

## Poster Output Preview

https://github.com/user-attachments/assets/857dd772-a649-4d62-a81b-37095ce1a403

## Key Features

- **9-Stage Framework** — A complete career planning flow from first uncertainty to concrete action.
- **One Question at a Time** — Keeps the conversation focused and emotionally manageable.
- **Evidence-Based Reflection** — Pushes gently for specific scenes, signals, and examples instead of accepting vague labels.
- **Different User Paths** — Adapts for full-time professionals, part-time/freelance users, and people with no work experience.
- **Market Reality Check** — Uses job descriptions, market requirements, and practitioner profiles when available.
- **Career Narrative Builder** — Turns scattered experience into a coherent "why this, why me, why now" story.
- **Self-Contained HTML Poster** — Produces a polished local poster in a single HTML file that can be opened in any browser.
- **Bilingual-Friendly** — Defaults to English, but naturally switches to Chinese when the user writes in Chinese.

## Installation

### Claude Code

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/thisisolivia/career-planning.git ~/.claude/skills/career-planning
```

Restart Claude Code after installation.

### Codex App / Codex CLI / Codex IDE Extension

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/thisisolivia/career-planning.git ~/.agents/skills/career-planning
```

Restart Codex after installation.

## Usage

In the Codex app, Codex CLI, or Codex IDE extension, start the skill explicitly:

```text
Use $career-planning to help me clarify my next career direction.
```

In Claude Code, invoke the skill by name if your setup supports slash commands or skill invocation:

```text
/career-planning
```

Then describe what you want help with:

```text
I want to clarify my next career direction.
```

Or describe your situation naturally:

```text
I don't know what to do with my career.
```

```text
Help me think through whether I should change jobs or change direction.
```

```text
我想重新规划一下我的职业方向。
```

The skill is designed to trigger whenever the user asks for help with career planning, career confusion, job dissatisfaction, career transitions, direction choice, or career storytelling.

## The 9 Stages

1. **Time Horizon** — Why now? How urgent is the decision?
2. **Current Situation & Motivation** — What is the user's current state, and what is driving the planning?
3. **Asset Inventory** — What skills, experiences, strengths, and blind spots are visible?
4. **Direction Elimination** — Which possible directions can be ruled out?
5. **Direction Prioritization** — Which direction should be primary, and what is the backup?
6. **Market Research** — What do job descriptions and practitioner backgrounds reveal?
7. **Gap Analysis** — What is missing between the user's current state and target direction?
8. **Narrative Construction** — How can the user explain their direction coherently?
9. **Action Framework** — What should they do next, and how will they know they are on track?

## Final Poster

After Stage 9 is complete, the skill asks the user to choose a poster style:

- **Clean Modern** — Light background, refined typography, muted ash tones.
- **Clean Modern Dark** — The same professional layout on a cool near-black background.

The poster includes:

- Name and career direction
- Motivation type and decision urgency
- Core assets
- Direction profile
- Six-node career story
- Gap analysis
- Current recommendation
- Priority next steps
- Success signal
- Version footer

Posters are generated as self-contained local HTML files under:

```text
career-planning-posters/<session-slug>/
```

Users can open the HTML file in any browser to review the poster.

## Architecture

This skill uses progressive disclosure: the main `SKILL.md` defines the workflow and rules, while detailed stage scripts and poster design specifications live in reference files.

| File                          | Purpose                                                                     | Loaded When                                   |
| ----------------------------- | --------------------------------------------------------------------------- | --------------------------------------------- |
| `SKILL.md`                    | Core workflow, trigger description, facilitation rules, poster output rules | Always                                        |
| `references/stages.md`        | Full 9-stage conversation script and decision logic                         | When running the career planning conversation |
| `references/poster-styles.md` | Poster layout, responsive rules, visual styles, and HTML requirements       | When generating the final poster              |
| `agents/openai.yaml`          | Codex/OpenAI-facing skill metadata                                          | By Codex/OpenAI-compatible environments       |

## Philosophy

This skill was built around a few beliefs:

**Career advice should not pretend to know more than the user.**  
The assistant helps structure thinking, but the final judgment belongs to the person living the career.

**Specific evidence beats vague self-description.**  
"I'm good at communication" is less useful than one concrete moment where communication changed an outcome.

**Direction is not only about desire.**  
A good career direction has to consider motivation, current assets, market needs, timing, and the story the user can credibly tell.

**A good summary should be shareable.**  
The final poster exists so the user can revisit the plan, discuss it with mentors, or refine it later.

## Requirements

- Claude Code, OpenAI Codex app, OpenAI Codex CLI, or OpenAI Codex IDE extension
- Git for installing from GitHub
- A browser for opening the generated HTML poster

## Credits

Created by [@thisisolivia](https://github.com/thisisolivia).

Built for people who want a clearer career direction without being handed generic career advice.

## License

MIT — Use it, modify it, share it.
