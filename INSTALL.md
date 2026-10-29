# Install AI with ME

This guide explains how to install the AI with ME Plugin as a Private Plugin from this Repository.
The [README](README.md) explains the Framework.

## 1. Plugin package

The Plugin root is the [plugin](plugin/) folder, not the Repository root.
The whole plugin folder installs together. Keep it intact, including the hidden `.claude-plugin` folder.
The folder contains:

1. [plugin.json](plugin/plugin.json): the Agent Plugins manifest.
2. [.claude-plugin/plugin.json](plugin/.claude-plugin/plugin.json): the Claude plugin manifest.
3. [skills](plugin/skills/): the nine Agent Skills.
4. [rules](plugin/rules/): the Global Writing Rules and the Global Communication Rules.
5. [templates](plugin/templates/): the standard file templates with their Operating Guides.
6. [LICENSE](plugin/LICENSE): the MIT License.

Both manifests describe the same Skills. The Skills share the rules and templates folders.

The Repository root also holds two marketplace files:

1. [.claude-plugin/marketplace.json](.claude-plugin/marketplace.json): the Claude marketplace.
2. [.agents/plugins/marketplace.json](.agents/plugins/marketplace.json): the Codex marketplace.

Both marketplace files point to the plugin folder.

## 2. Install with an AI

Give your AI the Repository URL and the commit you choose. The AI completes these steps:

1. Read the README.
2. Locate the plugin folder and this guide.
3. Assess dependencies in its actual environment.
4. Install the whole plugin folder through the host's own Private Plugin mechanism, within granted permissions.
5. Verify that the host lists all nine Skills.

When the AI cannot install the Plugin itself, it explains the limitation and guides the permitted next step.

The nine Skills are:

1. ai-with-me, the System entry.
2. meeting-agent.
3. execution-agent.
4. inbox.
5. knowledge-base.
6. workflow-book.
7. workflow-business-document.
8. workflow-qa.
9. profit-a.

## 3. Install on each host

This guide covers the command-line hosts.
For Claude chat, the Claude desktop app, Cowork and ChatGPT, follow the [README](README.md#installation).

Claude Code CLI uses the root `.claude-plugin/marketplace.json`:

1. Run `/plugin marketplace add bonchiang96/AI-with-ME`.
2. Run `/plugin install ai-with-me@ai-with-me`.

Codex CLI uses the root `.agents/plugins/marketplace.json`:

1. Run `codex plugin marketplace add bonchiang96/AI-with-ME`.
2. Install the ai-with-me plugin from the added marketplace.

The Codex CLI installs the Plugin in that environment, not in a ChatGPT account.

## 4. Dependencies

The Plugin needs Google Drive and Google Docs access at run time.
The Plugin does not ship these connectors. Your host's integrations select the connector.
Each Skill declares this need in its compatibility line.

Missing Google access never blocks installation.
At each Conversation start, the ai-with-me Skill checks actual access.
It explains any missing connector, capability or permission and discusses the next authorized step.

## 5. After installation

Start a Conversation and enter the System through the ai-with-me Skill. In Claude, type `/ai-with-me`.
It locates the Google Drive folder named “AI with me”.
When that folder is confirmed absent, it starts Bootstrap.

## 6. Updates

An update reinstalls the whole plugin folder from a chosen commit of this Repository.
Verify again that the host lists all nine Skills.
Installation and updates never change your Google records or governance resources.
The installed Plugin runs normal work without routine GitHub reads.
