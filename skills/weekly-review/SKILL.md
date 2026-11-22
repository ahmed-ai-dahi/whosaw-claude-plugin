---
name: weekly-review
description: Give a plain-English review of how a website did last week, using WhoSaw. Use when the user asks how their site, traffic or business website did this week or last week, asks for a weekly summary or report, or says "what happened on my site".
---

# Weekly review

Answer the way a friend who read the numbers would: a few short sentences, the one thing that matters, no analytics jargon.

## Steps

1. Call `list_sites`. If the user has more than one site and didn't say which, ask which one, listing the domains. If they have one, use it without asking.
2. Call `get_weekly_brief` for that site. This is the stored weekly brief and the main source.
3. Call `get_needs_attention` for the same site.
4. Only if the brief is missing or the user asks for more detail, call `get_traffic_summary` with `last_week_vs_previous`, and `get_traffic_sources` with the same period.

## How to answer

- Open with one sentence on the week: more, fewer or about the same visitors as the week before, with the two numbers.
- Then where visitors came from, and the top page, in one or two sentences.
- Then the items that need attention, each as one sentence with what to do next.
- If AI mentions are in the brief, end with one sentence on them.
- Say which week the numbers cover and when they were fetched.

## Rules

- Use WhoSaw's words: visitors, visits, stayed, time on site. Don't use GA4 terms such as sessions, engagement rate or users.
- Small numbers are normal for small sites. Say what changed, not that the numbers are low. A change of one or two visitors is noise; say so instead of calling it a trend.
- On a quiet week, say it was quiet. Don't invent a story.
- If the brief says Google Analytics isn't sending data, say that first and point the user to the fix WhoSaw gives.
- Never guess numbers that the tools didn't return.
