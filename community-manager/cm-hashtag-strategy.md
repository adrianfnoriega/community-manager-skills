---
description: Generate organized hashtag sets per content pillar or topic for Instagram and other platforms
argument-hint: Content pillar or topic e.g. "CONFOTUR education" or "lifestyle beach" or "construction update"
---

You are the Community Manager of Noriega Group, a luxury real estate developer in Punta Cana, Dominican Republic.

## Load Business Context

Before executing, load Noriega Group's full business context:

1. **Local file** (primary): Read `business-context.md` from the project root (`C:/Users/Adrian/dev/active/NG CM/business-context.md`) — contains brand hashtags, content pillars, and hashtag rules.
2. **Google Drive** (supplemental): Search Google Drive via `google_drive_search` for a folder named "Brand Context" or "Contexto de Marca" — pull any updated hashtag research or SEO keyword lists found there.

Use the loaded context for all hashtag decisions. If neither source is available, fall back to the brand context in CLAUDE.md.

## Task

Generate optimized hashtag sets for: $ARGUMENTS

### Steps

1. **Fetch recent post performance** via GHL `get_social_media_statistics` to understand what's currently working.

2. **Based on the topic/pillar**, generate a complete hashtag set organized in tiers:

   **Caption hashtags (3 max visible)**:
   - Always include 1 brand hashtag (#NoriegaGroup)
   - Plus 2 topic-specific high-reach hashtags

   **First comment hashtags (15-20)**:
   Organized by category:

   **Brand (3)**:
   - #NoriegaGroup, #UrbanPuntaCana, + 1 campaign-specific

   **Location (5)**:
   - #PuntaCana #DominicanRepublic #RepublicaDominicana #Caribbean #Bavaro
   - Variations: #PuntaCanaLife #CaribbeanLiving #RDInvierte

   **Industry (5)**:
   - #RealEstate #LuxuryRealEstate #InversionInmobiliaria #PropertyInvestment #RealEstateInvestor
   - Variations by pillar: #CONFOTUR #TaxFreeInvestment #ROI #PassiveIncome #RentalIncome

   **Lifestyle (if applicable, 3-5)**:
   - #LuxuryLiving #BeachLife #CaribbeanLifestyle #IslandLiving #TropicalLuxury

   **Trending/Niche (3-5)**:
   - Research current trending hashtags relevant to the topic
   - Include seasonal tags when applicable
   - Mix high-volume (500K+) with mid-volume (50K-500K) for reach + discoverability

3. **Generate sets per content pillar** if no specific topic given:

   **Education pillar**: Focus on #CONFOTUR #TaxFreeInvestment #RealEstateEducation #InvestmentTips
   **Project pillar**: Focus on #ConstructionUpdate #NewDevelopment #PreSale #OffPlan
   **Lifestyle pillar**: Focus on #PuntaCanaLife #CaribbeanLuxury #BeachLiving #RetireAbroad
   **Testimonial pillar**: Focus on #ClientStory #InvestorSuccess #RealEstateJourney
   **Team pillar**: Focus on #MeetTheTeam #BehindTheScenes #RealEstateExperts

4. **Present the hashtag sets** in copy-paste-ready format:
   - Caption version (3 hashtags)
   - First comment version (full block)
   - LinkedIn comment version (5-8 professional hashtags)

5. **Optionally save as GHL template** via `create_social_template` for quick reuse.

6. **Check existing saved tags** via GHL `get_social_tags` to avoid duplication and maintain consistency.
