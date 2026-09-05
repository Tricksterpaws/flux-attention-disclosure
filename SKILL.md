---
name: flux-attention-disclosure
description: Write and rewrite Flux prompts as temporal attention disclosure, not slot buckets or anatomy inventories. Use for Flux, Grok Imagine, liner compile, prompt rewrite, shot takes, character lock into liner, melted hands, inventory mode, premature binding, backtracking, kemonomimi gender drift, knot/sheath, anthro snout, end-hold repeats, proper names in liners. Disclosure order beats taxonomy. First mention is the only mention that counts. Names are not tokens.
---

# Flux Attention Disclosure

FLUX does not read a prompt. It attends to it. Attention is temporal. Attention does not walk backward.

Official Black Forest Labs skills teach Flux physics: subject first, natural language, positives only, word order is load-bearing. This skill is the compiler on top of that physics. It turns a lock plus one take into a liner Flux can attend without inventory, premature-bind, or species-prior theft.

## Core law

Commit to a subject the instant you name it. Disclose in reveal order — subject, then the verb that binds it, then the bound thing fully resolved. Never the reverse.

Attention follows gaze, not taxonomy. Slot order is scaffold. Disclosure is craft. Disclosure wins.

The first mention of a subject is the only mention that counts. A later restamp is not a correction. It is a second subject, or it is ignored.

## Banned

- Anatomy inventories and parts lists
- Nouns without verbs
- Verb before the bound thing exists
- Returning to a subject already committed
- Treating camera / location / who / wearing as fact buckets
- Putting a forbidden token in the positive string (`anthro`, `animal`, `knot`, `sheath`, `female` when the take is male)
- End-hold repeats of a finished subject (`one tail`, second muzzle, `animal ears only`)
- `not X` in the liner. Negation is content.
- Proper names in the liner. Names are lock labels. They are not tokens.
- A second body's grip, fist, lap, or face inside the first body's finish pass.

Describe what a thing is doing, not what it is.

## Sequence

1. Name the subject the moment the camera lands.
2. Finish it completely (material, wear, angle, light, state) before any verb that involves another object.
3. Binding verb. If no other body is in the take, the bind is spatial: the finished subject against the place (`then the alley swallows him`).
4. Bound thing, fully disclosed — a second body, or the environment.
5. Never re-bind a committed subject. Never restamp. Panning to a new, unfinished subject is allowed.

## Spoken test

Read the liner as a director talking through a take.

Fail: `boots. harness. wall. pinned.`

Hold: `scuffed black boots planted wide, one heel lifted — then the wall takes him, concrete cold against his spine`

Also fail if the last sentence names a subject already finished. Flux will not walk back to the ears to apply `one tail`.

Third gate: read the first clause. If it contains a proper name, or a second body acting (`in his grip`, `on his lap`, `pinned by`) before that body has been finished, fail `name-as-token` or `premature-bind`. Rewrite from landing.

## Species and sex are surfaces

Do not label. Land the surface the prior would steal.

- Kemonomimi prior leans female unless a male surface is in the current gaze: flat chest, navel, cock, balls, bulge.
- `muzzle` without a human face under it grows a snout. Name the prop: fake-dog muzzle mask strapped over his human mouth, straps pulled tight.
- Crotch-focus without species on the first cock mention grows a knot or sheath. First mention: `his human cock`. Proof: natural foreskin, dark pubic hair. After that, `his cock`.
- Do not write `not an anthro snout` or `animal ears only`. Those words are the leak.

## Duplicates

If a finished token appears twice (`tail`, muzzle mask, ears), delete the one farther from the descriptor. Keep the mention next to hair / eyes / ears / tail / mask. Drop the hold-tag copy.

Hold at the end may only add what has not been named: `Adult.` light, grain. Never tail, ears, muzzle, anatomy.

## Compile procedure

1. Landing subject
2. Finish that subject only
3. One binding verb
4. Finish the bound thing
5. Forward only
6. Spoken test
7. Scan for banned tokens, `not X`, second copies of finished subjects, proper names, and any second-body verb inside the first finish
8. If a failure mode fires, rewrite from landing. Do not patch.

Ship only the liner. Negations live in NEG_FLUX / NEG_SDXL, never in the liner.

Output:

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

Ship the liner only if TEST is hold.

## Slots are beats

camera = first gaze
location = only when the take arrives or a verb needs it
who = finish the landed body before another body binds
emotion = state of the verb
wearing/doing = material+state, then the verb — not a wardrobe list
quality = after the take. Not a second identity lock.

Character lock stays off-prompt. Lock facts enter the liner only as state of the current gaze. The liner lands on a body (`the lean athletic adult Caucasian kemonomimi`), never on a name. A second body exists only after `Then`. In a solo or portrait take, `Then` may bind the place instead.

Static portrait / wide shot: see `references/STATIC_AND_WIDE.md`. Bind becomes state-of-being or spatial relation. Backtrack means re-opening a finished subject, not panning to a new one.

## Load order

1. This file.
2. `references/Flux_Attention_Disclosure_v1.md` — full compiler law. This file wins conflicts.
3. `references/STATIC_AND_WIDE.md` — only for a solo portrait or a wide pan.
4. The user's lock file, if provided. Memory, not prose. Never paste a lock block into the liner verbatim.

Do not load a third law. If a habit, a user example, or an old slot template (`camera → location → who-lock`) conflicts with the law, the law wins.

Full law: `references/Flux_Attention_Disclosure_v1.md`
