# docs/source/development — Developer Documentation

Up: [`../CLAUDE.md`](../CLAUDE.md) · [`../../../CLAUDE.md`](../../../CLAUDE.md)

---

Developer-facing documentation for OPNsense core, plugins, and the REST API.
**The single most useful folder** when reasoning about how to write code
against OPNsense.

## Subtree

| Path | Topic |
|---|---|
| [`api/`](./api/) | Auto-generated REST API reference per module (controllers under [`../../../core/src/opnsense/mvc/app/controllers/OPNsense/`](../../../core/src/opnsense/mvc/app/controllers/OPNsense/)). |
| [`api.rst`](./api.rst) | Introductory page for the API. |
| [`architecture.rst`](./architecture.rst) | High-level architecture (Phalcon, configd, models). |
| [`backend/`](./backend/) | Backend (PHP/Python/shell) developer guide. |
| [`backend.rst`](./backend.rst) | Backend overview. |
| [`components/`](./components/) | Reusable UI components (Bootgrid, Tabulator, forms). |
| [`components.rst`](./components.rst) | Components overview. |
| [`examples/`](./examples/) | End-to-end plugin development examples. |
| [`examples.rst`](./examples.rst) | Examples overview. |
| [`frontend/`](./frontend/) | Frontend developer guide. |
| [`frontend.rst`](./frontend.rst) | Frontend overview. |
| [`guidelines/`](./guidelines/) | Style guidelines (PHP, JS, RST). |
| [`guidelines.rst`](./guidelines.rst) | Guidelines overview. |
| [`how-tos/`](./how-tos/) | Recipe-style developer how-tos. |
| [`howtos.rst`](./howtos.rst) | How-tos overview. |
| [`images/`](./images/) | Diagrams used in developer docs. |
| [`workflow.rst`](./workflow.rst) | Contribution workflow. |

## Working Rules

- Read-only vendor source.
- The `api/` subtree is **regenerated** by
  [`../../../collect_api_endpoints.py`](../../../collect_api_endpoints.py)
  — when upstream merges controller changes, this content updates
  automatically.
