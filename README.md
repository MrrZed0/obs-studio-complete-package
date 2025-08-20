# 🎥 OBS-Studio + Streamer.bot + Speaker.bot Streaming Setup

This setup is designed to run **entirely on your local machine**, combining **OBS-Studio**, **Streamer.bot**, and **Speaker.bot** for a complete streaming experience. Everything is self-contained and customizable, with overlays, alerts, music integration, and more.

---

## 📦 Included in this Pack
- **OBS-Studio** (Streaming software)
- **Streamer.bot** (Automation & alerts)
- **Speaker.bot** (Audio-based alerts)
- **YouTube Music App Integration**
- **Custom Alerts** with animations + randomized sounds from a folder
- **YouTube Music Overlays** with chat messages on song change
- **Channel Rewards** for adding songs or random song plays
- **Music Player Overlay** for YouTube Music
- **End Stream Credits**
- Common Twitch Commands: `!so`, `!lurk`
- **Be Right Back** Twitch clips overlay
- **Custom Shoutouts Overlay** with chat messages
- Pre-configured **OBS Scenes**: Starting Soon, BRB, Live, Ending, etc.

---

## 🔧 Things You’ll Need to Update

### 🎬 Scenes in OBS
Update the following sources inside `Live_Overlay`:

- `Webcam_Group`
- `PC Game Group`
- `Game Capture Card Group`
- `Microphone`

---

### 📢 Shoutout Player (OBS)
Path: `Scenes > Alerts > Shoutouts Player Overlay > URL`

Change the **username** in this URL:

```text
file:///C:/Program%20Files/OBS-Studio/Files/Sources/Alerts/twitch_shoutout/shoutout.html?channel=USERNAME&showClip=true&showMsg=false&showText=false&showImage=true&raided=false&raidCount=3&delay=10&modsOnly=true&timeOut=60&command=so&customMsg=&customTitle=&showDetails=false&detailsText=&dateRange=60&themeOption=3&ref=
```

---

### 🎞️ Twitch Clips (OBS)
Path: `Scenes > Be Right Back > Twitch_Clips > URL`

Change **Username** and **Twitch Client ID**:

```text
file:///C:/Program%20Files/OBS-Studio/Files/Sources/Be%20Right%20Back/twitch_clips/clips.html?channel=USERNAME&exclude=&limit=100&dateRange=360&themeOption=2&preferFeatured=false&showText=false&showDetails=true&detailsText=%7Btitle%7D%0AWhile%20streaming%20%7Bgame%7D%0AClipped%20by%20%7Bcreator_name%7D%20%7Bcreated_at%7D&mainAccount=sally_budz&command=&customText=&showFollowing=false&ref=&clientId=TWITCH-CLIENT-ID-HERE
```

---

### 🔊 SoundAlerts.com
Path: `Scenes > Alerts > Shoutouts Player Overlay > URL`

Replace with your **Sound Alerts Key**:

```text
https://source.soundalerts.com/alert/YOUR-SOUND-ALERT-KEY
```

---

### 🔑 Twitch Tokens (Dock Integration)
1. Open this file:  
   `C:/Program Files/OBS-Studio/Files/OBS-Studio_Docks/twitch/index.html`
2. Update the following:
   ```js
   const clientId = "TWITCH-CLIENT-ID";
   const clientSecret = "TWITCH-CLIENT-SECRET";
   ```
3. Save.

---

### 👥 Twitch Viewer List (Dock Integration)
1. Open this file:  
   `C:/Program Files/OBS-Studio/Files/OBS-Studio_Docks/viwer_list.html`
2. Update the following:
   ```js
   const CLIENT_ID = "CHANGE-ME"; 
   const ACCESS_TOKEN = "CHANGE-ME"; 
   const BROADCASTER_ID = "CHANGE-ME"; 
   const MODERATOR_ID = "CHANGE-ME"; 
   const REFRESH_INTERVAL = 10000; // update every 30s

   const usernames = ['stefxx96', 'spidermandingo', 'mrrzed0', 'anita_togo_box', 'diciestzebra'];
   ```
3. Save.

---

## 🎥 OBS-Studio Setup

### Scenes
- Starting Stream
- Live [PC]
- Live [Console]
- Live [Full Screen]
- Webcam [Full Screen]
- Be Right Back
- Ending Stream
- Live Overlay
- Alerts
- Transition

### Docks
- Music Player
- Hot Words From Chat
- Viewer List
- Twitch Activity Feed
- Twitch Chat
- Event List
- Scenes
- Sources
- Controls

---

## 🤖 Streamer.bot Setup

### Twitch Alerts with Sounds
Pre-configured alerts:
- Bits / Cheers (with Bits Rain overlay)
- New Follower
- Gift Subs & Prime Subs
- Resubs
- Raids
- Hype Train (start/end)
- Shoutouts
- Guest Star events
- Lurk command & reward
- Game changes

---

### 🎁 Custom Channel Rewards
Add via: `Platforms > Twitch > Channel Point Rewards`

#### Examples:

- **Addams Family Theme Song**
  - Plays theme song on redemption.

- **Lurk Mode Activated**
  - Message + lurking overlay.

- **Official Tittie-o-Meter**
  - Funny randomized result.

- **Peen-o-Meter 3000**
  - Comedy “measurement.”

- **SillyMeter**
  - Measures silliness for fun.

- **Wetness Meter**
  - Splashy and goofy effect.

- **SPLAT**
  - On-screen splat animation.

---

## 🎨 Custom Overlay Setup

Replace these files with your own assets:

```text
C:/Program Files/OBS-Studio/Files/Sources/logo.png
C:/Program Files/OBS-Studio/Files/Sources/Alerts/Alert.webm
C:/Program Files/OBS-Studio/Files/Sources/Be Right Back/BRB Screen.webm
C:/Program Files/OBS-Studio/Files/Sources/Ending_Stream/Ending Screen.webm
C:/Program Files/OBS-Studio/Files/Sources/Intro_Music/1.flac
C:/Program Files/OBS-Studio/Files/Sources/Intro_Music/2.flac
C:/Program Files/OBS-Studio/Files/Sources/Live [Full_Screen]/Webcam.webm
C:/Program Files/OBS-Studio/Files/Sources/Live_Overlays/Background_Overlay.png
C:/Program Files/OBS-Studio/Files/Sources/Live_Overlays/Top Overlay.webm
C:/Program Files/OBS-Studio/Files/Sources/Starting Stream/Starting Screen.webm
C:/Program Files/OBS-Studio/Files/Sources/Transition/Transition.webm
C:/Program Files/OBS-Studio/Files/Sources/Webcam [FullScreen]/Background_Overlay.png
```

---

✨ With this setup, you’ll have a **fully functional streaming package** — local, customizable, and ready to go with OBS, Streamer.bot, and Speaker.bot.
