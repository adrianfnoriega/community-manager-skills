# Community Manager Skills — Noriega Group

Claude Code slash commands for the Noriega Group community manager workflow. Covers daily engagement, weekly content planning, design, scheduling, and reporting.

---

## Installation

1. Clone this repo
2. Copy the skill files into your Claude commands folder:

```bash
cp community-manager/*.md ~/.claude/commands/
```

3. Place `CLAUDE.md` in the root of your working directory (or Claude Code will use the one in this repo if you open it here)

---

## Usage

Open Claude Code in a directory that has `CLAUDE.md` (brand context), then run any slash command:

```
/cm-monday-plan
/cm-tuesday-copy
```

Claude will use the brand context from `CLAUDE.md` automatically.

---

## Commands

### Daily
| Command | Purpose |
|---------|---------|
| `/cm-daily-stories` | Generate 2–3 Instagram Stories with CTAs |
| `/cm-daily-engage` | Review DMs/comments, draft responses, flag leads |

### Weekly (Mon–Fri)
| Command | Purpose |
|---------|---------|
| `/cm-monday-plan` | Plan the week's content, create Monday.com calendar |
| `/cm-tuesday-copy` | Write captions, story scripts, email copy, YouTube descriptions |
| `/cm-wednesday-design` | Generate Canva visuals, brief designer for complex pieces |
| `/cm-thursday-schedule` | Schedule all content via GHL Social Planner |
| `/cm-friday-review` | Weekly metrics, engagement review, recommendations |

### Monthly
| Command | Purpose |
|---------|---------|
| `/cm-monthly-report` | Full performance report across all channels |

### Utility
| Command | Purpose |
|---------|---------|
| `/cm-create-post` | Quick single post for any platform |
| `/cm-repurpose` | Adapt content between platforms (blog→LinkedIn, reel→Shorts) |
| `/cm-email-nurture` | Create/review/optimize GHL email nurture sequences |
| `/cm-hashtag-strategy` | Generate hashtag sets per content pillar |
| `/cm-competitor-audit` | Competitive analysis |
| `/cm-automation-setup` | Manage Make.com automation scenarios |

---

## Integrations Required

| Service | Used For |
|---------|---------|
| GHL (GoHighLevel) | Social posting, email campaigns, CRM |
| Canva | Design generation and exports |
| Monday.com | Content calendar and reporting |
| Make.com | Cross-platform automation |

Make sure your Claude Code session has the relevant MCP servers connected before running commands that use these integrations.

---

## Contributing

Skills are plain markdown files in `community-manager/`. To update a skill:

1. Edit the `.md` file
2. Commit and push to `main`
3. Team members pull and re-copy the updated file to `~/.claude/commands/`
