# Action-Repo

This repository contains the GitHub Actions workflow configuration to simulate webhook events for testing the webhook server.

## Features

- Contains `.github/workflows/main.yml` which triggers a dummy event on `push` or manually.
- Sends payloads to your webhook server URL (configure this in the workflow).

## Usage

1. Clone the repository:

   ```bash
   git clone <your-action-repo-url>
   cd action-repo
2. Edit .github/workflows/main.yml to update the webhook URL to your ngrok or live server URL.

3. Commit and push changes to trigger the workflow.
   

## Workflow Details
Triggers on push events.
Sends a POST request to your webhook endpoint with dummy event data.
make sure the locally the app.py is working
# Author
## Tejas Koli
