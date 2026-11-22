---
name: ai-visibility-check
description: Check whether AI assistants can read a website and whether they mention it, using WhoSaw. Use when the user asks if ChatGPT, Perplexity or Claude can see, read or find their site, whether AI recommends them, who AI suggests instead, or how to show up in AI answers.
---

# AI visibility check

Two questions, in this order: can the assistants read the site, and do they mention it when customers ask.

## Steps

1. Call `list_sites` and pick the site (ask only if there are several and the user didn't say which).
2. Call `get_ai_readability`. Note, per assistant, allowed or blocked, and how much of each page it can see.
3. Call `get_ai_mentions`. Note the mention rate per assistant this week and last, the questions tracked, the sites cited and who is suggested instead.

## How to answer

- Start with reading: "ChatGPT, Perplexity and Claude can all read your site" or name the one that is blocked and why.
- If pages show little of their text to assistants, say so: the site likely builds its pages in the browser, so assistants see an almost empty page.
- Then mentions: how many of the tracked answers mention the site, per assistant, against last week.
- Then who is suggested instead and which sites the answers cite, since those are where to get listed.
- End with the single most useful next step, in this order of priority: unblock a blocked assistant, make pages readable, then get onto the cited sites.

## Rules

- Readability comes before mentions. An assistant that can't read the site can't recommend it.
- Don't promise that any change will get the site mentioned. Nobody controls AI answers; say what improves the odds.
- If no questions are tracked yet, say so and explain that they are set up on WhoSaw's AI visibility screen.
- Report the time of the last check and the last questions asked.
