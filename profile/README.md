## h5i: Next-Gen AI-Aware Git

`h5i` (pronounced *high-five*) is a Git sidecar designed to track the **intent**, **provenance**, and **reasoning** behind AI-assisted development. While Git records *what* changed, `h5i` records *why* and *how* the AI arrived at those changes.

---

### 1. `h5i notes` — Deep AI Observability
This suite analyzes AI agent session logs to visualize the "hidden" work performed during development.

* **Exploration Footprint**: Reveals which files the AI consulted versus which it edited.
* **Uncertainty Heatmap**: Surfaces moments where the AI expressed low confidence.
* **Omission Reporting**: Automatically detects "deferred" tasks, placeholders, and unfulfilled promises in the code.
* **Attention Coverage**: Flags "blind edits", files modified by the AI without being read first in the current session.

### 2. `h5i context` — Reasoning Workspace
A version-controlled reasoning environment that allows AI agents to maintain state and goals across session resets.

* **OTA Trace**: Logs every *Observe–Think–Act* step to preserve the logic used during a task.
* **Milestone Management**: Tracks progress toward a specific project goal with checkpoint commits.
* **Reasoning Branches**: Allows the AI to explore risky alternatives in a separate reasoning thread without losing the main context.

### 3. `h5i commit` — Provenance & Integrity
Enhances traditional commits with AI metadata and automated safety checks.

* **Automatic Provenance**: Records the exact prompt, model, and agent ID used for the change.
* **Design Decisions**: Captures non-obvious implementation choices, including reasons for the final selection.
* **Automated Audit**: Runs security deterministic rules, such as credential leak detection, before a commit is finalized.
