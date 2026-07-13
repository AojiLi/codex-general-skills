# Repository Explainer Guide

Read this reference only when the HTML explains an existing software repository or a specific subsystem inside one.

## Orient Efficiently

Inspect in this order:

1. Repository instructions such as `AGENTS.md` and local equivalents.
2. Root `README`, package manifest, build configuration, and top-level directory tree.
3. Runtime or application entry points.
4. Files directly involved in the requested feature, flow, or subsystem.
5. Tests, schemas, or documentation that clarify behavior or ownership.

Use `rg` and `rg --files` to trace names, imports, routes, events, and data types. Stop reading once the visual explanation can be supported with concrete evidence. Do not inventory the whole repository when the user asks about one path.

## Select The Story

Match the visualization to the question:

- System architecture: layered module map with boundaries and ownership.
- Request lifecycle: sequence from entry point through handlers, services, storage, and response.
- Data flow: pipeline showing transforms, schemas, persistence, and consumers.
- State behavior: state machine with events, guards, and effects.
- Build or deployment: ordered stages with inputs, generated artifacts, and destinations.
- Feature walkthrough: user action mapped to UI, domain logic, API, and data changes.

Choose one. Do not combine architecture, sequence, and dependency graphs into one unreadable diagram.

## Evidence Rules

- Use exact file paths, exported names, routes, commands, schemas, and functions.
- Distinguish verified behavior from inference.
- Do not invent missing services or simplify boundaries in a way that changes ownership.
- Link or display the most useful source paths near the visual element they support.
- Prefer a representative trace over a complete dependency graph.
- Keep the primary view to roughly 6-12 nodes. Collapse low-value details into named groups.

## Page Structure

Use this compact narrative when it fits:

1. What the subsystem does.
2. The main architecture or flow diagram.
3. One concrete path through the system.
4. Key files and what each owns.
5. Important constraints, extension points, or failure boundaries.

Avoid dumping the repository tree or long source snippets. The HTML should explain how the code fits together, not reproduce the codebase.
