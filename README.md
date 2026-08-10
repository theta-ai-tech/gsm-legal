# gsm-legal

Public legal pages for the GameSetMatch (GSM) app, served via GitHub Pages.

- `/terms/` — Terms of Service
- `/privacy/` — Privacy Policy

**This repo is public on purpose** — these documents are linked from the App
Store listing and the app's sign-in screen, and App Store review requires them
to be publicly reachable. See `ops/decisions/` in the `gsm` workspace repo for
the record.

When the `gamesetmatch.app` domain is purchased (long-lead item L7), attach it
as a custom domain in this repo's Pages settings — the content moves without a
migration. Until then the canonical URLs are:

- https://theta-ai-tech.github.io/gsm-legal/terms/
- https://theta-ai-tech.github.io/gsm-legal/privacy/

The iOS app reads these URLs from `gsm/gsm/Core/Config/LegalLinks.swift`; the
same URLs go in App Store Connect (App Privacy → Privacy Policy URL). If a URL
here ever changes, update both.

Plain static HTML, no build step. Edit, commit, push — Pages redeploys.
