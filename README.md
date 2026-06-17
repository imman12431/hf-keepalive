# hf-keepalive

GitHub Actions cron job that pings a Hugging Face Space every 10 minutes to prevent the free-tier container from sleeping.

## Setup

1. Add a repository secret named `HF_SPACE_URL` with your HF Space URL as the value (e.g. `https://your-username-your-space-name.hf.space`). No trailing slash.
   - Go to: Settings → Secrets and variables → Actions → New repository secret

2. Push this repo to GitHub — the workflow will start running automatically on schedule.

3. To test immediately: Actions tab → "Keep HF Space Alive" → "Run workflow".
