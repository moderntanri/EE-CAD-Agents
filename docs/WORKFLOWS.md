# Workflow overview

EE-CAD-Agents is focused on existing electrical CAD projects rather than drawings generated without project context.

## Inspect

Identify the selected work area, relevant layers, device symbols, existing routes and drawing units. Distinguish existing completed work from locations requiring a change.

## Plan

Preserve circuit identity and the project's routing conventions. Group equivalent operations where practical. Flag ambiguous device connections instead of guessing their destination.

## Apply

Work on a copy. Make scoped geometry changes and preserve unrelated objects. Socket loops, coordinated dimensions and annotation are current development use cases.

## Validate

Review the saved result for connectivity, spacing, unwanted intersections and changes outside the intended area. Reopen the output drawing and report unresolved exceptions.

## Scope and limits

DWG is the target exchange format. Compatibility depends on drawing version, entity types and third-party data. The prototype is not certified for every CAD application or project. Automated checks support engineering review; they do not replace responsibility for electrical design.
