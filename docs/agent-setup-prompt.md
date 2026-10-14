Set up Anvil, a HighLevel build toolkit for Claude Code, on this computer. Do as much as you can yourself and ask me only for the things you cannot do.

<context>
Anvil is a Claude Code plugin made of nine skills. It plans HighLevel accounts from call notes and documents, builds them in my own signed-in browser, and reads every write back. I received the Anvil folder from its author; it is not downloaded from anywhere. The folder is its own plugin marketplace, so it installs straight from disk.

The folder carries its own setup guide for agents: `ENTRY_POINT.md` at the top level. Read it first and follow it. Where it and this prompt disagree, the folder's guide is newer and wins.

What Anvil needs:
- Claude Code, logged in.
- A browser Claude can drive: the Claude in Chrome extension is the default; a Playwright browser is the fallback.
- My own HighLevel login. I sign in myself. Anvil never handles passwords.
- Node.js, for Anvil's self-check and planning scripts.
</context>

<steps>
1. Ask me where the Anvil folder is. Confirm it is the right folder by finding `ENTRY_POINT.md` and the plugin manifest inside it. Do not move or edit anything in it.
2. Check what this machine has: operating system, Claude Code version, Node.js version, and whether a browser tool is already connected. Tell me in one short list.
3. Add the folder to Claude Code as a plugin, the way `ENTRY_POINT.md` describes for a folder install, and install the plugin from it.
4. Connect the browser. If the Claude in Chrome extension is missing, tell me to install it and wait. If I manage several client accounts, explain that each client can have its own browser profile so logins never mix, and ask whether I want that now.
5. Ask me to open HighLevel in that browser and sign in to the sub-account I want to use. Wait until I say I am in. Never type, read, store or screenshot a password.
6. Run Anvil's self-check. Fix anything it flags that you can fix; for the rest, show me its suggested fix and wait.
7. Do one read-only test: ask Anvil to list the custom fields of the sub-account I am signed in to. Confirm the sub-account name with me before and after.
8. Report: what you installed, what the self-check said, what the test returned, and anything still open.
</steps>

<rules>
- Read only. During setup, do not create, change or delete anything in HighLevel.
- Do not change Claude Code's permission mode or any settings outside what the plugin install needs. If Anvil's guide suggests a permission mode, tell me what it does and let me decide.
- If a step fails twice, stop and tell me what you saw instead of trying other routes.
</rules>
