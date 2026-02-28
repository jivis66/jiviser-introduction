# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a documentation repository containing curated daily consultation guides for AI content, food, fitness, and applications. All guides are in Chinese and structured for automated daily delivery.

## Project Structure

```
docs/
├── reddit-dailly.md    # AI subreddit monitoring guide (17:00 daily)
├── food-daily.md       # Recipe recommendation guide (13:00 daily)
├── fitness-daily.md    # Exercise consultation guide (07:00/20:00 daily)
└── ai-apps-daily.md    # AI application consultation guide (08:00/21:00 daily)
```

## Development Workflow

This repository contains only Markdown documentation. No build, test, or lint commands are required.

### Adding a new daily guide

1. Create a new `.md` file in `docs/`
2. Follow the established format: YAML metadata header, categorized source tables, weekly rotation schedule, output templates
3. Include both international and Chinese sources where applicable
4. Update this CLAUDE.md to reference the new guide

### Viewing content

```bash
cat docs/<filename>.md
```

### Standard commit format

```bash
git add docs/<filename>.md
git commit -m "Add <name>-daily.md <description>"
git push
```

## Content Guidelines

- Use YAML frontmatter for metadata configuration (schedule, rotation, preferences)
- Organize sources in tables with columns: name, type, URL/RSS, description, target audience
- Include HTML comments for category tags: `<!-- category: xxx -->`
- Provide both morning (brief) and evening (deep-dive) output templates where applicable
- All content is primarily in Chinese with translations for non-Chinese sources
