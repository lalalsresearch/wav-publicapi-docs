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
- Hosts, all on `wav.com` — keep them consistent and do not invent new ones:
  - `api.wav.com` — API request host, used in every curl and SDK sample
  - `cdn1.wav.com` — delivery host for all generated output and sample audio
  - `docs.wav.com` — this site; prefer root-relative links (`/api-documentation/...`) internally
- `mybucket.s3.amazonaws.com` and similar in request examples are placeholders for the
  *caller's* own storage. Leave them generic — they are not our infrastructure.
- Say "conversion" for an API job, "API Key" (capitalized) for credentials.
- SDK and integration links are withheld until those packages are republished under the
  WAV name; see `api-documentation/index/sdk.mdx`.

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document the public API only — no internal endpoints, admin tooling, or unreleased models.
- Keep sample request/response payloads consistent with `api-documentation/openapi.json`.
