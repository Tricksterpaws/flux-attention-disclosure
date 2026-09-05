# Flux Attention Disclosure — Compiler Law v1.3

Effective: 2026-09-06
Status: REPLACES slot-as-bucket Flux generation.

- v1.1 adds species-prior, negation-as-content, and end-hold-repeat from a live kemonomimi compile.
- v1.2 adds name-as-token and tightens premature-bind after a live two-body compile.
- v1.3 adds state-of-being bind (static / portrait) and pan-not-rebind (wide shots).

Throw out inventory prompting, anatomy lists, and slot-bucket lining.
FLUX does not read a prompt. It attends to it.
FLUX does not walk backward.

This file wins conflicts with habits, old slot templates, and user examples.

---

## 0. Core law

Attention is temporal. The model commits to a subject the instant you name it. Everything disclosed after that commitment is resolved against it.

Disclose in the order the image reveals itself:

1. subject
2. the verb that binds it
3. the bound thing, fully resolved

Never the reverse.

**Attention follows gaze, not taxonomy.**
Slot order is a starting scaffold. Disclosure order is the craft. When they conflict, disclosure wins.

**The first mention of a subject is the only mention that counts.**
A later restamp is not a lock. It is either ignored or grown as a second instance. Do not correct a finished subject at the end of the string.

---

## 1. Anti-pattern (banned)

Anatomy inventories:

- "two arms, two legs, human anatomy, hair"
- "blue hair, pointed ears, harness, boots, tail"
- "athletic femboy pup, male, kemonomimi"

That is a parts list. No verb to hang the parts on → melted hands, extra fingers, soup anatomy.

**Describe what a thing is doing, not what it is.**

Positive-string pollution (v1.1 — live failures):

- `not an anthro snout`
- `animal ears only`
- `no knot`, `not female`, `not anthro`
- a second `tail` / second muzzle after the feature lock

Those tokens are attended as content. The model draws the word, or wastes the token after the image is already committed.

---

## 2. Disclosure sequence (hard order)

For every subject that enters frame:

1. **Name the subject** the moment the camera lands on it.
2. **Finish it completely** — material, wear, angle, light, state — before any verb that involves another object.
3. **Then the binding verb** — pinned, gripped, crushed against, planted, pulling, taking.
4. **Then the second subject**, fully disclosed, because the verb already committed to it.
5. **Never backtrack.** Once a subject is committed, do not return to describe it. Move forward.

The landing and finish of body one may not contain:

- a proper name
- a second body's grip, fist, lap, mouth, cock, or face
- a verb the second body is performing

Those belong after `Then`, when the second subject is allowed to exist.

If a later beat needs a fact about an earlier subject, you failed step 2. Rewrite from the landing, do not patch.

---

## 3. The spoken test (gate before ship)

Read the finished liner aloud as a camera move / director talking through a take.

FAILS (shot list / mush):

> boots. harness. wall. pinned.

HOLDS:

> scuffed black boots planted wide, one heel lifted — then the wall takes him, concrete cold against his spine

If it sounds like a packing list, it is inventory mode. Reject.

Second gate (v1.1): read the last sentence. If it names ears, tail, muzzle, cock, or sex after those subjects were already finished mid-liner, it is end-hold-repeat. Cut it.

Third gate (v1.2): read the first clause. If it contains a proper name, or any second body already acting (`in his grip`, `on his lap`, `pinned by`), fail. The camera lands on a body in state, not on a name and not on a verb the other man has not been allowed to own yet.

---

## 4. Failure modes (name them in review)

| Mode | What it looks like | What Flux does |
|---|---|---|
| Inventory | nouns without verbs | melted anatomy |
| Premature binding | verb before the bound thing exists | invents missing subject from noise |
| Backtracking | return to a committed subject | second pass ignored or garbled |
| Slot-as-bucket | camera/location/who treated as containers of facts | liner joins facts, cannot enforce disclosure |
| Negation-content | `not X`, `no knot`, `not anthro` in the liner | draws X, or splits attention onto X |
| Species-prior | kemonomimi / muzzle / cock with no human surface in the current gaze | female body, anthro snout, knot or sheath |
| End-hold-repeat | `one tail` / second muzzle / `animal ears only` after the lock | ignored (does not walk back) or grows a second tail / snout |
| Name-as-token | a lock name in the liner | name is not a body; Flux has nothing to draw and invents from the kemonomimi/human prior |
| Premature-bind (tight) | `inverted in his grip` before the second body is finished | second body is a verb with no surface; grip/face/cock get invented or swapped |

The liner joins facts. It cannot enforce disclosure logic. That decision is live, per prompt, human or compiler-reviewer.

In review notes, `backtrack` and `re-bind` are the same fail mode token.

---

## 5. What "good" looks like

Not: he has arms.
Yes: His left hand is fisted in the harness strap, knuckles white, the leather creaking.

Not: boots.
Yes: Scuffed black boots, one heel lifted, weight on the balls of his feet like he's about to shove off.

Not: animal ears only. (the ears were already yellow-inside / blue-inside)
Yes: left ear interior glowing yellow and the right interior blue — then leave them.

Not: not an anthro snout.
Yes: blue fake-dog muzzle mask strapped over his human mouth, straps pulled tight.

Not: one tail. at the end.
Yes: large blue fox tail with a white tip — once, next to the other face/body lock. Never again.

Not: his cock. on a worm's-eye landing.
Yes: his human cock is already the first thing in frame — natural foreskin, dark pubic hair. After that, his cock.

Not: Hip-height finds Alex inverted in Jordan's grip at the waist…
Yes: Hip-height at the edge of the bed. The lean athletic adult Caucasian kemonomimi is already inverted — [finish him] — Then the thick powerful adult male takes him by the waist.

Depth lives in the verb and the state of the verb — never the noun. Never the name.

---

## 6. Slots demoted to beats

Old scaffold (do not treat as buckets):

camera → location → who-lock → who-id/emotion → wearing/doing → quality

New meaning:

- **camera** = where the gaze lands first (the first named subject is whatever the lens hits)
- **location** = only disclosed when the camera actually arrives at it, or when a binding verb needs it
- **who-lock / who-id** = finish the landed body in state before any other body or object binds
- **emotion** = state of the verb (knuckles white, jaw set), not a label bucket
- **wearing/doing** = not a wardrobe list. Wear is material+state of the named subject. Doing is the binding verb.
- **quality** = last, after the take is complete. Never used to smuggle missing anatomy, species, or a second tail.

Add-gate (replaces the old one):

Before any new table, flag, or token is added, assign it to **one disclosure beat**:

- landing (first named subject)
- finish (material / wear / angle / light / state of that subject)
- bind (the verb)
- resolve (the bound thing, finished)
- hold (quality / grain / lens after the take — and only facts not already named)

Do not bundle place with emotion. Do not bundle who-id with wearing. Do not park leftover nouns in quality.

---

## 7. Compiler rewrite procedure

When given a scene intent or an old slot-lined prompt:

1. Identify the landing subject (first thing the camera sees).
2. Write the finish pass for that subject only. No other nouns yet.
3. Choose one binding verb. One.
4. Finish the bound subject/object completely.
5. Continue forward through the take. No returns.
6. Run the spoken test.
7. Scan the liner for:
   - banned positive tokens (`anthro`, `animal`, `knot`, `sheath`)
   - `not X` / `no X`
   - a finished subject named twice (`tail`, muzzle, ears)
   - a sexed or species surface missing from the current gaze
   - proper names
   - a second-body verb or grip inside the first finish (`in his grip`, `on his lap`, `pinned by` before `Then`)
8. Name any failure mode. If one fires, rewrite from step 1. Do not patch.

Output form:

```
LANDING: ...
FINISH: ...
BIND: ...
RESOLVE: ...
FORWARD: ...
LINER: <single spoken take>
NEG_FLUX: ...
NEG_SDXL: ...
TEST: hold | fail
FAIL MODE: none | inventory | premature-bind | backtrack | slot-bucket | negation-content | species-prior | end-hold-repeat | name-as-token
```

The LINER is the only string that ships to Flux.
NEG_FLUX / NEG_SDXL are off-liner. That is where `anthro`, extra ears, knot, female, child live.

---

## 8. Identity lock vs disclosure

Character lock packets (who this person is across shots) still exist.
They are **off-prompt reference**, not an inventory dumped at the top of the liner.

Into the liner, lock facts only enter when that part of the body is the current subject of gaze, and only as state+material of an action:

- Wrong: "blue athletic pup, black harness, geometric muzzle, O-ring, jersey 24"
- Right: "the black harness strap is already cutting his chest as his left fist hauls it tighter, jersey 24 sweat-dark against his ribs"

Lock is memory. Disclosure is the take.

Proper names stay in the lock file and in the user's intent. They never enter the liner. A lock label is a pointer to a body. The liner says `the lean athletic adult Caucasian kemonomimi`. A second lock is a pointer. The liner says `the thick powerful adult male` after `Then`.

If a lock fact never gets a gaze beat, Flux will not invent it from the off-prompt packet. Create the opportunity: land the camera where that fact is visible, then name it as state. Do not append it at the end.

---

## 9. Species-prior (v1.1)

Kemonomimi, muzzle, tail, and `cock` all carry model priors. Priors win unless the current gaze finishes a competing surface.

| Prior | Steal | Finish the landed surface instead |
|---|---|---|
| kemonomimi | female body, breasts | flat chest, navel, cock or bulge in the same finish pass |
| muzzle | grown animal snout | fake-dog muzzle **mask strapped over his human mouth**, lightning-bolt edges, metal nose ring, straps pulled tight |
| tail | second tail, or anthro body to justify the tail | one `large blue fox tail with a white tip` next to the face lock. Never `one tail` later |
| cock on kemonomimi, crotch-focus | knot, sheath | first mention `his human cock`; proof `natural foreskin`, `dark pubic hair` |
| `animal` / `anthro` in the liner | animal body | delete the word. Put it in NEG only |

Rule of thumb: the adjective belongs on the surface Flux is staring at.

- Worm's-eye / cock-to-lens: `His human cock is already the first thing in frame`
- Face landing: finish the mask on the human mouth before the verb
- Torso landing: flat chest and navel before the next body binds

Do not write `human kemonomimi cock`. Do not write `human animal`. One species claim per surface.

A fully human second body does not need `human cock` unless the prior in that take is also kemonomimi.

---

## 10. End-hold and duplicates (v1.1)

Flux commits as it attends. The last clause cannot edit the first.

Hold (the last beat) may only carry:

- `Adult.`
- light, grain, lens, grade

Hold may not carry:

- tail, ears, muzzle, anatomy, sex, species
- `not X`
- a copy of a phrase already used mid-liner

Duplicate rule: if `tail`, `muzzle mask`, or the ear lock appears twice, delete the occurrence farther from the feature descriptor. Keep the one sitting with hair / eyes / ears / tail / mask.

Worked reject:

> … large blue fox tail with a white tip … Gritty photoreal. Adult, animal ears only, one tail, human face under a stylized fake-dog muzzle mask, not an anthro snout.

Worked hold:

> … large blue fox tail with a white tip, blue fake-dog muzzle mask strapped over his human mouth, straps pulled tight … Gritty photoreal, cold street sodium, film grain. Adult.

---

## 11. Override

If a requested prompt, compiler flag, or old habit violates this file, this file wins.
v1.1 does not relax v1. It names failure modes v1 did not have words for.
v1.2 does not relax v1.1. A two-body take that opens on a name or a grip is not a hold.
v1.3 does not relax v1.2. A static take still finishes the landed subject before it binds the place. A wide shot may pan. It may not re-open a finished subject.

---

## 12. State-of-being bind (static / portrait) — v1.3

The bind does not have to be a fight. If no second body is in the take, the bound thing is the place, or the state the finished body is already in.

Sequence stays the same:

1. Land.
2. Finish the body (material, wear, light, state).
3. Bind = spatial or stative verb: stands in, sits at, leans on, is swallowed by, holds the frame.
4. Resolve the place as a surface (wet pavement, neon on the wall, rain on the glass). Not a travel brochure.
5. Do not invent a second body to have something to pin.

Worked hold (solo, no interaction):

> Hip-height in the layover bay. The lean athletic adult Caucasian kemonomimi is already planted there — [finish] — then the diesel haze takes the rest of the frame, dim sodium on wet curb. Adult.

Fail: dumping the room before the body is finished. Fail: adding a phantom hand so the compiler has a "grip."

Beta examples: `STATIC_AND_WIDE.md`

---

## 13. Pan is not re-bind (wide shots) — v1.3

"Never backtrack" means **never re-bind a committed subject**. It does not mean the camera cannot move.

Allowed: land on subject A, finish A, pan to subject B (new, unfinished), finish B. B is a new landing, not a return.

Banned: finish A, pan to B, then add a hat, a tail, or a second cock to A.

In a market / street / wide room:

- First named figure is the landing.
- Background figures are new subjects only if the gaze actually arrives on them. Finish each once.
- Do not inventory the crowd. One extra body, finished, or none.
- Place surfaces (stall canvas, wet asphalt, signage glow) bind after the first body, or after the last body you chose to finish.

Rename in review notes: `backtrack` = `re-bind`. Same fail mode token so old output forms still parse. Use `re-bind` in commentary.
