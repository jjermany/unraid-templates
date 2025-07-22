# Plex Notifier

Plex Notifier periodically checks for new Plex episodes and sends user-specific email alerts based on watch history, powered by Tautulli.

## Features

- Scheduled polling for new Plex episodes
- Tautulli integration to match user watch history
- HTML email with show and episode artwork
- Web-based UI for configuration
- Simple setup: fill in form fields and go!

## Setup (Unraid)

1. Install via Unraid Community Apps using the template
2. Set these container settings:
   - `/mnt/cache/appdata/plex-notifier` → `/app/instance`
   - `TZ` (e.g., `America/Chicago`)
   - Network: `host`
3. Go to the Web UI
4. Enter:
   - Plex URL + token
   - Tautulli URL + API key
   - SMTP info for sending email
   - Poll interval in minutes
5. Click "Save Settings"

## Notes

- No episode notifications will be sent unless the user has a viewing history for the show.
- Poster fallback and email formatting handled gracefully.
- Easily test email settings from the UI.

🔗 GitHub: [https://github.com/jjermany/plex-notifier](https://github.com/jjermany/plex-notifier)
