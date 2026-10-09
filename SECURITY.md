# Security Policy

## Reporting a vulnerability

Please **do not** open a public issue for security problems. Use GitHub's private
reporting instead: **Security -> Report a vulnerability** on this repository
(<https://github.com/Syed-Muhammad-Tayyab/wargames-ai-simulator/security/advisories/new>).

## Things worth knowing

- Every game spends the AI provider key in your `.env`. The API server binds to
  `127.0.0.1` by default and rejects requests from foreign origins; set `HOST=0.0.0.0`
  only if you deliberately want to expose it on your network.
- Never commit `.env` (it is in `.gitignore`) or paste an API key into an issue.
