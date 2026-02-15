# Article Specification

This document defines the standard for rank articles across both tracks:
- Individual
- SMB/MSP

No article files should be generated until an explicit user signal is given.

## Scope

- Two tracks:
  - Individual Privacy Ranks
  - SMB/MSP Privacy & Security Ranks
- One article per rank.
- Consistent structure across all articles, with audience-specific tone and depth.

## Target Audiences

### Individual Track

- Primary:
  - Non-technical users
  - Creators
  - Freelancers
  - Remote workers
- Secondary:
  - Journalists
  - Activists
  - Other high-risk users
- Guidance:
  - Include explicit "if high-risk" sections where relevant.

### SMB/MSP Track

- Primary:
  - SMB owners
  - Office managers
  - Non-technical or less-technical managers
  - IT leads
  - MSP account engineers
- Secondary:
  - Compliance-conscious operators under audit/insurance pressure
- Guidance:
  - Assume limited staff and time.
  - Write for mixed technical fluency, including readers below average on technical savviness.
  - Increase technical depth gradually as rank increases; beginner ranks stay plain-language first.

## Standard Article Structure

Each rank article should include:

1. Who This Is For
2. What This Rank Means
3. Threats This Rank Reduces
4. Minimum Viable Implementation (30-60 Minutes)
5. Standard Implementation
6. High-Risk Implementation
7. Tooling Options
8. Common Mistakes
9. Verification Checklist
10. When To Move To Next Rank
11. Dependencies
12. Maintenance Cadence
13. Incident Scenario

Authoring rule:
- Do not expose writing/process metadata in article headings.
- Keep vendor-neutral policy in the spec, not in heading text.
- Avoid meta-writing phrases in article prose (for example: `In real-world terms`).

### Length Pairing Rules

To keep all 13 sections usable at short length, apply section budgets:

- Who This Is For: 50-85 words
- What This Rank Means: 50-85 words
- Threats This Rank Reduces: 70-110 words
- Minimum Viable Implementation: 110-155 words
- Standard Implementation: 110-155 words
- High-Risk Implementation: 85-145 words
- Tooling Options: 50-95 words
- Common Mistakes: 50-95 words
- Verification checklist: 5-8 bullets
- When To Move To Next Rank: 3-5 bullets
- Dependencies: 50-85 words
- Maintenance Cadence: 35-75 words
- Incident Scenario: 140-220 words

Guidance:
- Keep the default target at 760-1150 words.
- Use a 1400-word ceiling only when complexity justifies it, mostly SMB ranks 11-16 where standards alignment is introduced.
- Incident scenarios should describe concrete events in sequence (what happened, response, outcome), not abstract summary language.

## Readability by Rank

- Individual ranks 00-03:
  - Target readability around 9th grade.
  - Keep sentences short and jargon minimal.
  - Apply this rule to all sections, including Dependencies.
  - Prefer concrete terms over abstract phrasing.
- Individual ranks 04-06:
  - Introduce moderate technical terms with short in-line explanations.
- Individual ranks 07-09:
  - Higher technical density is allowed.

## High-Risk Section Usage

- Individual ranks 00-03:
  - Do not include full high-risk guidance.
  - Use one short escalation line: if readers believe they are high-risk, they should prioritize ranking up quickly.
- Individual ranks 04-06:
  - Include only a brief optional high-risk note.
- Individual ranks 07-09:
  - Include full high-risk guidance.
- SMB/MSP ranks 01-08:
  - Keep high-risk guidance optional and light.
- SMB/MSP ranks 09-16:
  - Include high-risk guidance when relevant.

## Narrative Intent by Rank

- Early ranks:
  - Use payoff-first framing and low-friction examples.
  - Focus on convincing readers to take one small step.
- Mid ranks:
  - Balance motivation with practical examples and tradeoffs.
- Late ranks:
  - Reduce persuasion intensity.
  - Increase clarity on operations, constraints, and tradeoffs.

## Preferred Phrasing

- Use: `Believing "nothing to hide" means "nothing to lose"` when that concept is needed.
- Prefer `concrete default` over `strong default` in Individual track wording.

## SMB Framing Rules

- Favor influence over chore-list language.
- Prefer phrasing such as "organizations at this rank typically..." over imperative command lists.
- Use "signals of maturity" framing where possible.
- Present actions as examples/options unless baseline safety requires stronger wording.
- Keep ownership clarity, but avoid overloaded checklist tone in SMB ranks 01-08.

## Tone and Style

### Individual Track

- Practical
- Low jargon
- Behavior-first

### SMB/MSP Track

- Operational
- Policy-aware
- Explicit ownership and accountability

## File Layout (Proposed)

- `articles/individual/00.md` through `articles/individual/09.md`
- `articles/smb/01.md` through `articles/smb/16.md`

Notes:
- Use numeric filenames to preserve flexibility while rank titles evolve.

## Template v1 (Locked)

Use these exact section headings in this exact order:

1. `Who This Is For`
2. `What This Rank Means`
3. `Threats This Rank Reduces`
4. `Minimum Viable Implementation (30-60 Minutes)`
5. `Standard Implementation`
6. `High-Risk Implementation`
7. `Tooling Options`
8. `Common Mistakes`
9. `Verification Checklist`
10. `When To Move To Next Rank`
11. `Dependencies`
12. `Maintenance Cadence`
13. `Incident Scenario`

## Navigation Format (Locked)

Each article must include a navigation block at both the top and bottom with:

- `Track: Individual` or `Track: SMB/MSP`
- `Rank: <number>`
- `Previous: <link or None>`
- `Next: <link or None>`

Rules:
- First rank uses `Previous: None`.
- Last rank uses `Next: None`.
- Navigation links stay within the same track.

## Decisions

1. Length target per article:
   - Default short target: 720-1080 words
   - Adaptive ceiling for complex SMB ranks (typically 11-16): up to 1320 words
2. Voice:
   - Fantasy-flavored and story-like, while preserving practical real-world applicability
   - Intensity: medium fantasy
   - Fantasy flavor appears in framing/transitions/examples
   - Implementation and checklists remain plain and operational
3. Tool recommendations:
   - Vendor-neutral by default
   - Product names allowed only as examples

4. SMB/MSP standards references:
   - Introduce standards language starting at SMB Rank 11 (`Telemetry and Detection Plane`)
   - SMB Ranks 1-10: no standards language
   - SMB Ranks 11-16: include a short `Standards Alignment` section (2-4 bullets max)
   - Format:
    - `NIST CSF: ...`
    - `CIS Controls: ...`
    - `SOC 2: ...`

## Retrofit Rule

When this spec changes materially, regenerate pilot articles so they conform before bulk generation.

## Execution Gate

Do not generate article files until the user explicitly authorizes generation.
