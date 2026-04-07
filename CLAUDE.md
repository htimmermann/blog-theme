# Claude Code Configuration

## Web Browsing

Use the `/browse` skill from gstack for all web browsing. Never use `mcp__claude-in-chrome__*` tools.

## Available gstack Skills

- `/office-hours` — Schedule or view office hours
- `/plan-ceo-review` — Plan CEO reviews
- `/plan-eng-review` — Plan engineering reviews
- `/plan-design-review` — Plan design reviews
- `/design-consultation` — Get design consultation
- `/design-shotgun` — Shotgun approach to design
- `/design-html` — Design HTML
- `/review` — Code review
- `/ship` — Ship changes
- `/land-and-deploy` — Land and deploy changes
- `/canary` — Canary deployment
- `/benchmark` — Run benchmarks
- `/browse` — Web browsing (preferred over mcp tools)
- `/connect-chrome` — Connect to Chrome
- `/qa` — Quality assurance
- `/qa-only` — QA only mode
- `/design-review` — Design review
- `/setup-browser-cookies` — Setup browser cookies
- `/setup-deploy` — Setup deployment
- `/retro` — Retrospective
- `/investigate` — Investigate issues
- `/document-release` — Document release
- `/codex` — Codex tool
- `/cso` — CSO tool
- `/autoplan` — Auto-planning
- `/plan-devex-review` — Plan developer experience review
- `/devex-review` — Developer experience review
- `/careful` — Careful mode
- `/freeze` — Freeze changes
- `/guard` — Guard mode
- `/unfreeze` — Unfreeze changes
- `/gstack-upgrade` — Upgrade gstack
- `/learn` — Learn mode

## Skill routing

When the user's request matches an available skill, ALWAYS invoke it using the Skill
tool as your FIRST action. Do NOT answer directly, do NOT use other tools first.
The skill has specialized workflows that produce better results than ad-hoc answers.

Key routing rules:
- Product ideas, "is this worth building", brainstorming → invoke office-hours
- Bugs, errors, "why is this broken", 500 errors → invoke investigate
- Ship, deploy, push, create PR → invoke ship
- QA, test the site, find bugs → invoke qa
- Code review, check my diff → invoke review
- Update docs after shipping → invoke document-release
- Weekly retro → invoke retro
- Design system, brand → invoke design-consultation
- Visual audit, design polish → invoke design-review
- Architecture review → invoke plan-eng-review
- Save progress, checkpoint, resume → invoke checkpoint
- Code quality, health check → invoke health
