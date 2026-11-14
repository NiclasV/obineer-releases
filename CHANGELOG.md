# Changelog

What is new in each version of Obineer, newest first.

## 0.1.10

One door to a sharp Brain, numbers you can trust, and the Brain in 3D.

- **Tell the Brain surgeon what you want in your own words** – "my agent is slow", "I build Lovable apps for small firms" – and it decides whether to tune the Brain, add knowledge, build it for your speciality or start a new one, and says why in plain words. It sees how your latest tasks went with the Brain, tells you the before and after of a change, and how to undo it.
- **A Brain built for a domain spends little from the start**: task sizes in the domain's words, a reading budget for each, and one real task measured before it is called ready.
- **The line under an answer counts that answer** – its steps, stages and tokens. When the conversation has earlier messages, a second line gives the whole conversation, and the warning about too many reads no longer follows every follow-up.
- **Follow-up messages cost less**: a conversation keeps the instructions it started with, so Claude's prompt cache is reused instead of written again.
- **The Brain graph in 3D**: a 2D | 3D switch in the graph's corner shows the same Brain in space. Nodes float gently, sparks run along the links like signals, and you can grab a node and pull it – its neighbours follow and swing back. Drag the space to turn it, scroll to zoom, click a node to open it.
- **The Flow view is gone.** The Brain view is Graph and Cards; stepping a run in the graph and the chat's links into Flow went with it. The route report, the task's size and the gates under an answer stay.

## 0.1.9

Runs that spend tokens in proportion to their task, and a way to see it.

- Agents now **size a task before they read**, and read only what that size needs. Several requests in one prompt are done one at a time, and what a task found is saved in its card before it builds, so an interrupted run continues instead of starting over.
- Every project gets a **code map**, `.obineer/CODEMAP.md`: each code file and what it exports, written from your files before every run. Agents look code up there instead of searching.
- **Right agent, right task**: a scout on a cheap model finds code, a checker runs the build and tests, and chats in *Investigate* or *Review* use Sonnet unless you choose another model (Settings › Agents).
- **Runs start much lighter**: a short tool list takes what every step re-reads from about 39k tokens to about 17k. Claude Code's own skills and PowerShell are left out of runs; switch it off in Settings › Claude Code if a run needs them. Your connectors stay.
- Under a run, the chat shows **the whole run's cost** – steps per stage, new tokens and tokens read again – and warns when finding the way took more than the task's size allows.
- **Health** tells you when a Brain does not send its tasks to the code map, and *Fix* lets the Brain surgeon bring it in line. The board check warns when `PROJECT.md` names a folder that is gone.
- A project's **Experiments** place lists its latest tasks one by one – calls and tokens before the first edit – with *Measure again*. Switch on *Experiment mode* in Settings › Usage to see it.

## 0.1.8

Rules that speak up only when they matter, and a process that fits the task.

- Every task now gets a size: **small**, **normal** or **large**. A small task takes the short way through your Brain: a one-line plan, and the commit as its record. The chat shows the size beside the route report, so the short way is never silent. A risk such as personal data or a release always makes a task at least normal.
- The rules in your Brain that a step rested on now sit as **one closed line under the answer** that cited them, instead of piling up open at the bottom of the chat. Open it to see each rule, why it matters, where it lives, and the way to the flow.
- When a rule **stops or flags** the work, that line opens by itself and says so. Rules that were only checked and held stay folded, marked *Checked, held*. In the flow analysis, a held rule is a green hexagon.
- The editor no longer marks `import … from './X.tsx'` as an error, the way Vite projects write imports.

## 0.1.7

Models by their real names, Fable, and a chat that shows it is working.

- The model list offers **Fable** too: Fable, Opus, Sonnet, Haiku – most capable first.
- Models are named by what they run as: **Opus 5.5**, **Sonnet 5.5**, **Haiku 5.5**. When Claude releases a new model and Claude Code is updated, the new name shows by itself. A model that has not run yet shows its family name until its first run.
- The explanations under *Model* and *Stages* sit behind an **i**: hover or focus it to read them. Map cards, columns and Settings use the same model names.
- While an agent works, the chat's last line starts with three dots that rise in turn. They stand still while it waits for your approval or answer.
- With only one Brain, the project card names it, and the project's details show which Brain it runs with. Before, nothing showed, though the project already used it.
- In the Brain chat, the branch guard looks at the Brain you work in. A Brain inside a project follows the project's branches, and a Brain in a repository of its own is never warned about. Before, it could warn about *master* in another Brain's repository.

## 0.1.6

Work like you do in VS Code – and see why your Brain stops you.

- The chat input works like Claude Code in VS Code: one box with a toolbar – **+** for files, the model, the file open in the editor (sent along as context, **×** leaves it out), the mode with its icon, and send.
- Approvals ask "Allow the agent to use Bash?" with numbered choices: Yes, Yes for this run, Yes for all of the tool, Don't ask again…, or No with a word to the agent. Press 1–5 to choose, Esc to deny.
- Right-click a tab: close it, the others, those to the right, the saved ones or all, or copy its path. Unsaved tabs ask once.
- Code reads like in VS Code: 15 px with roomy lines, bracket pair colours and the scope you are in kept at the top.
- Zoom the app with Ctrl + and Ctrl − (Ctrl 0 resets). The level shows for a moment, the status bar keeps it while it is not 100 %, and the next start opens at it.
- A project's plan and own Brain are found even a few folders down, like `httpdocs/.obineer` – not only at the project's root.
- When a gate in your Brain stops or flags the agent's work, the chat says which rule, why it matters and where it lives, with a link to the flow.
- *Fill the gap* shows how the fill goes, with *Follow it*, and a later run says when it read the new knowledge. The Brain agent's task is titled in your language.
- *Focus* in the status bar: only the project in focus interrupts you; the others keep working and wait in *Waiting for you*.
- Everything that says something waits for you now agrees – the tab title, the status bar, the badges and the list – and failed or quiet agents are listed too, with *Open*.
- If Obineer was rebuilt while it ran, it says so and asks you to restart, instead of new screens talking to an old server.
- New Brains come with a skill for plain answers: the result first, what was really done, no filler.
- A Brain task is shown under the Brain it works in, never another one's name.

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
