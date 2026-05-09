# GitHub Weekly Summary Workflow (n8n + Claude)

This workflow automatically fetches GitHub activity (commits, issues, PRs) for the week and uses Claude AI to generate a narrative summary, delivered via Discord.

## Setup Instructions (5 Steps)

1. **Import:** Download `workflow.json` from this PR and import it into your n8n instance (Settings > Import from File).
2. **GitHub Credentials:** Create a "GitHub OAuth2" or "GitHub Personal Access Token" credential in n8n and select it in the **GitHub Fetch Data** node.
3. **Claude Credentials:** Create an "Anthropic API" credential with your API key and select it in the **Claude Sonnet AI** node.
4. **Configure Variables:** Open the **Config** node (the second node) and replace the placeholder with your **Discord Webhook URL** and the target **GitHub Repo**.
5. **Activate:** Click **Execute Workflow** to test. Once verified, flip the switch to **Active** to enable the weekly schedule (Fridays at 5:00 PM).

## Features
- **narrative Summary:** Uses Claude 3.5 Sonnet to turn raw stats into a readable story.
- **Multilingual:** Supports EN/FR (configurable in the Config node).
- **Discord Integration:** Ready-to-use narrative delivery.
