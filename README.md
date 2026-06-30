# claude-jump

A tiny redirect page used by the **Morning Brief** tool. It exists only so that an
`https://` link (clickable in Gmail and other email clients, which strip custom-scheme
links) can hand off to the `claudejump://` URL-scheme handler that reopens a specific
Claude Code session in the desktop app.

`/?t=<session title>` → redirects to `claudejump://open?title=<session title>`.

No data is stored or sent anywhere; the page just bounces the browser to the local handler.
