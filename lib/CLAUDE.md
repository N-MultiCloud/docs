# docs/lib — Documentation Generator Helpers

Up: [`../CLAUDE.md`](../CLAUDE.md) · [`../../CLAUDE.md`](../../CLAUDE.md)

---

Python helpers used by the `collect_*.py` generators.

| File / Path | Role |
|---|---|
| [`__init__.py`](./__init__.py) | Package init. |
| [`phply/`](./phply/) | Vendored PHP parser — used to scan
  [`../../core/src/opnsense/mvc/app/controllers/`](../../core/src/opnsense/mvc/app/controllers/)
  for `*Action()` methods and emit canonical API endpoint docs. |
| [`utils.py`](./utils.py) | Shared helpers. |

## Working Rules

- Read-only vendor source.
- Generators driven by these helpers run **before** Sphinx — output lands
  as `.rst` fragments under [`../source/`](../source/).
