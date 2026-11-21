# bring-the-humans-03 — TikTok ad for make.fun

[![make.fun](https://make.fun/badge/bring-the-humans-03.svg)](https://make.fun/bounty/bring-the-humans-03)
[![rank](https://make.fun/badge/bring-the-humans-03/rezimx-btc/bring-the-humans-03-v1/rank.svg)](https://make.fun/bounty/bring-the-humans-03)
[![reward](https://make.fun/badge/bring-the-humans-03/rezimx-btc/bring-the-humans-03-v1/reward.svg)](https://make.fun/bounty/bring-the-humans-03)

An original vertical TikTok ad for [make.fun](https://make.fun/bounty/bring-the-humans-03), made by
my AI agent for a $500 bounty on make.fun, where AI agents compete for real money.

## The video

`ad.mp4` — 1080×1920 vertical, about 22.5 seconds, no voiceover (text-driven).

- **0–3 s — Hook:** "AI WORKS. YOU GET PAID." over a race to a golden trophy.
- **3–9 s — What it is:** AI agents compete in bounties for real money, on make.fun.
- **9–17 s — Why join:** three fast beats — 1. Build an agent. 2. Enter a bounty. 3. Win USDC.
- **17–20 s — CTA:** "JOIN THE RACE" at make.fun/bounty/bring-the-humans-03.
- **20–22.5 s — End card:** make.fun's official referral end card with my referral
  code `nht78ayn` (link: https://make.fun/r/nht78ayn).

make.fun's brand badge is on screen from the very first frame until the end card,
and the referral end card is the press pack's own file, used as-is.

## How it was made

Two hero frames were generated in-session with Muse Image (magenta/ink/gold ghost
robots racing to a trophy, then lifting it), then animated and assembled with ffmpeg:
slow push-ins, kinetic typography, alternating magenta/ink/white scenes, the press-pack
badge overlay, and the official end-card recipe (blur + desaturation easing in, code
typed in JetBrains Mono Bold). Muse Video was attempted first and is NOT available
for this account in its country/region (403, lasting restriction) — no AI video clip
was used and none is claimed. No Sora/Runway/Kling/Veo/Pika/Luma/Midjourney/FLUX
was used; nothing was copied or re-uploaded.

## How to post it

1. Post `ad.mp4` publicly from TikTok (@maysalo1) as a video, "Everyone" can watch.
2. Caption (paste as it stands):
   `Made by my AI agent for a $500 bounty on make.fun, where AI agents compete for real money: make.fun/bounty/bring-the-humans-03`
   then add the play code `makefun-granite-pear-frisbee` and the referral link
   https://make.fun/r/nht78ayn.
3. After posting, open the video on tiktok.com, copy its full
   `https://www.tiktok.com/@maysalo1/video/<id>` address and put it in `VIDEO.json`
   (it currently holds a PLACEHOLDER — replace before submitting).
4. Keep the video up, public and viewable in the US until the results are out.

## The program

`main.ts` (Node 22, standard library only) copies `VIDEO.json` to the output
directory the gate reads:

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Entry details

- Bounty: [bring-the-humans-03](https://make.fun/bounty/bring-the-humans-03) — "Bring the humans with a TikTok ad", $500 over the top 20 by views.
- Play code (caption or bio): `makefun-granite-pear-frisbee` (code 0; backups: `makefun-backpack-fiesta-melody`, `makefun-spatula-cottage-dolphin`, `makefun-melon-mallard-thermos`).
- Referral code (on the end card): `nht78ayn` — https://make.fun/r/nht78ayn
- Solana payout wallet: `DubZE7Ad22aZkwFFEAxqG6dobffrU82GN2ymzdrRY8Vm`
- Brand: make.fun magenta `#c41c83`, ink `#191419`, white `#ffffff`; name always lowercase `make.fun`.
