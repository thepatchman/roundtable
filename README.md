# Round Table

One question, up to five AI models, answering each other in turn.

A single static HTML file. No backend, no build step, no framework.

## How it reaches the models

Through [OpenRouter](https://openrouter.ai) — one account covering OpenAI,
Anthropic, Google, xAI, DeepSeek, Meta and the rest. A visitor connects their
own OpenRouter account and their own credits pay for their round.

There is no server and no key of ours anywhere. The key lives in the visitor's
browser and is sent to exactly one host: `openrouter.ai`.

Two ways in: OAuth with PKCE entirely in the browser, or paste a key from
https://openrouter.ai/keys.

## Modes

- **Relay** — each model reads everything said before it and answers the last
  speaker by name.
- **Blind** — nobody sees anyone. The fair comparison.

Pause at any point to cut in yourself; what you write enters the transcript and
the next model sees it.

## Deploying

It is one file. GitHub Pages will serve it from this repo with no build step —
Settings → Pages → deploy from `main`. Any static host works the same way.

## A note on what you will see

Models disagree less than you would hope. That is not a bug in the table, it is
what these systems are like: trained to be agreeable, reading much the same
internet. The useful part of a round is rarely the consensus. It is the one seat
that breaks from it, and what it says next.
