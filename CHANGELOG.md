# Changelog

What is new in each version of Obineer, newest first.

## 0.1.5

Fewer interruptions, and everything that waits for you in one place.

- *Waiting for you* in the rail gathers every agent that waits for an approval or an answer, from every project, then the boards' open questions and waiting cards. One click answers.
- *Tools* in the rail shows everything your agents can use – MCP servers, skills, subagents, commands, hooks, plugins and the programs on your computer – how often each is used, and what looks wrong.
- When Claude Code updates itself, Obineer checks that it still has everything Obineer uses, and says plainly what is missing if not.
- Obineer now remembers your theme, language, layout and the release notes you have read between starts.
- A new permission mode, Auto: Claude Code runs routine work, commands too, and asks only for what it judges risky. Choose it for one message or as the default in Settings.
- The approval card has *All Bash this run*: one click, and the rest of the run's shell commands run without asking. Nothing is saved.
- After a restart, a run that was cut off no longer shows an approval you cannot answer. It says it was interrupted, with Run again.
- The project manager on a card mentions the board's questions calmly – "when you have time" – and a click opens the board's Inbox where they are.

## 0.1.4

Brains and approvals, clearer.

- Building a Brain for a domain opens the Brain agent's chat on it, so its questions and approvals are in front of you instead of waiting unseen.
- Each project card shows which Brain its agent follows; click it to choose another.
- The Brain agent stays in the Brain view – never a card on the Workspace – and the Brain button in the rail tells when it works or waits for you.
- Settings › Claude Code shows each Brain's saved approvals too, the approval card says where a rule is saved, and a web fetch can be allowed for every site at once.

## 0.1.3

One title bar, as in VS Code and Discord.

- Windows' own title bar is gone: its buttons sit in Obineer's bar, in the theme's colours, and follow when you change theme.
- Obineer's mark sits beside the name, in the colour of the text – light on a dark theme, dark on a light one.
- The search box is in the middle of the window, and the bar's buttons, icons and the window's own buttons line up.

## 0.1.2

Projects from anywhere, a face of its own, and themes that reach the code.

**Projects**

- The first start opens straight away – no folder to choose first.
- The project list's *Add* has three ways in: *New project* (a name and a place – the folder is made and opens, ready to plan), *Add project* (one folder), and *Add a folder of projects* (every subfolder becomes a project; the folders are listed under the projects, to remove again).
- The installer no longer asks where to install: Obineer goes in your own programs folder, so it never needs admin rights.

**Looks**

- Obineer has its own icon – in the taskbar, the Start menu and the installer.
- Atom One Dark is the default colour theme. Six more: Dracula, GitHub Dark and Light, Tokyo Night, Catppuccin Mocha and Latte – all readable to WCAG 2.2 AA.
- Code in the editor takes the theme's own colours, and in TypeScript and JavaScript functions, variables, parameters, properties and types are told apart, as in VS Code.
- Your own theme reaches the code: *Settings › Appearance › Your own › Code* sets the colour of each kind of code.

## 0.1.1

Agentic is now **Obineer** – Obby the engineer. Your settings, run history and Brains come along on the first start.

**The new name**

- The app, the installer and the window say Obineer. Install it, then uninstall the old *Agentic*: Windows sees them as two programs. Your data stays and moves over by itself.
- A project's plan now lives in `.obineer/`; a project planned before moves there by itself the next time Obineer starts.

**Projects**

- Back in a project, its view shows what happened since your last visit – the tasks that ended, the commits, and what waits for you on the board or in the chat.
- A project folder you remove, rename or add on disk shows up at once. A removed one leaves the rail, and opening it says the folder is gone, with *Remove from Obineer*.
- Settings › Agents has *Model for planning*: the kickoff, board mode and ideas planned in can run on a cheaper model, since they read the board, not the code.

**Brains**

- Each skill and knowledge file says which area it serves – UX, architecture, delivery and so on – and the Brain view's cards show it as a small label; searching the cards finds by area too.
- Setting up a Brain asks what it will mostly build – a website, a web app, a SaaS and so on – and Health then shows the areas that kind of project needs and the Brain still lacks.
- Health is easier to read: the score, one line on what it means and what to fix first – the rest one click away. *Generality* is now *Portable*: whether a Brain is general or specialized is a label, not a grade.
- When Health shows a missing area, the Brain agent has something to fill it with: the library now covers UI, data, legal, docs and launch too.

## 0.1.0

The first version you install. Obineer runs several Claude Code agents across your projects, each guided by a Brain you build.

**A program of its own**

- Obineer installs like any Windows program and opens in its own window – no terminal, no browser, no Node of your own needed. Uninstalling never touches your projects, your data or your Brains.
- On first start it checks that Claude Code is installed and logged in, and its own login is one click away. Obineer never sees your login.
- Add any folder on the machine as a project with the system's folder picker.
- Closing Obineer stops every agent and site first, so nothing keeps running behind your back.
- Only Obineer's own window can talk to its agents – no other program or web page on your machine can.
- After an update Obineer shows what is new, once; Settings › About has the version and every version's notes.

**Cards that say what to do next**

- A free agent's card offers the project's next step from its own board: plan the project, continue or run the next card, or review what the last task changed.
- *Give a task* always lands you where you write.
- The project manager – the voice of the board – appears with its own name only while it plans, or when the board has questions for you.
- The cards keep only what guides you; MCP servers and the Brain picker live in the project's details.

**Brains**

- A new Brain starts lean – the method and what every change needs. Security, debugging and other know-how come when setup's answers or your work ask for them.
- What the Brain agent adds to a Brain is wired in at once, and Health warns when something is added that no route reaches.
- A first start without a Brain says there is nothing to check yet, instead of an error.
- Obineer's own helper agents step aside when they have nothing to do.

Known: the installer is not signed yet, so Windows SmartScreen warns the first time – choose *More info → Run anyway*.
