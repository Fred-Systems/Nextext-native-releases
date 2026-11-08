# Nextext-native-releases

Download and update channel for **NexText Native** (`com.nextext.native`) — the
full NexText experience as a native Android app, from Fred Systems.

NexText Native shares the same Firebase backend as the regular NexText app, so
accounts, chats, groups, contacts, statuses, calls and moderation are fully
interoperable with it. It is a **separate app** from NexText.Lite
(`com.nextext.fig`) — nothing is shared between them except the backend.

## Download

Latest release: **[NexText-v1.0.0.apk](https://github.com/Fred-Systems/Nextext-native-releases/releases/latest)**

1. On your Android phone, open the link above.
2. Download `NexText-v1.0.0.apk`.
3. Tap it and allow "install unknown apps" if asked.
4. Open NexText and sign in with your regular NexText account.

Requires Android 7.0+ (minSdk 24). Signed with the NexText Native release key
(SHA-1 `FA:CF:CA:F6:67:14:E3:F9:CD:FA:C7:8C:33:07:98:30:2E:CE:A0:AF`).

## What's included

Chat (text, images, **videos**, voice notes, polls, files, location, weather),
group chats, **voice and video calls** (WebRTC), **status** (contacts and
public, text/photo/video/voice, 24 h expiry), **Jewish Statuses** (JewishStatus
& YidStatus feeds inside the Status tab), the **Video Library** (YouTube and
Dailymotion), **NexText AI** (hundreds of personas, translation, Whisper
transcription, image analysis and generation, summaries, voice replies), and
**voice cloning** (Fish Audio: AI voice notes, cloned voice notes from a voice
recording, voice-sample submission).

Full details and the privacy posture are in
[`Fred-Systems/Nextext-native`](https://github.com/Fred-Systems/Nextext-native)
(`README.md`).

## How admins see this app's users

Native clients tag their accounts (`clientVariant: "native"`, `nativeUser: true`,
`nativeOnline`, `nativeAppVersion`, `nativeLastSeen`) so the admin dashboard can
list and moderate Native users separately from NexText.Lite and regular NexText
accounts. See `ADMIN_PROMPT.md` in that repository.

## Updates

The app checks this repository's `/releases/latest` on demand (Settings → Check
for updates) and installs the signed APK from here. Updates are never pushed
automatically; you always confirm the install.
