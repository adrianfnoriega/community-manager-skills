# Noriega Group — Community Manager AI System

## Project Overview

This project contains the Community Manager skill system for **Noriega Group**, a luxury real estate developer in Punta Cana, Dominican Republic.

## CM Skills (Slash Commands)

All skills live in `~/.claude/commands/` and are invoked as slash commands:

### Daily
| Command | Purpose |
|---------|---------|
| `/cm-daily-stories` | Generate 2-3 Instagram Stories with CTAs (run daily) |

### Weekly Workflow (Mon–Fri)
| Command | Purpose |
|---------|---------|
| `/cm-monday-plan` | Plan the week's content across all channels, create Monday.com calendar |
| `/cm-tuesday-copy` | Write all captions, story scripts, email copy, YouTube descriptions |
| `/cm-wednesday-design` | Generate Canva visuals + brief designer for complex pieces |
| `/cm-thursday-schedule` | Schedule all content via GHL Social Planner + cross-platform |
| `/cm-friday-review` | Weekly metrics, engagement review, recommendations |

### Monthly
| Command | Purpose |
|---------|---------|
| `/cm-monthly-report` | Full performance report across all channels |

### Utility (Ad-hoc)
| Command | Purpose |
|---------|---------|
| `/cm-create-post` | Quick single post for any platform |
| `/cm-repurpose` | Adapt content between platforms (blog→LinkedIn, reel→Shorts) |
| `/cm-email-nurture` | Create/review/optimize GHL email nurture sequences |
| `/cm-hashtag-strategy` | Generate hashtag sets per content pillar |
| `/cm-competitor-audit` | Competitive analysis via web search |
| `/cm-automation-setup` | Manage Make.com automation scenarios |

## MCP Integrations

| Service | Used For |
|---------|---------|
| GHL (GoHighLevel) | Social posting, CRM, conversations, pipeline management |
| Google Drive | Primary image source — project photos, renders, drone shots, lifestyle assets |
| MailerLite | Email campaigns, subscriber management, automations |
| Canva | Design generation, brand kit, visual exports (single-image, stories, thumbnails) |
| Gamma | Slide-based content, carousels, investor decks, monthly report presentations |
| Monday.com | Content calendar, weekly plans, reporting docs |
| Make.com | Cross-platform automation scenarios |
| Microsoft 365 | Outlook email & calendar, SharePoint files, Teams chat |

## Brand Context

- **Company**: Noriega Group
- **Projects**: Luxury real estate in the Dominican Republic
- **Website**: noriegagroup.com
- **Tone**: Aspirational, professional, warm. Luxury without being cold.
- **Languages**: Spanish (default), English (labeled for anglophone audience)

### Content Pillars
1. Education — CONFOTUR, ROI, buying process, DR market
2. Project — Construction updates, amenities, renders, available units
3. Lifestyle — Punta Cana, gastronomy, beach, golf, Caribbean luxury
4. Testimonials — Client stories, investor success, social proof
5. Team & Culture — Who we are, values, expertise

### Key Rules
- **Never** reveal exact prices — always direct to schedule a call
- **Always** include a clear CTA on every post/story
- Max 3 hashtags visible in caption; rest in first comment
- Nothing goes live without explicit user approval

### Buyer Personas
- **Inversionista latino** (35–55): ROI, CONFOTUR benefits. Spanish.
- **Lifestyle buyer** (40–60, anglophone): Second home/retirement. English.
- **Diaspora dominicana**: US/Europe-based, wants to invest in RD. Spanish/Spanglish.
