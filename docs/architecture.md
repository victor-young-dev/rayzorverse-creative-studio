# Hybrid production architecture

Android Chrome → mobile studio UI → template/storyboard editor → programmatic rendering (Canvas / future Remotion) + optional AI visuals (hosted provider or ComfyUI) → FFmpeg composition + audio → MP4 export.

## Current implementation
Standalone HTML/CSS/Canvas preview, adjustable text and speed, silent WebM capture in compatible browsers. No backend, no API calls, no embedded AI models.

## Future services
- Remote Remotion renderer for reliable H.264 1080×1920 and audio.
- Optional Wan/LTX/other models via supported hosting; no promise of unlimited free GPU time.
- Voiceover, subtitles and sound mixing with permission-cleared assets.
- Versioned jobs, user uploads, asset licensing metadata, render logs.

## Security
Never expose provider keys in browser JavaScript. Use a server-side secret store and limit generation requests. No paid service is assumed to be free.
