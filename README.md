# Render keep-alive ping

This repository contains a GitHub Actions workflow that requests the deployed dashboard every 10 minutes:

`https://dq-react-dashboard.onrender.com/overview`

## Set it up

1. Commit and push this repository to GitHub.
2. In the repository, open **Actions** and enable workflows if GitHub prompts you.
3. Run **Keep Render service warm** once with **Run workflow** to confirm it works. Later runs happen on the schedule.

GitHub scheduled workflows are best effort and can be delayed, so this cannot guarantee that the service is always awake. Render's free services may also be restarted or suspended for other reasons. For reliably avoiding idle spin-down, use a paid Render instance. Render documents the free service behavior at https://render.com/docs/free.
