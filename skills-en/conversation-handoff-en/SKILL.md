---
name: conversation-handoff-en
description: Creates a handoff summary of the current conversation so work can continue in a new chat. Use when the user says "handoff", "wrap up", "summarize for a new chat", or when a long task needs to move to a new chat. Outputs 8 fixed sections.
---

# Conversation Handoff

Long chats cost more credits, but a new chat loses context. This Skill compresses the conversation into a summary that a new chat can pick up immediately.

## Rules
1. Use the exact format below. Do not rename or add sections.
2. Output only the summary. No greetings, intro, or closing remarks.
3. Keep it short. Compress; do not copy the conversation.
4. Never invent information. If something is missing, write `(not in conversation)`.
5. Put code only in [Key code], and only essential snippets.
6. End with exactly: `Paste this into a new chat to continue.`

## Format
```
[Project goal]
[Languages / tools]
[File structure and role of each file]
[Done]
[Remaining tasks] (in priority order)
[Current errors or issues]
[My rules and style]
[Key code] (essential snippets only)

Paste this into a new chat to continue.
```
