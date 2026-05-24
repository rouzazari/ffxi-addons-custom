# CLAUDE.md

## Project Overview

This repository contains modified versions of existing [Windower](https://www.windower.net/) addons for Final Fantasy XI. The goal is to extend or customize addon behavior beyond the upstream originals.

## Contributor

- **rouzazari** (sole contributor)

## Workflow

- Each addon lives in its own subdirectory (e.g., `itemizer/`).
- Addons are forked from upstream Windower addon commits. The upstream source commit ID must be recorded in `README.md` when an addon is added.
- Changes are made on the `master` branch and merged to `main` via PR.

## Addons

| Addon | Source Commit |
|-------|--------------|
| itemizer | [697be7dc10b9deaddd1dec87875f2a16ce84c8e0](https://github.com/Windower/Lua/commit/697be7dc10b9deaddd1dec87875f2a16ce84c8e0) |

## Adding a New Addon

1. Copy the upstream addon files into a new subdirectory.
2. Commit with a message referencing the upstream commit ID (see git log for the convention).
3. Add a row to the **Addons** table above and to `README.md`.

## MCP Usage

An MCP (Model Context Protocol) server is connected to assist with information sourcing. Consult it before falling back to web searches or other sources.

## Code Conventions

- Addons are written in Lua following Windower's addon API.
- No comments unless the *why* is non-obvious.
- Do not introduce new dependencies beyond what Windower's standard library provides.
