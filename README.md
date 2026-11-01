# Obineer

**From vibe coding to agentic engineering.**

Obineer is a Windows app for building software with AI agents – with method instead of luck. It runs several [Claude Code](https://docs.claude.com/en/docs/claude-code/overview) agents across your projects, each guided by a *Brain*: the knowledge and ways of working you build up yourself, so every task starts from what you have already learned.

This repository holds Obineer's installers and release notes. It has no source code.

**[Download the latest version →](../../releases/latest)**

## What it does

- **Every project on one map.** Each project has its own agent, with a name, a robot and a card that says what it does, what it needs from you and what comes next.
- **A Brain behind every agent.** Skills and knowledge files the agent reads before it works – the method, your stack, your rules. Brain Health shows what a Brain covers, what it lacks for your kind of project and what to fix first.
- **A board per project.** Goals, groups and cards the agent plans with you and works through; nothing is written to the board without your approval.
- **You stay in charge.** Approvals for what an agent may run, a branch guard, and a project view that says what happened since you were last there.
- **Calm by design.** Agents work quietly; only what needs you asks for you.

## Install (Windows)

1. Download `Obineer-Setup-<version>.exe` from the newest [release](../../releases/latest).
2. Run it. The installer is not signed yet, so Windows SmartScreen warns the first time: choose **More info → Run anyway**.
3. Obineer opens in its own window. You need Claude Code installed and logged in – Obineer checks on first start and offers its login. Obineer never sees your login.

Prefer not to install? Take `Obineer-<version>-portable.zip`, unzip it anywhere and run `Obineer.exe`.

**Needs:** Windows 10 or 11 (64-bit) and a Claude Code account. Obineer ships its own Node; nothing else to install.

## Updates

Install a newer version over the old one; your projects, settings and Brains stay. After an update Obineer shows what is new, once. The full history is in [CHANGELOG.md](CHANGELOG.md) and in *Settings › About* in the app.

## Your data

Everything stays on your machine. Obineer has no account, no cloud service and collects nothing.

- Settings and run history: `%APPDATA%\Obineer\data`
- Brains you make: `Documents\Obineer\Brains`
- Each project's plan: a `.obineer/` folder inside the project, plain Markdown you can read and commit

Uninstalling removes the program, never your data, your Brains or your projects.

## The name

*Obby* was its maker's nickname for years; Obineer is Obby the engineer – and the engineer in every agent it runs.

## Status

Obineer is young: it works and is used every day, but expect changes between versions. Questions and bugs: open an [issue](../../issues). The licence is not decided yet; until then no open licence applies.
