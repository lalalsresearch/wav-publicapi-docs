# Documentation project instructions

## About this project

- This is the WAV Public API documentation site, built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Shared component styles live in `styles.css`, using the `wav-` class prefix
- Brand assets live in `wav-logo/`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

- The product is **WAV** (wav.com). Write it as `WAV` in prose, headings, and frontmatter.
- Never rewrite these to the WAV brand — they are live infrastructure, not branding:
  - API request host `api.musicgpt.com`
  - CDN output host `cdn1.musicgpt.com`
  - S3 sample-output buckets (`musicgpt.s3...`, `lalals.s3...`)
  - Published SDK package names on npm, PyPI, and Zapier (`musicgpt`)
- Say "conversion" for an API job, "API Key" (capitalized) for credentials.

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document the public API only — no internal endpoints, admin tooling, or unreleased models.
- Keep sample request/response payloads consistent with `api-documentation/openapi.json`.
