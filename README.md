# Community Manager Skills — Noriega Group

Claude Code slash commands for the Noriega Group community manager workflow. Covers daily stories, weekly content planning, design, scheduling, and reporting.

---

## Installation

1. Clone this repo
2. Copy the skill files into your Claude commands folder:

```bash
cp community-manager/*.md ~/.claude/commands/
```

3. Place `CLAUDE.md` in the root of your working directory (or Claude Code will use the one in this repo if you open it here)
4. `business-context.md` stays in the project root — all skills read it automatically for brand context

---

## Usage

Open Claude Code in the project directory, then run any slash command:

```
/cm-monday-plan
/cm-tuesday-copy
```

Every skill loads business context automatically from two sources:

1. **Local file** (primary): `business-context.md` in the project root — brand voice, personas, rules, hashtags, channel targets, posting times
2. **Google Drive** (supplemental): Skills search for a "Brand Context" / "Contexto de Marca" folder in Google Drive for updated guidelines, project sheets, or asset catalogs

To change brand context, edit `business-context.md` — all 14 skills inherit the changes.

---

## Commands

### Daily
| Command | Purpose |
|---------|---------|
| `/cm-daily-stories` | Generate 2–3 Instagram Stories with CTAs |

### Weekly (Mon–Fri)
| Command | Purpose |
|---------|---------|
| `/cm-monday-plan` | Plan the week's content, create Monday.com calendar |
| `/cm-tuesday-copy` | Write captions, story scripts, email copy, YouTube descriptions |
| `/cm-wednesday-design` | Generate visuals via Canva or Gamma, brief designer for complex pieces |
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
| `/cm-email-nurture` | Create/review/optimize MailerLite email nurture sequences |
| `/cm-hashtag-strategy` | Generate hashtag sets per content pillar |
| `/cm-competitor-audit` | Competitive analysis |
| `/cm-automation-setup` | Manage Make.com automation scenarios |

---

## Integrations Required

| Service | Used For |
|---------|---------|
| GHL (GoHighLevel) | Social posting, CRM, conversations, pipeline management |
| MailerLite | Email campaigns, subscriber management, automations |
| Canva | Design generation and exports (social images, stories, thumbnails) |
| Gamma | Carousels, investor decks, slide-based content, monthly report presentations |
| Monday.com | Content calendar and reporting |
| Make.com | Cross-platform automation |
| Microsoft 365 | Outlook email & calendar, SharePoint files, Teams chat |

Make sure your Claude Code session has the relevant MCP servers connected before running commands that use these integrations.

---

## Project Structure

```
NG CM/
├── CLAUDE.md                 # Project instructions for Claude Code
├── business-context.md       # Centralized brand context (edit here, not in skills)
├── README.md
└── community-manager/        # All 14 skill files
    ├── cm-monday-plan.md
    ├── cm-tuesday-copy.md
    ├── cm-wednesday-design.md
    ├── cm-thursday-schedule.md
    ├── cm-friday-review.md
    ├── cm-daily-stories.md
    ├── cm-create-post.md
    ├── cm-repurpose.md
    ├── cm-email-nurture.md
    ├── cm-hashtag-strategy.md
    ├── cm-competitor-audit.md
    ├── cm-monthly-report.md
    ├── cm-automation-setup.md
    └── cm-daily-engage.md
```

## Contributing

Skills are plain markdown files in `community-manager/`. To update a skill:

1. Edit the `.md` file
2. Commit and push to `main`
3. Team members pull and re-copy the updated file to `~/.claude/commands/`

To update brand context (tone, personas, rules, hashtags, channel targets), edit `business-context.md` — do not duplicate brand info in individual skills.
