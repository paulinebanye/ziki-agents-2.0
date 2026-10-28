# Ziki Agent Studio

An interactive, frontend-only redesign concept for the **Ziki Agents** workspace. It explores a friendlier way to discover, create, and manage AI agents through role-specific 3D robot characters, clearer agent cards, and conversational introductions.

> **Prototype only:** This project is not affiliated with or connected to a live Ziki workspace. Agent records, API keys, and management actions are simulated in the browser. Do not use the generated keys as credentials.

## Preview

Open `index.html` in a modern browser. No installation, development server, or build step is required.

## Features

- **Agent roster:** Responsive two-column desktop layout with character artwork, role descriptions, search, and role filtering.
- **Seven agent roles:** Observer, Contributor, Triager, Reviewer, Dispatcher, Merger, and Admin Merger.
- **Meet an agent:** Open a compact introduction dialog with the agent's role, capabilities, and suggested starting actions.
- **Suggested actions:** Choose a role-specific action and see a handoff-ready confirmation. No actual work is dispatched.
- **Create an agent:** Enter a name, optional model, project, and starting role. The *Your New Teammate* panel updates as the role changes.
- **Agent management:** Simulated key copying, regeneration, revocation, deletion, and role/project changes.
- **Team directory:** Expand team members to view compact lists of their agents.
- **Custom dropdowns:** Styled role and project selectors with keyboard support.
- **Character artwork:** Seven embedded 3D robot illustrations, so the standalone HTML can be viewed offline.

## Getting started

1. Download or clone this repository.
2. Open `index.html` in Chrome, Safari, Firefox, or Edge.
3. Try **Meet [agent name]**, select a suggested action, and explore the **Create agent** and **Team** sections.

If the repository contains the distributed standalone file under another name (for example, `Ziki-Agent-Studio-v14.html`), rename it to `index.html` before following these steps.

## Suggested repository structure

```text
ziki-agent-studio/
├── index.html       # Standalone prototype (HTML, CSS, JS, embedded artwork)
└── README.md        # Project documentation
```

## What is simulated?

This is a design/interaction prototype rather than a production client:

- The initial agents and team members are sample data.
- Registration, role changes, project changes, key operations, and deletion affect the current page session only. Refreshing the page resets the data.
- The displayed API keys are mock values and are **not** valid authentication credentials.
- Suggested agent actions do not connect to a model, ticket tracker, repository, or backend.
- Navigation and documentation links may be illustrative rather than fully implemented.

## Design approach

The interface retains Ziki's blue-and-white visual identity while presenting agents as recognizable collaborators. The 3D characters are used in the roster, creation preview, and introduction dialog; the Team directory uses compact rows to avoid overwhelming the page.

## Accessibility and responsiveness

The prototype includes keyboard-operable dropdowns and a dismissible agent dialog. The agent roster adapts to smaller screens. This is not a claim of full accessibility compliance; additional testing is recommended before production use.

## Future improvements

- Connect the UI to real agent and project APIs.
- Replace sample data and mock keys with authenticated workspace data.
- Persist changes and show backend errors and loading states.
- Add automated browser tests for dropdowns, dialogs, registration, and responsive layouts.
- Perform a complete accessibility audit.

## Running locally with a server (optional)

A local server is **not required**, but you can use one if you prefer:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## License

No license is included by default. Add a `LICENSE` file after deciding how you want others to use or contribute to this prototype. Ziki branding and any third-party assets remain subject to their respective owners' rights.
