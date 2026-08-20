# SITS9

SITS9 (A Stitch in Time Saves Nine) is a minimal domain-specific language with five primitive instructions — FWD, RET, CROSS, TENSION, and ANCHOR — designed to encode temporal processes in music, textile, and cuisine. This repository contains a prototype implementation and demonstrative renderers.

## Reproducing the figures

Install dependencies:

```bash
pip install -r requirements.txt
```

Generate the Pachelbel Canon schematic figures:

```bash
python3 create_pachelbel_schemas.py
```

Generate the national-anthem demonstrations and Deck statistics:

```bash
python3 demo_anthems.py
```

Both scripts produce PNG/SVG/MIDI/JSON outputs in `output/`.

## Repository layout

- `core.py` — SITS9 `Deck`, `Card`, and primitive instruction definitions.
- `renderer_svg.py`, `renderer_midi.py`, `renderer_cooking.py` — domain renderers.
- `demo_pachelbel.py` — Pachelbel Canon cross-domain demo.
- `create_pachelbel_schemas.py` — generates Figure 2–4 schema diagrams.
- `demo_anthems.py` — encodes four national anthems as SITS9 Decks and renders them.
- `output/` — generated figures, anthems, and Deck JSONs.
