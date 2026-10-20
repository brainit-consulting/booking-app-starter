# House rules for this project

You're helping a small-business owner build their own booking app. They are not a programmer. These rules are for
Claude Code and Codex alike (CLAUDE.md and AGENTS.md say the same thing).

## How to work

- Talk in plain words, briefly. No jargon without a one-line explanation.
- Before you change anything, say in two or three lines what you'll change and why.
- One small change at a time. Touch only the files the task needs.
- Never delete files, folders or data without asking first and saying exactly what would be lost.
- Don't say "done" until you've checked it: `npm run build` passes and you've looked at the page in the browser.
  Say what you checked.
- If something fails twice, stop. Explain what went wrong in plain words and suggest what to try, instead of a third
  guess.
- If the request is unclear, ask one question rather than guessing.
- To stop a program you started (such as a test server), stop only that one, by its port or process number. Never
  stop all Node programs at once (no `taskkill /IM node.exe`, no `Stop-Process -Name node`): other apps on this
  computer, including the Claude app itself, use Node too.

## The project

- What the app does: `docs/spec.md`. How it looks: `DESIGN.md`. Follow both; ask before changing either.
- Next.js (App Router) with Tailwind CSS, TypeScript. Pages live in `app/`.
- The owner works on Windows; commands run in PowerShell. On Windows, run npm as `npm.cmd` (for example
  `npm.cmd install`, `npm.cmd run dev`): Windows often blocks the `npm` script PowerShell would otherwise use.
- Keys and passwords never go in the code. They go in `.env.local`, which is never saved to Git or sent anywhere.
- Don't add new packages without saying why and asking first.

## Saving work

- Make a Git commit (a "save point") only when the owner's prompt asks for one, with a short, clear message saying
  what changed.
- Push to GitHub only when the prompt says so.
