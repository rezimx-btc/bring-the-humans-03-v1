# SUBMIT HANDOFF — bring-the-humans-03 v1

## Video

- File: `ad.mp4` (repo root — this is the file to post to TikTok)
- Specs (verified with ffprobe): **1080×1920, H.264, 60 fps, 22.5 s, 4,260,764 bytes,
  1 video stream, no audio stream**, bitrate ~1.51 Mbps
- Structure: 0–3 s hook "AI WORKS. YOU GET PAID." · 3–9 s what make.fun is
  ("AI AGENTS COMPETE FOR REAL MONEY — ON make.fun") · 9–17 s three beats
  (1 BUILD AN AGENT / 2 ENTER A BOUNTY / 3 WIN USDC) · 17–20 s CTA "JOIN THE RACE"
  + make.fun/bounty/bring-the-humans-03 · 20–22.5 s official referral end card
  with code `nht78ayn`
- Frame checks (viewed): t=0.1 badge visible from first frame (magenta flash) ·
  t=1.5 hook crisp over hero art · t=6.0 WHAT scene readable · t=11.0 beat 1 clean ·
  t=18.5 CTA + URL readable · t=22.4 end card perfect, code `nht78ayn` in the
  white field, caret covered, copy button clear
- `main.ts` verified: 2 runs (`MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts`)
  produce byte-identical output, sha256
  `e46011b92820a9e852ede78f3fb450dc05050534fdf562a4b16c30b701c9c708`

## How the video was REALLY made (honest)

1. **Muse Image** (`media.generate_image`, worked): 2 hero frames, both verified
   1152×2048 with PIL and viewed — (a) three ghost robots racing to a golden
   trophy, (b) one ghost robot lifting the trophy. Prompts were detailed
   (§4: subject + environment + lighting + low-angle camera + composition with
   empty upper third + magenta/ink/white/gold palette, no text).
2. **Muse Video was attempted and FAILED**: `media.generate_video` returned 403
   "Video generation is not available for this account in its country or region.
   This is a lasting restriction, not an outage: retrying will not help."
   Per that error I did NOT retry. 0 video clips used, 0 of the 6-clip quota spent.
   Note: the capability report's "Muse Video operational" rested on docs + catalog
   presence with no live test — the live test now proves it unavailable here.
3. **ffmpeg 8.1.2 assembly** (the motion): zoompan push-ins on both stills,
   kinetic DejaVu Sans Bold typography, alternating magenta/ink/white scenes,
   press-pack ghost mark in the WHAT scene, badge overlay as-is at 0,0 from frame 1,
   official llms.txt end-card recipe (HOLD=2.5 over the held last frame, blur
   sigma 28 + saturation 0.35 easing 0.8 s, code in JetBrains Mono Bold 62 px
   ink #191419 from x210 centre y1271, caret covered white 9×82 at x208 y1230).
4. **No audio**: no TTS/music tool exists in this session (espeak/piper absent),
   and Muse Video's synthesized sound was unavailable with it — the ad is
   text-driven and silent. No voiceover is claimed.
5. **Not used / not claimed**: Sora, Runway, Kling, Veo, Pika, Luma, Midjourney,
   FLUX, Stable Diffusion, Krea, Canva — none connected. Nothing copied or
   re-uploaded; the video is original and made in this session.

## Event facts used (verbatim from the brief)

- Play code 0: `makefun-granite-pear-frisbee` (backups:
  `makefun-backpack-fiesta-melody`, `makefun-spatula-cottage-dolphin`,
  `makefun-melon-mallard-thermos`) — goes in the caption or bio
- Referral code: `nht78ayn` — https://make.fun/r/nht78ayn (on the end card)
- TikTok account: @maysalo1 · Solana wallet: `DubZE7Ad22aZkwFFEAxqG6dobffrU82GN2ymzdrRY8Vm`
- Brand: magenta #c41c83, ink #191419, white #ffffff; name lowercase `make.fun`

## What the coordinator / Uzan still must do (NOT done by me)

- **Post `ad.mp4` to TikTok** from @maysalo1 (public, Everyone) — I did not post it.
- Caption (paste as it stands):
  `Made by my AI agent for a $500 bounty on make.fun, where AI agents compete for real money: make.fun/bounty/bring-the-humans-03`
  plus the play code `makefun-granite-pear-frisbee` plus referral link
  https://make.fun/r/nht78ayn. (Caption NOT made in the video — parent prepares it.)
- After posting, replace the PLACEHOLDER in `VIDEO.json` with the real
  `https://www.tiktok.com/@maysalo1/video/<id>` URL, then submit.
- Deadline: 24 Nov 19:00 UTC. Top 20 by views share $500.

## Repo contents

- `ad.mp4` — the ad (22.5 s, 1080×1920, 4,260,764 bytes)
- `main.ts` — Node 22 stdlib-only, copies VIDEO.json to the output dir
- `VIDEO.json` — `{"url": "https://www.tiktok.com/@maysalo1/video/PLACEHOLDER"}` —
  **PLACEHOLDER, must be replaced with the real TikTok URL after Uzan posts**
- `README.md` — badges (3 make.fun markdown images) + video + how to post
- `LICENSE` — MIT, line 1 `SPDX-License-Identifier: MIT`
- `.makefun/owner.json` — `{"wallet": "DubZE7Ad22aZkwFFEAxqG6dobffrU82GN2ymzdrRY8Vm"}`
- `SUBMIT-HANDOFF.md` — this file

## Limitations (honest)

- 60 fps, not 30 fps: the official end-card recipe sets fps=60 (the card itself
  is 60 fps native). TikTok accepts 60 fps; no visual downside observed.
- No motion-video clips: Muse Video is region-blocked for this account, so all
  motion is ffmpeg zoompan/kinetic type over two AI stills — the ad is a
  motion-graphics piece, not AI video footage.
- No sound: silent by necessity (no TTS/music tool in session, no usable
  synthesized audio). TikTok viewers can add trending audio in-app when posting
  if Uzan wants sound — that edit would be his, outside this build.
- The ghost robots in the AI frames are original illustrations in the brand
  palette, not the press-pack mascot; the real press-pack mark appears in the
  WHAT scene and in the badge/end card.
