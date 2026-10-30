# Kovalam Homestay

Website for [kovalamhomestay.in](http://kovalamhomestay.in).

A static site served by a Cloudflare Worker (`kovalamhomestay-in`). Everything in
`public/` is published as-is; configuration lives in `wrangler.jsonc`.

## Commands

No install step is needed — `npx` fetches Wrangler on demand.

```sh
npx wrangler login              # sign in to Cloudflare (once per machine)
npx wrangler dev                # preview locally at http://localhost:8787
npx wrangler deploy             # deploy manually
npx wrangler deployments list   # see recent deployments
npx wrangler rollback           # revert to the previous deployment
npx wrangler tail               # stream live request logs
```

## Deploying

Pushes to `main` deploy automatically via Cloudflare Workers Builds.
