# NCEMS Field Reference Hub

Central landing page for North Country EMS crew and admin tools.

## Links

- Live (hub): [https://ncemsderek.github.io/apps/](https://ncemsderek.github.io/apps/)
- Live (admin): [https://ncemsderek.github.io/apps/admin.html](https://ncemsderek.github.io/apps/admin.html)
- Repo: [https://github.com/ncemsderek/apps](https://github.com/ncemsderek/apps)
- Upload: [https://github.com/ncemsderek/apps/upload/main](https://github.com/ncemsderek/apps/upload/main)

## Files

- `index.html` — crew-facing hub (clinical reference + app cards + notice banner)
- `admin.html` — BC/Chief login to push notices live to the hub
- `README.md` — this file

## Adding more apps

Open `index.html`, find a section (`Clinical Reference`, `Operations`, etc.) and copy a card block. The grid handles layout automatically.

## Firebase setup (notices)

1. Paste your Firebase config into both `index.html` and `admin.html`
2. Set `FIREBASE_READY = true` in both files
3. Change `ADMIN_PASSWORD` in `admin.html` to something real before deploying

## Admin password

Default is `ncems2026` — **change this before deploying** in `admin.html`.

## Changelog

### v1.2
- Full hub rebuild — clinical reference first, apparatus last
- iPad/iOS primary layout, 2-column grid, big tap targets
- Admin notice banner pinned to bottom (never blocks content)
- `admin.html` — BC/Chief login, push/clear notices, urgent flag (amber)
- Firebase listener wired and ready — just needs config + `FIREBASE_READY = true`
- Seven clinical cards as Coming Soon placeholders
- WAMBOchecker full-width at bottom with fleet units listed

### v1.1
- Config-driven APPS list; added NCEMS OT as fifth card

### v1.0
- First build. Four app cards, forest green branding, mobile-first.

## Notes

- Hosted in `apps` repo so it sits at `/apps/` — never touches the root URL
- iOS home-screen caches hard — delete and re-add icon after every deploy
- Admin page is at `/apps/admin.html` — share only with BCs and chiefs
