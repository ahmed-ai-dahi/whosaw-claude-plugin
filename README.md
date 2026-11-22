# WhoSaw for Claude

Ask Claude about your website in plain English. WhoSaw reads your Google Analytics and checks how AI assistants see your site. This plugin connects Claude to your WhoSaw account and teaches it to answer like WhoSaw does: a few short sentences, the one thing that matters, no analytics jargon.

## What you can ask

- "How did my site do last week?"
- "Why did my traffic drop?"
- "Where do my visitors come from?"
- "Which pages bring people in?"
- "Can ChatGPT read my site?"
- "Does Perplexity mention my business? Who does it suggest instead?"

## What's inside

- **WhoSaw connector** (`https://whosaw.app/mcp`): eight read-only tools for your sites, weekly briefs, what needs attention, traffic summaries, top pages, sources, AI mentions and AI readability.
- **Skills:**
  - `weekly-review`: a plain-English review of last week.
  - `traffic-change`: finds the source and pages behind a rise or drop.
  - `ai-visibility-check`: whether ChatGPT, Perplexity and Claude can read your site, and whether they mention it.

## Setup

1. You need a WhoSaw account with a website connected: [whosaw.app](https://whosaw.app).
2. Add the plugin, then connect WhoSaw on the plugin's Connectors tab.
3. Sign in with your WhoSaw account and press Allow.

In Claude Code:

```
/plugin install whosaw --marketplace ahmed-ai-dahi/whosaw-claude-plugin
```

Full guide: [Use WhoSaw in Claude](https://whosaw.app/help/use-whosaw-in-claude).

## Data and privacy

- The plugin itself runs no code and stores nothing. The skills are instructions for Claude.
- The connector is read-only. It can't change anything in WhoSaw, and it can't see your Google account.
- When you ask a question, the WhoSaw data needed to answer it (site names, visitor numbers, pages, sources, AI visibility results) is sent from whosaw.app to Claude. It never includes AI answer text or your pages' text.
- You can disconnect at any time in WhoSaw under Settings, Account, Connected apps.
- WhoSaw's privacy policy: [whosaw.app/privacy](https://whosaw.app/privacy).

## Support

Email [support@whosaw.app](mailto:support@whosaw.app).

## License

MIT
