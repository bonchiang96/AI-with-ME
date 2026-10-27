# Install AI with ME

## 1. Select the package

1. Use this repository as the source for your Private Plugin.
2. Select the branch or commit you intend to install.
3. Obtain the complete [plugin directory](plugin/), including its hidden `.claude-plugin` directory.
4. Keep the package intact. Its rules, templates and supporting references belong with its nine Skills.

The package root is `plugin/`, not the repository root.
It contains the Agent Plugins 1.0 `plugin.json` and the Claude `.claude-plugin/plugin.json`.
Both manifests use the same Skills and supporting resources.

## 2. Install with an AI

1. Give your AI this repository URL and the chosen branch or commit.
2. Ask it to read the README, locate this guide and assess the actual environment's installation capabilities.
3. Let it assist private installation through the host's supported mechanism and granted permissions.
4. If it cannot install directly, let it explain the limitation and guide the permitted next step.
5. Verify that the host discovers the nine Skills in the installed package.

Google Drive and Google Docs connectors are runtime dependencies.
They are not included in the package and do not block installation.
Their manifest declarations are descriptive metadata, not automatic connector installation or enforcement.
The `system-entry` Skill checks available connectors and explains missing access when the Plugin runs.

Use the host's current installation guidance for its exact setup steps.
This package does not require public directory publication.

## 3. Update manually

1. Select the intended newer repository branch or commit.
2. Obtain its complete `plugin/` directory.
3. Ask your AI to apply the host's supported private Plugin update method within granted permissions.
4. Verify that the installed package contains the intended updated files and all nine Skills.

Intentional updates use GitHub source. Installation and updates do not modify your Google governance or records.
