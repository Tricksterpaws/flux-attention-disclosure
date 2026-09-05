# Flux Attention Disclosure

A compiler skill for Flux liners.

Official Black Forest Labs skills teach Flux physics: subject first, natural language, positives only, word order is load-bearing. This skill is the compiler on top of that physics. It turns a character lock plus one take into a liner Flux can attend without inventory, premature-bind, or species-prior theft.

FLUX does not read a prompt. It attends to it. Attention is temporal. Attention does not walk backward.

## What this is

| Layer | Job |
|---|---|
| BFL `flux-image-best-practices` | Physics. Subject + action + style + context. No negatives on FLUX.2. |
| This skill | Compiler. Landing → finish → one bind → resolve → forward. Named fail modes. Spoken test. Rewrite from landing. |

Do not treat this as a third official BFL dialect. It is a production procedure the public docs left on the table.

## Install

Agent Skills layout. Load `SKILL.md` first.

```bash
npx skills add <your-github-user>/flux-attention-disclosure
```

Or copy the folder into an agent skills directory:

```
flux-attention-disclosure/
  SKILL.md
  AGENTS.md
  references/Flux_Attention_Disclosure_v1.md
  references/STATIC_AND_WIDE.md
  examples/hold-fail.md
```

Claude Code / Codex: point the project at this repo and tell the agent the first message in `AGENTS.md`.

## Load order

1. `SKILL.md` — short law, banned list, spoken test, output form
2. `references/Flux_Attention_Disclosure_v1.md` — full compiler law. Wins conflicts.
3. `references/STATIC_AND_WIDE.md` — only for a solo portrait or a wide pan
4. The user's lock file, if they provide one. Memory, not prose. Never paste it into the liner.

## Core law

Disclose in reveal order:

1. subject
2. the verb that binds it
3. the bound thing, fully resolved

Never the reverse.

The first mention of a subject is the only mention that counts. A later restamp is not a correction. It is a second subject, or it is ignored.

Names are lock labels. They are not tokens. The liner lands on a body, never on a name.

## Fail modes

`inventory` · `premature-bind` · `backtrack` · `slot-bucket` · `negation-content` · `species-prior` · `end-hold-repeat` · `name-as-token`

If any mode fires, rewrite from landing. Do not patch.

Worked pairs: `examples/hold-fail.md`.

## Output

```
LANDING:
FINISH:
BIND:
RESOLVE:
FORWARD:
LINER:
NEG_FLUX:
NEG_SDXL:
TEST: hold | fail
FAIL MODE: none | inventory | premature-bind | backtrack | slot-bucket | negation-content | species-prior | end-hold-repeat | name-as-token
```

The liner is the only string that ships to Flux. Ship it only if TEST is hold.

## What does not belong in this repo

- Character lock packets
- Outfit bibles
- Room inventories
- Proper names used as identity tokens
- A `scratchpad.md`

Lock memory stays in the user's private files. This repo is the law.

## License

MIT. See `LICENSE`.
