# Indian Astronomers Around the World — Website

This repository contains a minimal Jekyll site for the academic initiative *Indian Astronomers Around the World*. The site is intentionally simple and content-first, built with plain Jekyll and Markdown so it can be hosted on GitHub Pages.

## What this project is

- A static website using Jekyll (no JavaScript frameworks).
- Pages: Home, About, Events (each event is a Markdown file under `/events/`).

## Run locally

Install Ruby, then:

```bash
gem install bundler jekyll
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000/` in your browser.

## Add a new event

1. Create a new Markdown file in `/events/`, e.g. `2026-05-my-event.md`.
2. Add front matter at the top with at least the following fields:

```yaml
---
layout: default
title: "Event Title"
date: 2026-05-10 15:00:00 +00:00
event: true
summary: "One-line summary of the event."
---
```

3. In the body, include speaker, affiliation, abstract, format, links to recording/slides, and organizers.
4. Submit a Pull Request; maintainers will review and merge.

## Contribution guidelines

- Use PRs for changes and new events.
- Keep copy factual and concise; prefer Markdown.
- For site-wide style changes, open an issue first to discuss.

---
If you need help testing or building, I can assist with a minimal GitHub Actions workflow on request.
