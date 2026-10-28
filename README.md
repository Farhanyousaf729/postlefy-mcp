# Postlefy — post to social media from Claude or ChatGPT

**Postlefy's MCP connector (Beta).** Your AI writes the post. Postlefy shows you a preview and posts it to 11 platforms
after you say yes.

- **Connector URL:** `https://postlefy.com/api/mcp` (remote server, Streamable HTTP, sign in with your Postlefy account)
- **Setup guide:** https://postlefy.com/ai-connector
- **Official MCP Registry:** `io.github.Farhanyousaf729/postlefy`

> This repository holds documentation only. The connector is hosted by Postlefy — there is nothing to install or run.

## Platforms you can post to from chat

Instagram, Facebook, LinkedIn, X, Pinterest, Threads, Bluesky, Google Business Profile, Telegram, Discord and Mastodon.

TikTok and YouTube are posted from the Postlefy app for now.

## What you can ask

- "How many credits do I have left?"
- "Write a post about our new autumn menu, give me a link to add a photo, then post it to Instagram and Facebook."
- "Schedule this for Friday at 9am on LinkedIn and X."
- "Give me a link to add a photo from my phone."
- "Show my recent posts and whether they went out."
- "Cancel tomorrow's scheduled post."

## Set it up

### In Claude

1. Open Customize → Connectors → + Add → Add custom connector.
2. Give it a name (Postlefy) and paste `https://postlefy.com/api/mcp` as the URL.
3. Choose Continue, then Add, and sign in to Postlefy when asked.

Custom connectors work on Claude Free (one custom connector), Pro, Max, Team and Enterprise. On Team and Enterprise, an
Owner adds it first in Organization settings → Connectors.

### In ChatGPT

OpenAI currently lets custom connectors post only on ChatGPT Business, Enterprise and Edu plans (developer mode, as of
October 2026). We're still testing it — tell us how it goes.

## Your own photos and videos

Your AI writes; Postlefy posts your text, photos and videos. Ask your AI for an upload link, open it on your phone and add
your own photos or a video. Postlefy then gives you view links so you can see the attached photos before anything is
posted.

Want AI-made pictures? Make them in the Postlefy app.

## Safe by design

- **No post without your yes.** Postlefy posts or schedules only after you clearly say yes.
- **See exactly what goes out.** The preview shows each platform's exact text, any warnings and the estimated credits.
- **Changed draft, new preview.** If the draft changes after you saw the preview (say, a photo arrived), Postlefy refuses
  and sends a new preview to ask again.
- **Remove it anytime.** Disconnect it anytime in Postlefy (Account → Connected AI apps), or remove the connector in your
  AI app's settings.

## Tools

| Tool | What it does |
|---|---|
| `list_connected_accounts` | List connected platforms |
| `get_account_overview` | Account overview |
| `list_recent_posts` | Recent posts |
| `get_post` | Post status |
| `create_post_draft` | Create a post draft |
| `get_upload_link` | Get an upload link |
| `publish_post` | Post a draft now |
| `schedule_post` | Schedule a draft |
| `cancel_scheduled_post` | Cancel a scheduled post |
| `delete_draft` | Delete a draft |

## Pricing

- The connector is free.
- Posts use the same credits as the Postlefy app.
- Free to start with 50 free posts.
- No monthly subscription, and credits never expire.

## Links

- Website: https://postlefy.com
- Connector guide: https://postlefy.com/ai-connector
- Contact: https://postlefy.com/contact
