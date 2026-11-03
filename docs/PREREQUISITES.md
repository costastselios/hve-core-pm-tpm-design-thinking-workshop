# Prerequisites
- VS Code with GitHub Copilot Chat.
- The GitHub Copilot app or GitHub Copilot CLI, to install HVE Core.
- The HVE Core plugin, installed as described in [Install HVE Core](#install-hve-core).
- Agents visible: **DT Coach**, **BRD Builder**, **PRD Builder**.

## Install HVE Core
HVE Core is distributed as a plugin: a Git repository of reusable skills and related components, including the agents this workshop uses. Install the `hve-core` plugin from the `microsoft/hve-core` marketplace source once, using either option below; it's then available in GitHub Copilot, VS Code, and Copilot CLI.

- **GitHub Copilot app:** [add the marketplace](https://docs.github.com/en/copilot/how-tos/github-copilot-app/customize-github-copilot-app#adding-a-plugin-marketplace), then [install the plugin](https://docs.github.com/en/copilot/how-tos/github-copilot-app/customize-github-copilot-app#install-a-plugin).
- **Copilot CLI:** follow HVE Core's [Copilot CLI Plugin guide](https://microsoft.github.io/hve-core/docs/getting-started/methods/cli-plugins).

Don't also install HVE Core from VS Code's plugin menu or the VS Code Marketplace. Either can add a VS Code-only copy that duplicates agents and skills.

The plugin tracks `main` and receives ongoing updates. Use your client's refresh option, or see [Update an Installed Plugin](https://microsoft.github.io/hve-core/docs/getting-started/methods/cli-plugins#update-an-installed-plugin). Version pinning isn't available yet; future tagged releases will add it, and stable-release updates will be posted in the HVE Core working group channel. Because `main` changes often, repeat the readiness check before each session.

## Agents and skills
| Agent | Workshop steps | Skills it loads |
|---|---|---|
| **DT Coach** | 1–6 | Design Thinking skills, such as `dt-coaching-foundation` and `dt-methods` |
| **BRD Builder** | 7 | `requirements-author` |
| **PRD Builder** | 8–9 | `requirements-author` |

Skills come with the plugin, and each agent loads its skills automatically. You only select agents.

## Readiness
- [ ] HVE Core plugin installed, with no duplicate agents in the picker
- [ ] DT Coach
- [ ] BRD Builder
- [ ] PRD Builder

Check the agent picker in VS Code Copilot Chat. In Copilot CLI, run `/agent` and look for `hve-core:dt-coach`, `hve-core:brd-builder`, and `hve-core:prd-builder`.

## Providing files to Copilot
Use the file-context mechanism available in your VS Code Copilot Chat: for example **Add Context**, the workspace file picker/reference syntax, or drag-and-drop when supported. Verify the intended file appears in chat context before sending the prompt.

If an agent is missing, or reports that it can't load a skill, stop rather than substituting another agent. Install or update the plugin as described above, or use your organization's HVE setup process. Then run **Developer: Reload Window** in VS Code and repeat this check.

## Next
[Workshop Map →](WORKSHOP-MAP.md)
