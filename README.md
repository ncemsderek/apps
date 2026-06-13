# NCEMS Apps

Landing page hub for the North Country EMS field app suite. One home-screen icon that links out to every app.

## Links

- Live: [https://ncemsderek.github.io/apps/](https://ncemsderek.github.io/apps/)
- Repo: [https://github.com/ncemsderek/apps](https://github.com/ncemsderek/apps)
- Upload: [https://github.com/ncemsderek/apps/upload/main](https://github.com/ncemsderek/apps/upload/main)

## Apps linked

- WAMBOchecker — [https://ncemsderek.github.io/WAMBOchecker/](https://ncemsderek.github.io/WAMBOchecker/)
- Intubation Guide — [https://ncemsderek.github.io/Intubation/](https://ncemsderek.github.io/Intubation/)
- On-Duty Incident Report — [https://ncemsderek.github.io/onduty-incident-report/](https://ncemsderek.github.io/onduty-incident-report/)
- Clark County Protocols — [https://ncemsderek.github.io/Protocols/protocol-app.html](https://ncemsderek.github.io/Protocols/protocol-app.html)
- NCEMS OT — [https://ncemsderek.github.io/ncems-ot/](https://ncemsderek.github.io/ncems-ot/)

## Adding more apps

Open `index.html`, find the `APPS` list near the top of the `<script>`, and copy one block:

```js
{
  name: "App Name",
  desc: "Short one-liner",
  icon: "\uD83D\uDE9A",   // any emoji
  url:  "https://ncemsderek.github.io/your-repo/"
}
```

Order in the list = order on the page. No other changes needed.

## Stack

Single-file `index.html` + `logo.png`. No build step. GitHub Pages deploy.

## Changelog

### v1.1
- Cards now render from an `APPS` list at the top of the file — adding an app is one block.
- Added fifth card: NCEMS OT.

### v1.0
- First build. Four app cards, forest green branding, mobile-first, no-cache headers, logo fallback.

## Notes

- Hosted in its own repo (`apps`) so it serves at `/apps/` and never touches the root URL or any other app.
- Drop a `logo.png` in the repo root (reuse the one from WAMBOchecker) or the header just shows the title.
- iOS home-screen app caches hard — delete and re-add the icon after every deploy.
