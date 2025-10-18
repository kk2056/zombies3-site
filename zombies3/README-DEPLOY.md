Zombies3 site (ready-to-deploy)
Files:
- index.html  (includes GA ID G-J8GHJM9XN5)
- game.html

Quick steps:
1) Unzip and inspect files.
2) Deploy to Cloudflare Pages or Netlify (upload folder or connect to GitHub).
3) On Cloudflare DNS, point CNAME zombies3 -> <your-pages>.pages.dev
4) Verify in browser (no extensions) and check DevTools Network for g/collect requests.
5) Use DebugView in GA and send debug events (debug_mode: true).

Debug test (browser console):
gtag('event','test_event_manual',{'send_to':'G-J8GHJM9XN5','debug_mode':true});
