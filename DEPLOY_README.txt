
DEPLOY README
=============
Measurement ID used in these files: G-J8GHJM9XN5

Files included:
- zombies3/index.html, zombies3/game.html
- space/index.html, space/game.html

Quick deploy options (Cloudflare Pages):
1) Zip upload (manual):
   - Cloudflare Pages -> Create project -> If available choose 'Deploy site' -> upload the ZIP or drag folder content.
   - Set custom domain to zombies3.promax.it.com and set CNAME in DNS to the pages.dev domain. Make sure Proxy = DNS only (gray cloud).
2) Git method:
   - Push one folder per repo or a monorepo with separate directories, connect Pages, and set build/publish accordingly.

DNS example (Cloudflare):
 - Type: CNAME
 - Name: zombies3
 - Target: <your-pages-subdomain>.pages.dev
 - Proxy status: DNS only (灰色云)

Verify:
 - Use incognito window and browser DevTools -> Network -> filter 'collect' or search measurement_id=G-J8GHJM9XN5
 - Check GA DebugView for incoming events.

Notes:
- cookie_domain is set to 'promax.it.com' so subdomains share client id across your sites.
- If you want only zombies3, upload just the zombies3 folder contents to a Pages project.
