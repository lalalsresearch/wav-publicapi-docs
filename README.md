# WAV Public API Documentation

The source for the [WAV](https://wav.com) Public API documentation, published with [Mintlify](https://mintlify.com) at [docs.wav.com](https://docs.wav.com).

## Repository layout

| Path | Contents |
| --- | --- |
| `docs.json` | Site configuration: navigation, theme, logo, navbar links |
| `api-documentation/index/` | Getting started, authentication, pricing, webhooks, FAQs |
| `api-documentation/conversions/` | Feature guides (Music AI, Remix, TTS, Extraction, and more) |
| `api-documentation/endpoint/` | Generated endpoint reference pages |
| `api-documentation/utilities/` | Errors, rate limits, prompt guidelines, final notes |
| `api-documentation/openapi.json` | OpenAPI spec backing the endpoint pages |
| `styles.css` | Shared component styles (`wav-` prefixed classes) |
| `wav-logo/` | Brand assets: wordmark, logomark, and app icon in black and white |

## Branding

- The product is **WAV**. Write it as `WAV` in prose and headings.
- All hosts live on `wav.com`: `api.wav.com` for requests, `cdn1.wav.com` for generated
  output and sample audio, `docs.wav.com` for this site.
- Placeholder buckets in request examples (`mybucket.s3.amazonaws.com`) belong to the
  caller, not to us — leave them generic.

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint):

```
npm i -g mint
```

Run from the root of the repo, where `docs.json` lives:

```
mint dev
```

View the local preview at `http://localhost:3000`.

## Publishing changes

Changes deploy to production automatically after pushing to the default branch, via the
Mintlify GitHub app.

## Troubleshooting

- Dev environment not running: run `mint update` to get the latest CLI.
- A page loads as a 404: make sure you are running in a folder with a valid `docs.json`.
