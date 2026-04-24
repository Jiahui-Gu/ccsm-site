# ccsm-site

Product site for [Claude Code Session Manager (ccsm)](https://github.com/Jiahui-Gu/Agentory-next) — a desktop GUI for Claude Code that organizes work by task instead of repo.

Single static `index.html`, Tailwind via CDN, no build step.

## Local preview

Open `index.html` in a browser, or:

```bash
python -m http.server 8000
```

## Deploy (Cloudflare Pages)

```bash
npm install -g wrangler
wrangler login            # opens browser
wrangler pages deploy . --project-name=ccsm
```

The Cloudflare project is `ccsm`; the assigned subdomain is `https://ccsm-1io.pages.dev` (the bare `ccsm.pages.dev` was taken).

## License

MIT.
