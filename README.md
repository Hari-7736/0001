# CA firm website (static)
Single `index.html`, no build step. Three preview themes: emerald, navy (gold), slate (indigo). Open with `?theme=navy` to pick one.

## Before sharing / going live
1. Find & replace: `Meridian Associates`, `yourfirm.com`, `hello@yourfirm.com`, `+91 00000 00000`, `910000000000` (WhatsApp).
2. Update the address and details in the JSON-LD block in `<head>`.
3. To ship one theme: delete the `#themes` div and the "theme preview switcher" script, then set `data-theme` on `<html>`.
4. Add `og-image.png` (1200x630) and a real founder/team photo.

## Deploy
- **Vercel:** import the repo (framework: Other, no build command), or run `npx vercel`.
- **GitHub Pages:** push to a repo, Settings > Pages > deploy from `main` / root.

## Contact chat box
Opens the visitor's email app with a pre-filled message (no backend). For direct sending, point the form at Formspree/EmailJS.
