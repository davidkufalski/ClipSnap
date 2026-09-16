# ClipSnap iPhone-friendly PWA prototype

## What is included
- Watch → Clip → Make Short → Share workflow
- Twitch / Kick tabs with demo stream discovery cards
- One-tap Clip action
- 15 / 30 / 60-second selector
- Local clip queue using `localStorage`
- Make Short modal with 9:16 preview placeholder
- Caption + title fields
- iOS share-sheet friendly handoff
- Save queue as JSON
- Settings
- PWA manifest + service worker
- Update-friendly hosted architecture

## Important platform note
This prototype does not bypass Twitch/Kick protections and does not silently download other creators' streams. For production use, connect approved platform APIs and/or a compliant hosted capture/transcoding service that is authorized for the content and workflow you support. Direct TikTok / YouTube publishing likewise requires each platform's approved auth/API path.

## Deploy on iPhone with GitHub Pages
1. Create a GitHub repository.
2. Upload the files in this folder to the repository root.
3. In GitHub: Settings → Pages → deploy from the `main` branch root.
4. Open the Pages URL in Safari.
5. Tap Share → Add to Home Screen.

## Update architecture
Keep this app hosted at one stable URL. Future versions can replace the files in the repository; users opening the Home Screen app will receive the updated service-worker cache after refresh.
