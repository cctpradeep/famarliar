# famarliar.com

The live website for [Famarliar](https://www.famarliar.com), a marriage, family
and life counselling practice in Bangalore.

## How publishing works

Cloudflare Workers Builds publishes this repository to the Worker
`young-leaf-c6a4`.

- **`main` is the live site.** Anything merged into `main` goes live within a
  minute or two.
- **Every other branch gets a preview link.** Cloudflare posts it as a comment
  on the pull request. Nothing on a branch is live.

Changes arrive as pull requests. Open the preview link, check the pages the pull
request lists, and merge to publish. To reject a change, close the pull request.

## What's in here

- `public/`: the complete site exactly as visitors receive it. A deploy
  replaces the whole site with this folder, so it always holds every page,
  never a partial set.
- `wrangler.jsonc`: the Cloudflare configuration.

The pages are generated elsewhere and copied in whole on every change. Editing
files in `public/` by hand here won't last; the next change overwrites them.
