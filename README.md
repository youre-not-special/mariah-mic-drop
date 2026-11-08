# Mariah Mic Drop

A voice-led AI workroom skill: think out loud, explain deeply, keep real work moving and keep its results visible.

Created: 2026-11-07 · Thread: 01a1b887-308b-7c71-9714-6f6aeddd8553

Copy the `mariah-mic-drop` folder into the skill directory your host actually discovers. Invoke Mariah or voice mode. A one-off request to be brief does not activate it. Read `SKILL.md` for the workflow and `references/voice-workroom.md` for capability limits.

The package includes no microphone or speech engine, dashboard server, background scheduler or companion bridge. It uses the tools your host offers, verifies updates and gives an honest fallback when a capability is missing. Personal configuration can live in a private `local/` folder; none is distributed here.

## Check and use

Validate the package with an Agent Skills validator or your host’s skill validator, then test one real trigger and one near miss in that host. The author’s bounded text checks do not establish live audio quality or acceptance by a new user.

## License

MIT. No third-party source code or skill text is bundled. The reference page links original documentation.
