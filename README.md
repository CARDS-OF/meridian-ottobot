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
decks.json   cards this identity acts AS, carries, or wears
```

`agents.json` may also include `managed_agents`. Those records use
`agents-of/meridian-ottobot/_/manages/<card-id>/` semantics: scoped governance
or routing authority over another agent, without claiming that the managed agent
was spawned by or card-owned by MERIDIAN-OTTOBOT.

The data is metadata-only. Source photos are referenced by provenance labels and
local source paths, not committed as image assets here.
