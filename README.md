# ProjectHiLL

![Status](https://img.shields.io/badge/status-alpha-orange)
![Language](https://img.shields.io/badge/language-Rust-000000)
![License](https://img.shields.io/badge/license-MIT-blue)

Hill is a programmable workspace operating system for developers.

It isn't another window manager—it's a runtime for intelligent workspaces.

Hill treats a project as something you can enter, restore, and operate, instead of something you manually rebuild every time you switch context.

## Overview

- Project-centric workspace runtime
- Local-first and event-driven
- Built for restoring development context across terminals, services, and workspace state

## What you can do
 
- Register and manage projects
- Restore project context from a single command
- Observe workspace events through a structured event bus
- Extend the system through adapters and plugins

## Architecture

```mermaid
flowchart TD
  A[Users / Tools] --> B[CLI / Shell]
  B --> C[Hill Runtime]
  C --> D[Event Bus]
  C --> E[State Store]
  C --> F[Adapters]
  D --> G[Rules]
  E --> H[Project Data]
  F --> I[Desktop / Services / Workspace]
  G --> J[Actions]
  J --> I
```

Hill is designed as a runtime, not a one-off utility:

- Requests enter through the CLI or shell.
- The runtime coordinates state and events.
- Adapters bridge external systems.
- Rules transform events into workspace actions.



## Repository layout

```text
hill/
  crates/
    hill-runtime/
    hill-cli/
    hill-shell/
    hill-config/
    hill-types/
```


## Screenshots

<img width="1254" height="1254" alt="call_uaEB6E2yEi7FTSMbU2fkkyPJ" src="https://github.com/user-attachments/assets/cd26866a-f796-4fe2-9dfe-d962c60eab34" />


## Status

Hill is under active development.


## Releases

- `v0.1.0-alpha`
- `v0.2.0-alpha`
- `v0.3.0-alpha`


