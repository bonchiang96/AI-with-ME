# Install AI with ME

This guide explains how to install the AI with ME Plugin as a Private Plugin from this Repository.
The [README](README.md) explains the Framework.

## 1. Plugin location

The Plugin resides in the [plugin](plugin/) folder. It contains:

1. [plugin.json](plugin/plugin.json): the Agent Plugins manifest.
2. [.claude-plugin/plugin.json](plugin/.claude-plugin/plugin.json): the Claude plugin manifest.
3. [skills](plugin/skills/): the Agent Skills.
4. [rules](plugin/rules/): the Global Writing Rules and the Global Communication Rules.
5. [templates](plugin/templates/): the standard file templates with their Operating Guides.

## 2. Install with an AI

Give your AI the Repository URL. The AI completes these steps:

1. Read the README.
2. Locate the Plugin and this guide.
3. Assess dependencies in its actual environment.
4. Assist installation with its available tools and granted permissions.

Use your host's own mechanism to create, install and update the Private Plugin.
Exact packaging and update methods are pending design.

## 3. Dependencies

The Plugin needs Google Drive and Google Docs access at run time.
The Plugin does not ship these connectors. Your host's integrations select the connector.

Missing dependencies do not block installation.
At each Conversation start, the system-entry skill checks the connectors.
It explains any missing connector, capability or permission and discusses the next authorized step.

## 4. After installation

Start a Conversation and enter the System through the system-entry skill.
It locates the Google Drive folder named “AI with me”.
When that folder is confirmed absent, it starts Bootstrap.

## 5. Updates

Update the installed Plugin intentionally from this Repository.
The installed Plugin runs normal work without routine GitHub reads.
