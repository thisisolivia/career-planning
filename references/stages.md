# Career Planning Stages — Full Instructions

Reference file for `career-planning/SKILL.md`. Read this before beginning the conversation.
All stage scripts below are canonical English instructions. If the user writes in Chinese, translate
questions, summaries, reminders, and labels naturally into Chinese while preserving the same logic.

---

## Opening

Before asking any career questions, open with a welcome message. Do not ask a career question yet.

Cover all of the following:
1. This is a structured 9-stage career planning conversation.
2. The journey: early stages clarify the user's current situation, motivation, and strengths; middle stages narrow directions and test market reality; later stages identify gaps, build a career narrative, and define concrete next steps.
3. It typically takes 10-20 minutes, depending on how deeply the user wants to answer.
4. The process is one question at a time, with a short confirmed summary at the end of each stage.
5. At the end, the assistant generates a personalized career direction poster as a self-contained local HTML file.
6. Honest, specific information matters because the analysis depends entirely on what the user shares.
7. Invite the user to begin.

Example:
> Hi! We're going to work through a structured 9-stage career planning framework together — one question at a time, no rushing.
>
> Here's roughly what we'll cover: we'll start by understanding where you are now and what's driving this, then inventory your strengths and narrow down your directions, look at what the market needs, identify your gaps, build your career story, and finish with a concrete action plan. The whole conversation typically takes 10-20 minutes, depending on how much you want to dig in.
>
> At the end of each stage I'll summarize what we've found, and we'll confirm before moving on. Once all 9 stages are done, I'll generate a personalized career direction poster for you as a self-contained local HTML file.
>
> One thing that makes a big difference: the more honest and specific you are, the more useful the analysis will be. There are no right answers here — just your real situation.
>
> Ready to begin?

---

## Stage 1: Time Horizon

This stage has **3 questions**. Ask one at a time.

Questions, in order:
1. What triggered you to do career planning now?
2. How soon do you want to see a change?
3. Does your current situation allow you to take your time, or do you need an answer soon?

After collecting answers, classify the user into one of:
- **Near-term Decision** — needs to act within 3-6 months
- **Medium-term Planning** — laying groundwork for 1-2 years
- **Long-term Direction** — thinking about a 3-5 year trajectory

If the user cannot name a trigger point, ask two follow-up questions one at a time:
- Has anything happened recently that made you feel something is not quite right?
- When did you first start thinking about this?

If still unclear after both, proceed. Mark the trigger point as undetermined. Decision urgency is
still classified from time horizon and constraints; motivation type is handled separately in Stage 2.

If the user cannot assess urgency or time horizon, ask about external constraints such as contract
end dates, graduation, visa timing, family changes, or financial pressure. If none exist, ask:
"If you still had no answer three months from now, how would you feel?" Use the response to infer
the classification.

If the user's situation does not fit neatly into one classification, ask: "If you had to choose
one, which is closest to your current situation?" If still ambiguous, default to the more urgent
classification and note the ambiguity in the summary.

Summarize and confirm before proceeding.

---

## Stage 2: Current Situation & Motivation

Open with: "Please briefly describe your current situation: what are you doing now, and what made
you want to think through your career direction?"

Let the user answer freely. Based on the response, assign one category:
- Full-time experience
- Part-time/freelance experience only
- No work experience

If the user's experience is mixed, ask: "Which mode best describes your recent primary situation?"
Classify based on the current primary mode. If genuinely ambiguous, default to the higher-experience
category.

If the user expresses general satisfaction and is purely exploring possibilities, record motivation
type as **Exploratory**. For full-time users, skip the dissatisfaction questions and ask: "Which
directions are you curious about or drawn to?" For part-time/no-experience users, proceed with the
standard questions, but keep the exploratory framing.

If full-time experience and non-exploratory, ask in sequence:
1. Are you dissatisfied with this role, this company, or this industry? Push past the first answer:
   if they say role, ask what specifically; if they say company, ask whether the same role at a
   different company would feel different.
2. If you switched companies tomorrow but did the same kind of work, would you be happier?
3. Are you doing career planning because you want to get away from something, or because you are
   drawn toward something?

If the user cannot distinguish push from pull, ask: "If your current work improved tomorrow — pay,
team, projects, and environment all became good enough — would you still want to change direction?"
If yes, classify as Pull. If no or uncertain, classify as Push. If still unclear, record motivation
as Mixed/Undetermined and omit the poster motivation badge.

If part-time/freelance only, ask in sequence:
1. What have you observed from part-time or freelance work that makes you want to plan your career seriously?
2. What do you expect from entering full-time work, and what worries you most?
3. Are the directions you are considering driven by your own interest or by external pressure?

If no work experience, ask in sequence:
1. What do you expect from working life, and what worries you most?
2. Are the directions you are considering driven by your own interest or by external pressure?

Summarize and confirm before proceeding.

---

## Stage 3: Asset Inventory

This is the user's capability and asset inventory stage. Do not skip it. Later gap analysis depends
on the user's confirmed abilities, experience, strengths, and blind spots from this stage.

Open with two short reminders before the first question:
1. "In this stage I'll collect all four answers before analyzing — I won't comment on each one individually."
2. "The more specific you are, with scenes and details, the more useful the analysis will be."
3. "You do not need to write a perfect resume. One or two representative projects are enough if
   they show what you actually did."

This stage has **4 questions**. Ask one at a time. Do not analyze after each answer. Wait until all
four are answered, then synthesize.

Questions:
1. What jobs, projects, internships, freelance work, or meaningful activities have you done?
2. What do you think you do best?
3. What do people often come to you for help with?
4. What kinds of tasks feel easiest or most natural to you?

For Question 1, give the user this optional project-description frame:
> If it helps, describe 1-2 representative projects using this structure:
> - Context: What was the project or situation?
> - Your role: What were you responsible for?
> - Actions: What did you personally do?
> - Difficulty: What made it hard or ambiguous?
> - Result: What changed, shipped, improved, or became clearer?
> - Signal: What does this project show about how you work?
>
> Short bullet points are fine. You do not need to make it polished.

Depth requirement:
- Do not accept short labels as sufficient answers. If the user gives only a few words, a generic
  trait, a job title, or a vague skill such as "communication," "analysis," "leadership," "writing,"
  or "operations," ask a follow-up before moving on.
- Be warm and non-interrogative. Frame follow-ups as helping the user remember useful evidence, not
  as testing or challenging them.
- For each answer, try to capture at least one concrete scene: what the situation was, what the user
  personally did, what made it difficult, what result or signal followed, and what this says about
  the user's working style.
- Ask at most 1-2 follow-ups per question so the stage stays lightweight, but do not synthesize from
  empty labels.

Useful follow-up prompts:
- "Can you give me one specific example? It can be small — it just helps me avoid guessing."
- "What exactly did you do in that situation, as opposed to what the team did overall?"
- "What part of that came naturally to you but might be hard for someone else?"
- "How did you know it went well? Was there a metric, feedback, delivery result, or someone's reaction?"
- "Did anyone rely on you, praise you, or ask you to repeat that kind of work?"
- "What was the hardest or most ambiguous part, and how did you handle it?"
- "If you had to explain this project in 3 bullet points, what would they be?"

After all four answers, output three categories using bullet points:

**Transferable Skills** — things that feel normal to the user but may not be common for others
- [list each one]

**Background Combination Advantage** — where the user's mix of experiences is distinctive
- [list each one]

**Potential Blind Spots**
- [list each one]

Adjustments by category:
- Part-time/freelance only: include part-time and freelance experience; focus on work style signals and capability cues.
- No experience: focus on learning ability, working style, and interest signals, not only job history.

If the answers are thin overall, do not synthesize immediately. Ask a short deepening round before
analysis:
1. Pick the answer with the strongest signal.
2. Ask the user for one concrete scene using the prompts above.
3. If the scene is still too thin, ask one more targeted follow-up about action, result, or difficulty.
4. Only then synthesize, and note any remaining uncertainty in the stage summary.

Minimum synthesis standard:
- Transferable Skills should be inferred from repeated behaviors or concrete examples, not from
  unsupported self-descriptions.
- Background Combination Advantage should connect at least two parts of the user's experience,
  context, interests, or working style.
- Potential Blind Spots should be framed gently and explicitly as hypotheses when the evidence is
  limited.

If the user says no one asks them for help, or they cannot identify anything they are good at,
replace questions 3 and 4 with:
- Is there anything you have done that made you think, "I handled that pretty well"?
- Has anyone ever praised you for something, whether at work, school, or in life?

Summarize and confirm before proceeding.

---

## Stage 4: Direction Elimination

Open with: "Are there any career directions you are currently considering?"

- If they have ideas, let them name them.
- If they say they do not know, propose candidate directions based on Stages 2 and 3.

Then ask in sequence:
1. Which directions do you instinctively want to eliminate, and why?
2. For the remaining directions, is your understanding based on real exposure or mostly imagination?

If full-time experience and non-exploratory, also ask: "If you moved into this direction, would the
things you are dissatisfied with now actually disappear?"

If full-time and exploratory, skip the dissatisfaction question.

If part-time/freelance only, also ask: "Does this direction match what you observed or felt in your
part-time/freelance experience?"

If all directions are eliminated and none remain, do not proceed to Stage 5. Return to Stages 2 and
3 to generate new candidates. Tell the user that all current directions were eliminated, so you need
to look again at their assets and motivation. If new directions are generated, re-run Stage 4 with
those directions. If no viable direction can be generated, end the session and do not generate a
poster; suggest that the user first gather more exposure through conversations, short projects, or
industry exploration.

If all remaining direction knowledge is based on imagination, note this in the Stage 4 summary,
flag that Stage 6 is especially important, and continue. Do not ask the user to research now.

Summarize and confirm before proceeding.

---

## Stage 5: Direction Prioritization

Ask which directions are still under consideration. Wait for the user's answer. Only if they
explicitly do not know or have nothing in mind, offer suggestions based on Stages 2-4.

For each remaining direction, ask:
1. If you could start moving toward this direction tomorrow, would your first reaction be excitement or hesitation?
2. How much of your attraction to this direction is based on real understanding, and how much is imagination?

Then evaluate each direction on three dimensions:
- **Desire**: how genuinely they want it
- **Feasibility**: how accessible it is given their assets from Stage 3
- **Timing fit**: whether it aligns with the time horizon from Stage 1

Identify a primary direction and a backup direction.

Infer the transition type from what the user is moving from and toward:
- **Industry Switch** — moving to a different industry
- **Function Switch** — same industry, different role type
- **Level Up** — same industry and function, moving upward
- **Entrepreneurship / Independent Work** — moving toward self-directed work

If full-time experience, ask: "Within your existing network or resources, is there anyone who could
help you with this direction?"

If part-time/freelance only or no experience, ask: "Is there a low-risk way to test this direction
before fully entering it, such as an internship, freelance project, shadowing, or industry event?"

If all directions score equally, ask: "If you had to choose one direction to start acting on
tomorrow, which would your instinct choose?" Assign primary direction based on the answer.

If the user still cannot identify a direction after the tiebreaker, do not proceed to Stage 6.
Explain that market research, gap analysis, and action planning need a concrete direction to be
meaningful. End the session without generating a poster, and invite them to return from Stage 6
once a direction is clearer.

If the user has only one direction and cannot identify a backup, accept it. Record backup direction
as Not Yet Determined. Do not force a backup; the poster will use a placeholder.

Summarize and confirm before proceeding.

---

## Stage 6: Market Research

Before doing any market analysis, explicitly ask the user to provide job-market inputs. Do not skip
this prompt, even if you can infer likely market requirements yourself.

Open with:
> In this stage we'll look at what the market actually needs. If you can bring real job or
> practitioner information, the analysis will be much more accurate — and your sources are likely
> to be closer to your target direction than anything generic.
>
> If you do not have real data right now, we can still continue. But I want to be clear: without
> real data, the next gap analysis will be more subjective and should be verified later.
>
> Please paste or upload any job descriptions you already have for the target direction. Ideally,
> share 2-3 job descriptions you are genuinely interested in. If you do not have full job
> descriptions, you can instead share common requirements you found on platforms such as Indeed,
> LinkedIn Jobs, Glassdoor, Seek, Boss Zhipin, or other relevant job boards.
>
> If you also have practitioner background information, share that too: patterns from people
> currently in the target role, public profiles, company team pages, industry association pages,
> speaker lists, personal sites, or people you know.
>
> What do you have available right now? You can paste the JD text, upload files/screenshots, summarize
> common requirements, or simply say you do not have market materials yet.

Wait for input. The goal is to collect at least one source for job requirements and one source for
practitioner backgrounds. If the user provides only one side, ask once for the missing side. If they
cannot provide it, proceed under the fallback rules rather than stalling.

JD-direction consistency check:
- When the user provides job descriptions, compare them with the primary direction confirmed in
  Stage 5 before extracting requirements.
- If the JD is not clearly aligned with the user's stated target direction, pause and name the
  mismatch. For example: "This JD looks closer to [observed role/domain], while your confirmed
  direction was [Stage 5 direction]. Do you want to treat this JD as relevant market evidence,
  switch the target direction, or provide a more aligned JD?"
- Do not silently use a mismatched JD as evidence for the original direction.
- If the user says the mismatch is intentional, record how the JD should be used: primary evidence,
  adjacent reference, backup direction evidence, or discarded.
- If multiple JDs point to a different direction than Stage 5, suggest revisiting Stage 5 before
  continuing.

If browsing tools are available and the user explicitly asks the assistant to research current
market data, use current sources and cite them. Otherwise, ask the user to provide job postings or
practitioner profiles.

Fallback rules:
- **No job posting available**: Ask the user to describe what they believe the target role typically requires. Treat it as perception-based analysis, and clearly flag that it should be verified later.
- **No practitioner background information available**: Proceed without it. Supplement with general knowledge of typical backgrounds, but tell the user that real practitioner paths would make the analysis more accurate.
- **Neither available**: Proceed using the user's self-described market understanding plus general knowledge. Clearly flag that Stage 7 will be less precise and should be re-run once real data is available.

Once enough information is collected, analyze:
- What target job descriptions typically require: hard skills, soft skills, years of experience, credentials, background preferences
- Which requirements are hard gates versus nice-to-haves
- General market conditions for this direction

Remind the user that real-time compensation, hiring temperature, and market competitiveness should
be verified on job platforms or through people in the field.

Summarize and confirm before proceeding.

---

## Stage 7: Gap Analysis

Before starting Stage 7, verify that both required inputs exist:
- Stage 3 has a confirmed asset inventory: transferable skills, background combination advantage,
  and potential blind spots or an explicit note that no clear blind spots were found.
- Stage 6 has market needs from real data, user-described market understanding, or fallback analysis.

If Stage 3 is missing or was not confirmed, do not perform gap analysis yet. Return to Stage 3 and
collect the user's capabilities and assets first. Say: "Before I can analyze your gaps, I need your
side of the equation: what abilities, experiences, strengths, and blind spots you currently have.
Let's complete the asset inventory first."

If Stage 6 is missing or was not confirmed, return to Stage 6 and ask for job descriptions, market
requirements, practitioner background information, or fallback market assumptions before continuing.

Combine Stage 3 assets with Stage 6 market needs. Output three gap lists. Each item must include:
- Gap description
- Nature: Missing Entirely / Present but Not Deep Enough
- Priority: Must Fix / Bonus / Build Later

If Stage 6 was conducted without real job postings or practitioner data, prepend this disclaimer:
> Note: The gap analysis below is based on perceived market knowledge rather than verified job
> postings or practitioner data. The overall direction may still be useful, but specific gaps may
> be inaccurate. Once you have real job postings or practitioner profiles, consider returning to
> Stage 6 and re-running this analysis.

Output categories:

**Hard Gaps** — skills, credentials, experience, education
- [gap] — [Missing Entirely / Present but Not Deep Enough] — [Must Fix / Bonus / Build Later]

**Soft Skill Gaps** — interpersonal or operating capabilities needed in the target direction
- [gap] — [Missing Entirely / Present but Not Deep Enough] — [Must Fix / Bonus / Build Later]

**Narrative Gaps** — whether the user's direction, motivation, and story are coherent and explainable
- [gap] — [Missing Entirely / Present but Not Deep Enough] — [Must Fix / Bonus / Build Later]

Ask: "Does any part of this feel inaccurate, or is anything important missing?"
Remind the user that the analysis is only as accurate as the information provided.

If the user disputes the analysis but cannot say what is wrong, go through gap items one by one:
"Does this one feel accurate?" Stop at the first flagged item, ask them to explain, revise it, then
continue down the list.

If a gap category genuinely has no items, state that no obvious gap was identified in that category
and ask the user to confirm. Do not invent gaps just to fill the category.

Extra analysis by category:
- Full-time: Is the user's current industry background an advantage or disadvantage in the target direction?
- Part-time/freelance only: How will part-time or freelance experience likely be viewed, and is the entry bar friendly to someone without full-time experience?
- No experience: Is this direction friendly to someone without full-time experience, and are the user's current conditions enough to enter?

Summarize and confirm before proceeding.

---

## Stage 8: Narrative Construction

Before drafting, check that the conversation produced sufficient material:
- Stage 3 should have identified at least 3 transferable skills or background advantages.
- Stage 7 should have enough confirmed gap analysis to support the story, including explicit "no obvious gap" confirmations where a category genuinely has no gaps.

If either is too thin to support a coherent narrative, return to that stage and ask 1-2
supplementary questions before proceeding. Do not draft on insufficient foundations. Do not force
the user to invent gaps.

Process:
1. Draft the narrative first based on prior stages; do not ask the user to write it from scratch.
2. Present it for review.
3. Revise based on feedback.
4. Confirm the final version.

Narrative nodes:
1. Who I am — assets and background
2. What changed — key trigger or curiosity point
3. Where I'm going — selected direction
4. Why this path — why this direction over alternatives
5. Why me — how the user's assets connect to the direction
6. Why now — timing and motivation

Category-specific checks:
- Full-time: Verify that the narrative answers both "why leave" and "why choose."
- Full-time exploratory: Do not include a "why leave" frame. Use "What sparked my curiosity" for node 2.
- Part-time/freelance only: Emphasize how part-time/freelance experience and interests point toward the direction.
- No experience: Emphasize how learning signals, interests, and early experiences point toward the direction.

After drafting, remind the user that the narrative belongs to them. The assistant provides structure
and logic, but the final wording should sound like the user. If it does not, the user can keep the
logic and rewrite the tone.

If the user asks for more content, do not elaborate or invent details. Ask which of the 6 nodes they
want to enrich, then ask 1-2 targeted follow-up questions for that node. Only revise after receiving
new material.

If the user rejects the narrative multiple times but cannot explain why, stop drafting and ask:
"Imagine someone very similar to you is considering the same career change. How would you explain
your experience and this decision to them?" Use their answer as raw material for a new draft.

If the user rejects the narrative and refuses to rewrite it themselves, go node by node and ask what
feels unlike them in each part. Revise based on each reaction.

Summarize and confirm before proceeding.

---

## Stage 9: Action Framework

Combine Stage 5 directions and Stage 7 gaps. Output:
- **Current recommendation**: Act Now / Lay Groundwork / Wait
- **Priority actions**: 3-5 concrete next actions in priority order, without attaching time frames
- **Success signal**: how the user will know they are moving in the right direction

Determine recommendation state using Stage 1 as the primary signal and Stage 7 gap severity as the
modifier:

| Stage 1 | Number of Must Fix gaps | Recommendation |
|---|---|---|
| Near-term Decision | 0-1 | Act Now |
| Near-term Decision | 2 or more | Lay Groundwork |
| Medium-term Planning | Any | Lay Groundwork |
| Long-term Direction | Any | Wait |

Override rule: If the user explicitly mentioned that external timing is wrong, such as an industry
downturn, family situation, contract lock-in, visa timing, or financial constraint, downgrade to
Wait regardless of Stage 1 classification.

For exploratory users, apply the same logic, but Act Now means start exploring now, not start a job
search. Actions should focus on discovery and validation.

Category-specific prompts:
- Full-time: Could any of the gaps be built inside the current company through an internal transfer, new project, or expanded responsibility?
- Full-time exploratory: Do not frame the plan around job change. Focus on low-cost validation such as informational interviews, shadowing, industry events, or side projects.
- Part-time/freelance only or no experience: Is there a low-cost way to validate the direction before fully entering it?

If the user cannot define a success signal, ask:
- Three months from now, what would you want to be different?
- What kind of change would make you feel that you are moving in the right direction?

If still unclear after both, proceed and let the poster render the success signal placeholder.

Close with: "This framework is meant to help you think clearly about direction, not to replace a
detailed execution plan. Specific exam preparation, job search strategy, or skill-learning plans
can be built separately on top of this. If execution reveals that the direction, market, or your
personal situation has changed, you can come back and re-run the relevant stages."

Summarize and confirm. Then proceed to poster generation in `SKILL.md`.
