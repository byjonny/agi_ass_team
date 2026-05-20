# AGI-AS(S)_TEAM

AGI-AS(S)_TEAM is a persistent multi-agent personal assistant system. It runs teams of agents that can coordinate through direct messages, team chat rooms, scheduled heartbeats, shared memory, and messaging channels like Telegram, WhatsApp, and Discord.

## What It Does

- Keeps agents running in persistent mode
- Supports teams, direct agent messages, and shared chat rooms
- Connects to Discord, Telegram, and WhatsApp channels
- Tracks agent heartbeats and scheduled work
- Stores long-term memory and per-agent identity files
- Includes TinyOffice, a web UI for agents, teams, tasks, and conversations

## Quick Start

1. Install dependencies:

   ```bash
   npm install
   ```

2. Build the workspace:

   ```bash
   npm run build
   ```

3. Start TinyAGI:

   ```bash
   npm start
   ```

## Useful Commands

```bash
npm run dev        # run core, teams, server, and main in dev mode
npm run server     # start the API/server package
npm run visualize  # open the visualizer
npm run chatroom   # open the chat room viewer
npm run discord    # run the Discord channel
npm run telegram   # run the Telegram channel
npm run whatsapp   # run the WhatsApp channel
```

## Key Files

- `AGENTS.md` describes agent behavior, team messaging, memory, and file exchange.
- `docs/` contains deeper setup and architecture notes.
- `packages/` contains the core runtime, teams, channels, server, visualizer, and CLI.
- `tinyoffice/` contains the web interface.

## Notes

- Agents should keep their own workspace `AGENTS.md` updated as their setup evolves.
- Shared files for the human live under `.tinyagi/files/`.
- Channel credentials and runtime settings should be configured outside source control.
