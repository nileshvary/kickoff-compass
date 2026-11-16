# Use Kickoff Compass in any AI chat app

Chat apps like ChatGPT, Gemini, Claude.ai, Microsoft Copilot, Mistral Le Chat and others can't load skill folders.
Instead, use the paste-in version: [`kickoff-compass-prompt.md`](kickoff-compass-prompt.md) (about 3,400
characters).

App menus change often, so the steps below describe where to look rather than exact button names.

## Option A: one-off (works everywhere, free plans included)
1. Open `kickoff-compass-prompt.md` and copy everything.
2. Start a new chat, paste it, and on the next lines describe your idea.
3. Answer the questions (`1A, 2C`, or just `OK`).

## Option B: save it once, reuse forever (recommended)
Paste the prompt into the app's "instructions" box for a reusable assistant:

| App | Where to paste it |
|---|---|
| ChatGPT | Create a custom GPT (Explore GPTs → Create → Configure → **Instructions**), or a **Project**'s instructions |
| Gemini | Create a **Gem** (Gems → New Gem → **Instructions**) |
| Claude.ai | Create a **Project** and paste it into the project **instructions** |
| Microsoft Copilot, Le Chat, others | Any "custom instructions", "agent" or "assistant" setting that accepts a system prompt |
| Your own app or API | Use it as the **system prompt** |

Name it "Kickoff Compass", then start each new idea by describing it.

## Picking up where you left off
Chat apps can't save files, so every reply ends with a **"Progress so far"** block.
- Copy that block somewhere safe (a note, an email to yourself).
- Days later, start a new chat with the same assistant and paste the block: *"back again! here's where we were: …"*.
- It continues from the next step without asking anything you already answered.

Some apps also have their own memory or project history; the block still works if those don't.

## Coding agents (they can save progress automatically)
Tools that support the open **Agent Skills** format (`SKILL.md`) can use the full skill, with automatic progress
saving. See the main [README](../README.md#start-here).
