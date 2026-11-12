# Nextext-native-releases

Download and update channel for **NexText Native** (`com.nextext.native`) — the
full NexText experience as a native Android app, from Fred Systems.

NexText Native shares the same Firebase backend as the regular NexText app, so
accounts, chats, groups, contacts, statuses, calls and moderation are fully
interoperable with it. It is a **separate app** from NexText.Lite
(`com.nextext.fig`) — nothing is shared between them except the backend.

## Download

Latest release: **[NexText-v1.2.1.apk](https://github.com/Fred-Systems/Nextext-native-releases/releases/latest)**

1. On your Android phone, open the link above.
2. Download `NexText-v1.2.1.apk`.
3. Tap it and allow "install unknown apps" if asked.
4. Open NexText and sign in with your regular NexText account.

Requires Android 7.0+ (minSdk 24). Signed with the NexText Native release key
(SHA-1 `FA:CF:CA:F6:67:14:E3:F9:CD:FA:C7:8C:33:07:98:30:2E:CE:A0:AF`).
Updating over an earlier install keeps your data — same certificate.

## What's included

Chat (text, images, **videos**, voice notes, polls, files, location, weather),
group chats, **voice and video calls** (WebRTC, with video PiP), **status**
(contacts and public, text/photo/video/voice, 24 h expiry, full editors and
sticker support), **Jewish Statuses** (JewishStatus & YidStatus feeds inside
the Status tab, Jewhub-style podcast player with date picking), the **Video
Library** (YouTube and Dailymotion, off by default), **NexText AI** (hundreds of
personas with their own voices, translation, Whisper transcription and
voice-to-text, image analysis and generation, summaries, voice replies, AI
podcast generator), **voice cloning** (Fish Audio), and native-only **Calculator
and Notes disguises**.

Full details and the privacy posture are in
[`Fred-Systems/Nextext-native`](https://github.com/Fred-Systems/Nextext-native)
(`README.md`).

## How admins see this app's users

Native clients tag their accounts (`clientVariant: "native"`, `nativeUser: true`,
`nativeOnline`, `nativeAppVersion`, `nativeLastSeen`) so the admin dashboard can
list and moderate Native users separately from NexText.Lite and regular NexText
accounts. See `ADMIN_PROMPT.md` in that repository.

## Updates

The app checks this repository's `/releases` on demand (Settings → Check for
updates) and installs the signed APK from here. Updates are never pushed
automatically; you always confirm the install.

## Releases

- **v1.2.1** — Calls that reach you: Answer/Decline actions on call banners,
  auto-answer when you tap Answer, keep-alive service (calls ring even with
  the app closed). AI now works even when shared-store quota hiccups (local
  optimistic rendering + 5-minute cached config read). Videos in chats render
  inline, Jewish Status page is fully scrollable with collapsed filters +
  creator grid, smaller APK (~108 MB, arm64).
- **v1.2.0** — Agora calling (shared worker token server + ICE/TURN from the
  same globalSettings, automatic WebRTC fallback), keep-alive service so
  nextext calls ring with the app closed, pause/eye toggle/download on the
  status viewer, frozen-video fix, Jewish Status as "The Hock" podcast +
  "Updates" creator rings, AI config caching + model fallback chains,
  disguise setup flows and full launcher-icon set, updater with separate
  install/download paths, 1.2.0 (3).
- **v1.1.0** — Status studio (full editors, stickers, voiceover, downloads),
  Jewish podcast player with date picking, AI voice fixes (persona voices,
  generating states, STT, provider failover, AI podcasts), cross-app call fixes
  (mic permission preflight, video call ringing, full-screen lock-screen UI,
  PiP, ICE watchdog), in-app camera (photo/video, zoom, status/chat destinations),
  Calculator/Notes disguises, archive-instead-of-leave, green splash, 1.1.0 (2).
- **v1.0.0** — First release. Full-feature native client.
