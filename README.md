# NCEMS Field Reference Hub

Central landing page for North Country EMS crew and admin tools.

## Links

- Live (hub): [https://ncemsderek.github.io/apps/](https://ncemsderek.github.io/apps/)
- Live (admin): [https://ncemsderek.github.io/apps/admin.html](https://ncemsderek.github.io/apps/admin.html)
- Repo: [https://github.com/ncemsderek/apps](https://github.com/ncemsderek/apps)
- Upload: [https://github.com/ncemsderek/apps/upload/main](https://github.com/ncemsderek/apps/upload/main)

## Files

<<<<<<< HEAD
- `index.html` — crew-facing hub (swipe pages, clinical reference, ops, notice banner)
=======
- `index.html` — crew-facing hub (clinical reference + app cards + notice banner)
>>>>>>> 6d5ffdf88cd1a14bfdb604bc1cc0dbf48dbb67ad
- `admin.html` — BC/Chief login to push notices live to the hub
- `README.md` — this file

## Page layout

<<<<<<< HEAD
**Page 1 (swipe left):** Clinical reference cards (big SF Mono, one per row) + Quick Protocols
**Page 2 (swipe right):** Operations (Incident Report, NCEMS OT) + Apparatus (WAMBOchecker)

## Clinical card order (Page 1)

1. Intubation — live
2. Advanced Airway — coming soon
3. Drip Sets — coming soon
4. Medication List — coming soon
5. Shock — coming soon
6. Sepsis — coming soon
7. Stroke — coming soon
8. Cardiac — coming soon
9. Quick Protocols — live (links to Clark County Protocols app)

## Firebase setup (notices)

1. Paste your Firebase config into both `index.html` and `admin.html`
2. Set `FIREBASE_READY = true` in both files
3. Change `ADMIN_PASSWORD` in `admin.html` before deploying

## Changelog

### v1.3
- Two swipe pages: clinical left, ops/apparatus right
- Page indicator dots below header; tap dots or swipe to switch
- Clinical cards: SF Mono, all-caps, full width, one per row, no confirm on tap
- Quick Protocols as separate section at bottom of page 1
- Coming Soon pills on unbuilt clinical cards
- Back-to-hub button needed on each individual app (handle per-app)

### v1.2
- Full hub rebuild, iPad/iOS primary, admin notice banner
- admin.html with BC/Chief login and Firebase-ready notice push

### v1.1
- Config-driven APPS list; added NCEMS OT

### v1.0
- First build. Four app cards, forest green branding.

## Notes

- Hosted in `apps` repo — never touches root URL
- iOS home-screen caches hard — delete and re-add icon after every deploy
- Admin page at `/apps/admin.html` — share only with BCs and chiefs
- Each individual app (Intubation, WAMBOchecker, etc.) needs its own back button added pointing to `https://ncemsderek.github.io/apps/`
=======
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
>>>>>>> 6d5ffdf88cd1a14bfdb604bc1cc0dbf48dbb67ad
