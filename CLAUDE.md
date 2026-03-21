# SearchGL — Claude Code Project Guide

## Project Overview

**SearchGL** is a Jekyll-based documentation site (GitHub Pages) providing systematic search methods for Korean health policy gray literature — materials not easily discoverable via standard search engines or LLMs.

- Live site: `https://wanderingstone.github.io/SearchGL`
- Jekyll theme: `just-the-docs`
- Language: Korean (ko-KR)

## Repository Structure

```
docs/
  _config.yml          # Jekyll config
  index.md             # Redirect to part1
  part1.md             # Guide: government & private organizations (A01–A15, B01–B22)
  part2.md             # Guide: integrated search databases (Core/부가/확장)
  downloads/
    guide_part1.txt    # LLM-optimized reference for Part 1
    guide_part2.txt    # LLM-optimized reference for Part 2
  assets/
    css/custom.css
    source.pdf
```

## Search Guide Rules (Critical)

The guide files enforce strict rules — follow these when assisting with searches:

1. **Never guess or generate URLs.** Only output URLs that exist in search results or have been directly verified.
2. **If a URL cannot be confirmed**, leave the field blank and mark it `확인 불가`.
3. **All listed organizations/DBs must be included** as search targets — no omissions.
4. Use URL status values: `직접확인` / `검색확인` / `확인불가`

## Search Database Priority

| Priority | Databases |
|----------|-----------|
| Core DB | 국립중앙도서관, 국회도서관, ScienceON, PRISM |
| 부가 DB | NKIS, 국립의과학지식센터, 알리오, RISS |
| 확장(민간) | DBpia, KISS, earticle, 교보문고 스콜라 |

## Remote Control Setup

This project is configured for use with **Claude Code remote control**, allowing you to access and continue this Claude Code session from any device (phone, tablet, browser via claude.ai/code).

### Starting a Remote Control Session

```bash
# Start Claude Code with remote control enabled
claude --remote-control

# Or start a dedicated remote control server
claude remote-control
```

### Within an Active Session

Use the `/remote-control` slash command to enable remote access mid-session.

### What Remote Control Provides

- Access the same Claude Code session from any device
- All local files, MCP servers, and project context remain available
- Sync continues seamlessly across devices

## Common Tasks

- **Editing the search guide**: modify `docs/part1.md` or `docs/part2.md`
- **Updating LLM reference files**: edit `docs/downloads/guide_part1.txt` or `guide_part2.txt`
- **Local preview**: run `bundle exec jekyll serve` from the `docs/` directory
- **Deploy**: push to `main` — GitHub Pages auto-deploys

## Development Branch Conventions

Feature branches follow: `claude/<description>-<sessionId>`
