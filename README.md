# Circuit Solver

A web-based circuit analysis tool for students — built for textbook problems that don't come with answers or worked solutions. Solves symbolic circuit problems using nodal analysis, mesh analysis, and dependent sources.
![beta run](sg_gif.gif)
Designed around how students actually sketch circuits on paper: draw lines first, then place components on them, with everything happening directly on the canvas (no sidebar, no drag-and-drop component palette).

> **⚠️ Status: work in progress, incomplete.** Currently at Phase 2 (component placement) of the build roadmap below. The solver backend (nodal/mesh analysis, symbolic math) is not yet implemented.

## Scope (current)

Resistive circuits only (DC, symbolic). Capacitors and inductors are excluded for now but the architecture is meant to support adding them later without a rewrite.

## Files

- `circuit-tool-phase2.html` — the tool itself (single-file HTML/CSS/JS). Open directly in a browser.
- `circuit_tool_spec.md` — full design spec: canvas/grid behavior, keyboard shortcuts, variable system, analysis methods, visual design, and the build roadmap.

## Build Roadmap

1. **Canvas & Drawing** — grid, line drawing, snap behavior, erase, undo/redo
2. **Components** *(current phase)* — keyboard placement on lines, symbol rendering, value/name editing
3. **Variable System** — region selection, variable pool, dependent source linking
4. **Solver Integration** — netlist extraction, MNA equation generation, Sympy solve
5. **Mesh Analysis** — loop current placement, KVL equations, unified solver
6. **Polish** — error messages, edge cases, UI refinement

See `circuit_tool_spec.md` for full details.
