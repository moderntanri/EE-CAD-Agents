# EE-CAD-Agents · Engineering overview

[Project home](README.md) · [Workflows](docs/WORKFLOWS.md) · [Status](docs/STATUS.md)

## The problem

Electrical drafting combines visible geometry with information about devices, circuits and drawing conventions. A batch operation needs to preserve that context while changing the selected area. Geometric proximity alone cannot explain every connection.

## Design choices

| Decision | Why it matters |
| --- | --- |
| Start with an explicit selection | The task has a bounded work area and known targets |
| Inspect the existing drawing | Layers, symbols, routes and units influence the operation |
| Keep planning separate from applying | A candidate can be reviewed before it changes geometry |
| Preserve unrelated objects | Completing one task should not silently rewrite the surrounding drawing |
| Save a separate result and reopen it | The delivered artifact can be inspected beyond the original session |
| Report exceptions | Unresolved connections remain visible instead of being guessed |

## Development areas

Drawing inspection, repeatable drafting, circuit editing, coordinated dimensions and annotation are the current areas described in this public overview. They have different geometry and validation requirements; a successful example in one area does not establish universal coverage.

## Read further

- [Workflow overview](docs/WORKFLOWS.md) follows inspect, plan, apply and validate.
- [Development status](docs/STATUS.md) lists the work still required before a public release.
- [Engineering notes](https://github.com/moderntanri/moderntanri/tree/main/notes) explain geometry, operation state and AI tool boundaries through separate synthetic examples.

This repository contains public product documentation. The implementation and private engineering material are not included, and no public installer is available yet.
