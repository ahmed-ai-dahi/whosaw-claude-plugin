---
name: traffic-change
description: Explain why a website's traffic went up or down, using WhoSaw. Use when the user asks why visitors dropped, why traffic fell or jumped, where a spike came from, or whether a change is something to worry about.
---

# Explain a traffic change

Find which source and which pages moved, and say it plainly. Most changes have one main cause.

## Steps

1. Call `list_sites` and pick the site (ask only if there are several and the user didn't say which).
2. Call `get_traffic_summary`. Use `last_week_vs_previous` for "this week" or "last week" questions and `last_28_days` for "this month" or longer.
3. Call `get_traffic_sources` with the same period and find the sources whose visitors changed most.
4. Call `get_top_pages` with the same period (limit 10) to see which pages carry the change, including the pages where visits started.
5. Call `get_needs_attention` in case WhoSaw already flagged the cause.

## How to answer

- First sentence: the size of the change, both numbers and the period.
- Second: the source behind most of it, for example "Most of the drop is Google search: 40 visitors, down from 95."
- Third: the page or pages involved, if one stands out.
- Then one or two likely reasons, labelled as likely, and one thing to check or do next.

## Rules

- Separate what the numbers show from what you suspect. Never present a guess as the cause.
- With fewer than about 20 visitors in either period, say the change may be chance and suggest looking at 28 days instead.
- If a source moved to "typed or bookmarked" or "other", mention that tracking links or setup can cause this.
- Use WhoSaw's words (visitors, visits, stayed), not GA4 terms.
