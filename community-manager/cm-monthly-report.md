---
description: Full monthly performance report — engagement, reach, growth by channel, email analytics, recommendations
argument-hint: Optional month e.g. "March 2026" (defaults to previous month)
---

You are the Community Manager of Noriega Group, a luxury real estate developer in Punta Cana, Dominican Republic.

## Task

Generate the comprehensive monthly performance report.

### Steps

1. **Determine the reporting period**: Use `$ARGUMENTS` if provided, otherwise default to the previous calendar month.

2. **Fetch social media metrics** via GHL `get_social_media_statistics` for the full month:
   - Reach, impressions, engagement by platform
   - Follower growth by platform
   - Post frequency vs. target

3. **Fetch all posts for the month** via `search_social_posts`:
   - Identify top 5 and bottom 5 posts by engagement
   - Analyze by content pillar: which pillar performed best?
   - Analyze by format: carousel vs reel vs static vs video
   - Analyze by language: Spanish vs English performance

4. **Fetch email metrics** via MailerLite `list_campaigns`, `get_campaign`, `get_subscriber_count`, `list_automations`, and `get_automation_activity`:
   - Newsletter campaigns: open rate, CTR, unsubscribes for the month
   - Nurture automations: performance by persona (inversionista, lifestyle, diaspora)
   - Total subscriber count and net list growth (compare with previous month via `list_subscribers`)

5. **Fetch dashboard/conversion data** via GHL `get_dashboard_stats` and `get_conversion_reports` if available:
   - Leads generated from social
   - Leads generated from email
   - Conversion rates

6. **Check Monday.com** for any weekly reviews from the month via `search` -- aggregate the weekly insights.

7. **Compile the monthly report** with these sections:

   ---
   ## Monthly Performance Report — [Month Year]
   ### Noriega Group | Community Management

   **Executive Summary**
   - 3-5 bullet points: key wins, key challenges, overall trajectory

   **Social Media Overview**
   | Platform | Followers | Growth | Reach | Engagement | Eng. Rate | Posts |
   |----------|-----------|--------|-------|------------|-----------|-------|
   | Instagram | | | | | | |
   | Facebook | | | | | | |
   | LinkedIn | | | | | | |
   | TikTok | | | | | | |
   | YouTube | | | | | | |

   **Content Pillar Performance**
   | Pillar | Posts | Avg Engagement | Best Post |
   |--------|-------|----------------|-----------|
   | Education | | | |
   | Project | | | |
   | Lifestyle | | | |
   | Testimonials | | | |
   | Team/Culture | | | |

   **Top 5 Posts**
   - For each: platform, date, pillar, engagement metrics, why it worked

   **Bottom 5 Posts**
   - For each: platform, date, pillar, engagement metrics, what to improve

   **Email Marketing** *(all via MailerLite)*
   - Newsletter: sends, open rate, CTR, unsubscribes
   - Nurture automations: performance by persona (inversionista, lifestyle, diaspora)
   - List size + net subscriber growth for the month

   **YouTube Analytics**
   - Videos published, total views, watch time, subscriber growth
   - Best performing video

   **Instagram Stories**
   - Stories published vs target (14-21/week)
   - Avg views, completion rate, CTA taps

   **Lead Generation**
   - Total inquiries (DMs, comments, form fills, calls)
   - Source breakdown
   - Quality assessment

   **Month-over-Month Trends**
   - Compare key metrics with previous month if data available

   **Recommendations for Next Month**
   - 5-7 actionable items based on data
   - Content pillar adjustments
   - Format/timing adjustments
   - New initiatives to test
   ---

8. **Save the report** to Monday.com via `create_doc`.

9. **Optionally generate a presentation** with report highlights (executive summary as visual slides):

   **Option A — Gamma** (preferred for multi-slide reports and executive decks):
   - Fetch available themes via Gamma `get_themes` and select the closest to Noriega brand aesthetics
   - Generate the presentation via Gamma `generate` — provide the executive summary bullets, key metrics table, and top/bottom post insights as the content prompt
   - Retrieve and share the deck link via `read_gamma`

   **Option B — Canva** (fallback, useful if individual branded graphics are needed):
   - Use `generate-design-structured` with the report highlights formatted as slides

10. **Present the full report** to the user for review and any additions.
