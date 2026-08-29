# 1000 Bot URL Viewer

Open `index.html` in a modern browser.

This version intentionally separates:
- **1000 virtual bots**: simulated entirely in JavaScript for the dashboard.
- **Real previews**: a small configurable number of iframes.

A browser is not a practical place to launch 1000 independent real browser sessions.
For authorized load testing of infrastructure you control, use a backend load-testing
system (for example, Playwright workers, k6, or a similar tool) and feed aggregate
metrics into this dashboard.

Some sites also prevent iframe embedding with CSP/X-Frame-Options, so a preview may
remain blank even when the URL itself works.
