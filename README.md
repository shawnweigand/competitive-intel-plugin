# Competitive Intel Plugin

Weekly competitive intelligence for your business — research competitor websites, surface recent posts, product updates, pricing changes, and upcoming events, then deliver a structured digest with a cross-competitor comparison.

## What it does

Give Claude a list of competitors and get back a structured digest showing what each one has been up to recently, followed by a comparison that highlights positioning gaps, feature gaps, and strategic trends you should be aware of.

The output is factual and neutral — no hype, no alarmism. Just clean intel you can act on.

## Requirements

No API keys or external configuration required. This plugin uses Claude's built-in web search — install and go.

## Installation

1. Download `competitive-intel.plugin` from the [Releases](https://github.com/shawnweigand/competitive-intel-plugin/releases) page
2. In Claude Cowork, open **Plugins** and choose **Install from file**
3. Select the `.plugin` file — that's it

## Components

### Commands

| Command | Description |
|---------|-------------|
| `/competitive-research [competitors]` | Full weekly digest for a list of competitors |
| `/add-competitor [competitor]` | Quick single-competitor lookup |

### Skills

| Skill | Triggers |
|-------|----------|
| `competitive-research` | Auto-triggered when you ask about competitors, request a digest, or use the commands above |

## Usage

### Full weekly digest

```
/competitive-research Notion, Coda, Obsidian
```

Or with URLs:

```
/competitive-research notion.so, coda.io, obsidian.md
```

You can also ask naturally:
- "Research my competitors: Acme Corp, Beta Inc, and Gamma Co"
- "Give me a weekly digest on these three companies: [list]"
- "What's new with [company] this week?"

### Quick single lookup

```
/add-competitor Notion
```

Gives you a focused report on one company without running the full multi-competitor digest.

## Digest structure

Each competitor gets a section with:
- **Recent blog posts & content** — articles and announcements from the past 7–14 days
- **Product updates & pricing changes** — new features, releases, or pricing page changes
- **Upcoming events** — webinars, conferences, or launches they've announced
- **Social media highlights** — notable activity on LinkedIn and Twitter/X

The digest closes with a **Competitive Comparison** covering:
- **Positioning gaps** — what competitors are emphasizing that you may not be
- **Feature gaps** — capabilities or offerings competitors are promoting
- **Strategic direction** — patterns across competitors signaling where the market is heading

## Notes

- If a section has no recent findings, it will say so explicitly rather than padding with old content.
- For best results, provide competitor names or website URLs. Both work.
- Each competitor section targets 200–300 words. A 3-competitor digest runs under 1,200 words.

## License

MIT — free to use, modify, and share.
