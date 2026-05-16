# opnsense/docs — Official OPNsense Documentation Source

## Workspace Context

- Up to opnsense subworkspace: [`../CLAUDE.md`](../CLAUDE.md)
- Up to nmulticloud-context: [`../../CLAUDE.md`](../../CLAUDE.md)
- Upstream: https://github.com/opnsense/docs

---

The official OPNsense documentation source — Sphinx + reStructuredText.
Build output is the published site at https://docs.opnsense.org/.

## Stack

- **Format:** reStructuredText (`.rst`).
- **Engine:** Sphinx (see `requirements.txt` and `Makefile`).
- **Custom extensions:** Local Python helpers in [`lib/`](./lib/) — including
  `phply` (PHP parsing) used to derive API endpoint docs straight from the
  [`../core/`](../core/) controllers.
- **Generators:** [`collect_api_endpoints.py`](./collect_api_endpoints.py),
  [`collect_changelogs.py`](./collect_changelogs.py),
  [`collect_plugin_tiers.py`](./collect_plugin_tiers.py),
  [`make_bios.py`](./make_bios.py). These produce `.rst` fragments under
  [`source/`](./source/).

## Layout

| Path | Role |
|---|---|
| [`Makefile`](./Makefile) | Sphinx build / clean / serve targets. |
| [`requirements.txt`](./requirements.txt) | Python dependencies (Sphinx, theme, plugins). |
| [`lib/`](./lib/) | OPNsense-specific Python helpers used during documentation generation. |
| [`source/`](./source/) | All documentation source. |
| [`collect_*.py`](./collect_api_endpoints.py) | Auxiliary documentation generators run before Sphinx. |
| [`make_bios.py`](./make_bios.py) | Hardware-BIOS doc generator. |

## Working Rules

- **Read-only vendor source.** Submit changes upstream at
  `github.com/opnsense/docs`.
- This is the **canonical prose** when API/config behavior is ambiguous —
  check the docs before extracting intent from code in [`../core/`](../core/).
- When [`../core/`](../core/) and these docs disagree, the docs are usually
  authoritative for **intent**; code is authoritative for **current
  behavior**.

## Per-Folder Entrypoints

- [`lib/CLAUDE.md`](./lib/CLAUDE.md)
- [`source/CLAUDE.md`](./source/CLAUDE.md)
