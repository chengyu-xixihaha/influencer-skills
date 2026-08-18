# Influencer Skills

Agent Skills for influencer-marketing operations across **TikTok, Instagram, and YouTube** — creator discovery, audience-fit scoring, and evidence-based shortlisting. Built on the open [Agent Skills](https://agentskills.io) standard (`SKILL.md`), so they run in Claude Code, OpenAI Codex CLI, Cursor, Gemini CLI, OpenClaw, and other compatible agents.

## Skills

| Skill | What it does |
|---|---|
| `influencer-lead-discovery` | Search creators/content, expand similar creators, enrich profiles, produce outreach-ready lead lists |
| `influencer-audience-fit-scoring` | Evaluate audience geography/language/age/gender/interests/**follower authenticity**, compare creators, score fit |
| `influencer-realtime-enrichment` | Fetch freshness-critical profile/media/video details and latest content during active campaigns |
| `influencer-campaign-monitoring` | Create/list/refresh/stop monitor tasks, pull metrics, download tracked assets, post-campaign review |
| `influencer-commerce-intel` | TikTok Shop monetization signals — sale/goods/live/video-ad data, product details, commerce potential |

## Install

```bash
npx skills add chengyu-xixihaha/influencer-skills
```

Or install a single skill:

```bash
npx skills add chengyu-xixihaha/influencer-skills --skill influencer-lead-discovery
```

## Zero-config free tier

These skills work out of the box — **no API key required**. Calls route through a hosted gateway that injects credentials server-side, subject to a shared daily free quota.

## Unlock your own quota

When the free quota is exhausted (HTTP `429`), register and get your own API key at **https://data.scdata.cc/pricing**, then set:

```bash
SCRUMBALL_API_KEY="your-key"
```

in your host/agent environment (or a local `.env`). Your calls then run against your own quota.

## Data

Creator and audience data covers TikTok, Instagram, and YouTube (search, profiles, similar creators, brand collaborations, audience demographics, follower authenticity, and more). See each skill's `references/` for the full operation index.

## License

MIT
