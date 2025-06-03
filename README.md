# Action-Repo

This repository contains the GitHub Actions workflow configuration to simulate webhook events for testing the webhook server.

## Features

- Includes `.github/workflows/main.yml` which triggers on `push` events or can be manually triggered.
- Sends dummy webhook event payloads to your webhook server URL (configure this URL in the workflow file).

## Usage

1. Clone the repository:

   ```bash
   git clone <your-action-repo-url>
   cd action-repo
Edit .github/workflows/main.yml to update the webhook URL to your public ngrok URL or deployed server URL.
    ```
### Commit and push your changes:

```bash
Copy
git add .github/workflows/main.yml
git commit -m "Update webhook URL"
git push origin <branch-name>
This push will trigger the GitHub Actions workflow that sends a test webhook event to your server.
```
### Workflow Details
The workflow triggers on push events to any branch.

It sends a POST request to your configured webhook endpoint with dummy event data for testing.

### Author
## Tejas Koli
