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

1. Who this is for
2. What this rank means
3. Threats this rank reduces
4. Minimum viable implementation (30-60 minutes)
5. Standard implementation (baseline best practice)
6. High-risk implementation (optional escalation)
7. Tooling options (2-4 examples, non-prescriptive)
8. Common mistakes (expanded "Boss Fight")
9. Verification checklist (pass/fail style)
10. When to move to next rank (exit criteria)
11. Dependencies (prerequisites)
12. Maintenance cadence (daily/weekly/quarterly)
13. Incident scenario (short failure + recovery example)

### Length Pairing Rules

To keep all 13 sections usable at short length, apply compact section budgets:

- Who this is for: 40-70 words
- What this rank means: 40-70 words
- Threats this rank reduces: 60-90 words
- Minimum viable implementation: 90-130 words
- Standard implementation: 90-130 words
- High-risk implementation: 70-120 words
- Tooling options: 40-80 words
- Common mistakes: 40-80 words
- Verification checklist: 5-8 bullets
- When to move to next rank: 3-5 bullets
- Dependencies: 40-70 words
- Maintenance cadence: 30-60 words
- Incident scenario: 80-120 words

Guidance:
- Keep the default target at 600-900 words.
- Use a 1100-word ceiling only when complexity justifies it, mostly SMB ranks 11-16 where standards alignment is introduced.

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
7. `Tooling Options (Vendor-Neutral, Example Products)`
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
   - Default short target: 600-900 words
   - Adaptive ceiling for complex SMB ranks (typically 11-16): up to 1100 words
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

## Execution Gate

Do not generate article files until the user explicitly authorizes generation.
