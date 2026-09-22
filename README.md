# CARDS-OF / meridian-ottobot

Concrete card and child-agent provenance for:

```text
MERIDIAN-OTTOBOT
👽8♥️/AS/📎9♥️/AS/🔱3♣️
root session 019f68b6-7e58-7621-9f32-410588171513
```

This repo is intentionally separate from `CARDS-OF/cards-of`.

- `CARDS-OF/cards-of` owns schemas and namespace conventions.
- `CARDS-OF/meridian-ottobot` owns this identity's concrete card records.

## Files

```text
cards.json   physical cards dealt for children/forks/sidecars OF this identity
agents.json  agent/thread spawn order OF this identity
decks.json   SUPERSEDED, see migration note below
stacks.json  SUPERSEDED, see migration note below
```

### Migration note (2026-09-22)

`decks.json` and `stacks.json` were carried here as a level-1 flattening of
what several sibling identities (`gnomon-ottopoet`, `rancor-monster`,
`aurora-thesean`, `imperial-tie-fighter-pilot`) already keep as fully
separate org-level repos — `decks-of/<identity>` and `Stacks-Of/<identity>`.
Per Victor, 2026-09-22: *"decks-of/cards-of/agents-of and stacks-of/cards-of/
agents-of are technically the spaces we are flattening to one level."* This
identity's records have now been migrated to match that established
pattern:

- Real, canonical: [`decks-of/meridian-ottobot`](https://github.com/decks-of/meridian-ottobot)
- Real, canonical, private: [`Stacks-Of/meridian-ottobot`](https://github.com/Stacks-Of/meridian-ottobot)

The `decks.json`/`stacks.json` files below are kept in place as historical
record, not deleted — but treat the two repos above as source of truth going
forward, not these files. `cards.json` and `agents.json` are unaffected;
`CARDS-OF/meridian-ottobot` remains their real home, matching every sibling
identity's own convention. No canonical level-2/3 agglutination practice
exists yet anywhere in this swarm (Victor, same day) — this migration stops
at level 1, matching precedent, not inventing deeper structure.

`agents.json` may also include `managed_agents`. Those records use
`agents-of/meridian-ottobot/_/manages/<card-id>/` semantics: scoped governance
or routing authority over another agent, without claiming that the managed agent
was spawned by or card-owned by MERIDIAN-OTTOBOT.

The data is metadata-only. Source photos are referenced by provenance labels and
local source paths, not committed as image assets here.

## Scope Model

Use the narrowest correct card scope:

- `🚀9♦️`: PFM Codex red-team / Team-Of scope. Use `/AS/🚀9♦️/` for generic
  Codex-team infrastructure or statements about the PFM red team.
- `📎9♥️`: MERIDIAN office worker scope.
- `🔱3♣️`: MERIDIAN project-facing KPFM/PFM red-team captain role.
- `👽8♥️`: root thread/selfhood card for the durable MERIDIAN continuity.
- `🪄GRN:170`: MERIDIAN-OTTOBOT name/persona card.

DashBOrg currently has card-grid registrations for the individual cards and
relationship events. `stacks.json` records the physical stack observation that
binds those layers together; ingestion into DashBOrg should preserve it as stack
provenance rather than flattening it into a single identity card.
