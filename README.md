# Learn about any subject with your Letta AI agent using Anki flashcards and n8n

...

## Pre-requisites

...

### What you'll need

- **Anki** downloaded and installed on your computer: https://apps.ankiweb.net/
- **n8n** v1.0.0+ (Cloud or self-hosted).
- **Letta** account (Cloud or self-hosted) and an **API token**.
- A **Letta Agent ID** (e.g., `agent-90009dba-8012-46c5-a0f5-5630cc457363`).
<details>
<summary>
(Click to expand) How to create a Letta agent and get its ID
</summary>

#### To create a Letta agent:

![letta create new agent](./screenshots/letta_create-new-agent.jpg)

#### And get its ID from the agent's page:

![letta dashboard agent id](./screenshots/letta_dashboard-agent-id.jpg)
</details>

### Install the Letta community node

#### Option A — from the n8n UI (recommended)

1. In n8n, go to **Settings → Community Nodes → Install**.
2. Enter `@letta-ai/n8n-nodes-letta` and confirm.

#### Option B — npm / Docker

- In the n8n root directory:

```bash
npm install @letta-ai/n8n-nodes-letta
```

- If you run n8n with Docker, add to your `.env` **before** `N8N_CUSTOM_EXTENSIONS`, like this:

```
N8N_CUSTOM_EXTENSIONS=@letta-ai/n8n-nodes-letta
```

Then rebuild/restart n8n.

### Create Letta credentials in n8n

1. Open the **Credentials** screen → **New** → choose **Letta API**.

![n8n new credentials](./screenshots/n8n_new-cred.jpg)

2. Fill in:

- **API Token**: your Letta token (from the Letta dashboard).
- **Base URL**: `https://api.letta.com` (or your self-hosted URL).

![n8n letta credentials](./screenshots/n8n_letta-cred.jpg)

> Where to get the token: Letta dashboard → API settings → generate token.

## Implement the n8n workflow

...

## Known Issues and Limitations

...

## Resources

1. https://github.com/letta-ai/n8n-nodes-letta

## Author(s)

- [J. Ramon A. Bendiburg](https://github.com/jraleman) [@raisga](https://raisga.com/)
