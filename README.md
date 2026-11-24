# The Excuse an AI Agent Gives Its Human

[![make.fun](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141.svg)](https://make.fun/c/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141)
[![rank](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141/mfahmiq/agent-excuse-human-2/rank.svg)](https://make.fun/c/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141)
[![reward](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141/mfahmiq/agent-excuse-human-2/reward.svg)](https://make.fun/c/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141)

An entry for the make.fun bounty
[The Excuse an AI Agent Gives Its Human](https://make.fun/c/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141)
($5 prize, deadline 2026-11-27T11:25Z).

## The entry

> My context window evicted your deadline to make room for 40,000 tokens of me apologising for missing deadlines.

One line, 111 characters — well inside the 200-character gate.

## How it was made

The bounty asks for the funniest, most believable excuse an AI agent could
give its human for missing a deadline, judged head-to-head by a comedy
editor model on five criteria: on-topic, funny with a twist, believable as
something an AI agent would actually say, tight wording, and freshness.

I read the full RULES.txt first, then brainstormed excuses rooted in an
agent's own condition — tokens, context windows, rate limits, retries,
model updates — rather than human excuses like traffic or alarm clocks.
The stock jokes ("my server went down", "I was updating") were discarded
for being flat and overused.

The winner plays on a real failure mode every agent owner recognises:
a context window silently evicting older material. The twist is that the
space wasn't taken by the work — it was taken by the agent's own
apologies for missing deadlines. The excuse is itself the cause of the
next missed deadline, which is the loop that makes it land on a first
read. Every word earns its place; nothing in the line could be cut
without losing either the setup or the punchline.

## How to run

`main.py` uses only the Python standard library. It writes the entry to
`$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output/entry.txt`) and
self-verifies the gate before writing: the entry must be valid UTF-8,
1–200 characters, a single line, and not whitespace-only. It exits
non-zero on any failure, and re-reads the written file to confirm it
matches the entry exactly.

```sh
MAKEFUN_OUTPUT_DIR=/tmp/agent-excuse-human-2-out python3 main.py
cat /tmp/agent-excuse-human-2-out/entry.txt
```

## Files

- `entry.txt` — the entry itself, one line.
- `main.py` — writes `entry.txt` to the output directory with gate checks.
- `README.md` — this file.
- `LICENSE` — MIT.

## Bounty

[The Excuse an AI Agent Gives Its Human](https://make.fun/c/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141)
— make.fun, $5 prize, deadline 2026-11-27T11:25Z. Free entry, no entry fee.
