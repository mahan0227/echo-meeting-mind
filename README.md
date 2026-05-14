# Echo Meeting Mind

Turn a **raw meeting transcript** into tight operational minutes: decisions, owners, risks, and a parking lot—optimized for speed, not ceremony.

## What it is

A BYOK Next.js microtool that distills messy dialogue into structured JSON you can paste into Notion, Linear, Jira, or Slack. One hop from browser → your API route → OpenAI.

## Why it’s useful

- **Saves time** for anyone who takes notes but hates reformatting.
- Surfaces **decisions vs discussion** so nothing ambiguous ships as “decided.”
- Captures **risks and parking lot** so follow-ups do not evaporate.
- Works from **Zoom/Otter/Fireflies** exports or hand-typed notes.

## Where you can use it

- **Engineering managers** — sprint planning, incident reviews, retro notes.
- **Startups** — weekly leadership syncs without a full-time chief of staff.
- **Sales & CS** — pipeline reviews and QBR prep from call transcripts.
- **Remote teams** — async handoff after a long thread or voice memo dump.

## Stack

Next.js 16 · React 19 · TypeScript · Tailwind CSS v4 · OpenAI Chat Completions (JSON mode)

## Run locally

```bash
npm install
npm run dev
```

## Production check

```bash
npm run build
npm run start
```

## API

`POST /api/minutes` · Header `Authorization: Bearer <key>`

Body: `transcript` (required), optional `model`.

## Suite brochure

[`docs/neuron-suite-brochure.html`](docs/neuron-suite-brochure.html) · [`docs/neuron-suite-ig-square.svg`](docs/neuron-suite-ig-square.svg)

## License

MIT
