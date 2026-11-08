# Voice workroom mechanisms

Checked: 2026-11-07. These sources explain mechanisms; they do not verify the current user's app or account.

A voice application decides when speech starts and ends, manages playback, and sends conversation items to a model. The skill governs the model's work and conversational choices. Changing prose does not change the application's audio controls.

[OpenAI Realtime conversations](https://developers.openai.com/api/docs/guides/realtime-conversations) describes sessions, conversation items, streaming transcripts and interruption handling. With WebSocket playback the client must stop queued audio and reconcile unheard output; WebRTC and SIP handle server output buffering differently. A delivered transcript does not prove its audio was heard. Use the application's actual events when those are available.

[Voice activity detection](https://developers.openai.com/api/docs/guides/realtime-vad) distinguishes silence-based detection from semantic turn detection. The latter estimates whether the thought ended; it can trade responsiveness for fewer premature turns. This is an application setting, not a promise made by a prompt.

[OpenAI Agents SDK orchestration](https://openai.github.io/openai-agents-python/multi_agent/) describes specialists as tools while a manager keeps the user-facing conversation. Adapt the ownership pattern without requiring the SDK: one owner merges findings, retains accepted choices and finishes the work. Independent review is useful at a concrete gate; adding agents alone does not establish accuracy or save tokens.

[Anthropic's doc-coauthoring source](https://github.com/anthropics/skills/blob/main/skills/doc-coauthoring/SKILL.md) demonstrates an evolving linked artifact and fresh reader testing. Reuse that pattern with questions sized to the actual uncertainty. No source code or skill text is bundled here.

For persistent state, use the host's supported document, artifact or file tools. Keep the selected surface stable, verify writes, and preserve checkpoints outside transient model context. Reconnection, refresh and rendering need their own observed checks. A static file fallback is useful, but it is not an automatic feed.
