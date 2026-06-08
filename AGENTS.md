# Agents

This is a GitHub profile repository (`cschanhniem/cschanhniem`). It is not a software project — it's a personal profile README with automated 3D contribution visualizations.

## What this repo does

- Hosts the profile README displayed on `github.com/cschanhniem`
- Runs a daily GitHub Actions workflow to generate 3D contribution skyline SVGs
- Contains no application code, no tests, no build system

## Structure

```
README.md                    # Profile page — the only file that matters
AGENTS.md                    # This file
.github/workflows/
  profile-3d.yml             # Daily 3D contribution generation
  link-check.yml             # Weekly broken link detection
  stale.yml                  # Auto-close stale issues
  repo-health.yml            # Weekly README freshness validation
profile-3d-contrib/          # Auto-generated SVGs — do not edit manually
```

## Rules

1. **Do not edit files in `profile-3d-contrib/`** — they are auto-generated daily by `yoshi389111/github-profile-3d-contrib`
2. **Do not add application code** — this is a profile repo, not a project repo
3. **Keep README.md concise** — it's the first thing people see on GitHub. Respect the reader's time.
4. **No AI slop** — no "leveraging synergies", no "passionate about", no generic badge tables, no emoji section headers. Write like a person who builds things.
5. **Show real work** — link to actual repos with actual descriptions. Stats are fine but substance matters more.
6. **Tone** — direct, specific, technical. Like a senior engineer's profile, not a marketing page.

## Editing README.md

When updating the profile README:

- Keep the structure: intro → projects → stack → stats
- Link to real repos with real descriptions
- Update the "What I'm shipping" section when new projects ship
- Keep the fintech and enterprise sections accurate
- Don't bloat it — if a project isn't worth showing, leave it out

## Workflow maintenance

- `profile-3d.yml` runs daily at 3 AM UTC — leave it alone
- `link-check.yml` validates README links weekly — fix broken links when flagged
- `stale.yml` auto-closes issues after 30 days — this is intentional for a profile repo
- `repo-health.yml` validates structure weekly — fix issues when flagged
