# 🎥 OBS-Studio + Streamer.bot + Speaker.bot Streaming Setup

This setup is designed to run **entirely on your local machine**, combining **OBS-Studio**, **Streamer.bot**, and **Speaker.bot** for a complete streaming experience. Everything is self-contained and customizable, with overlays, alerts, music integration, and more.

## 📦Latest Release [Updated: 8/25/2025]
📦 [Download Latest Release](https://mrzed0.com/wp-content/uploads/OBS-Studio-Public.zip)

---

## 📦 Included in this Pack
- **OBS-Studio** (Streaming software)
- **Streamer.bot** (Automation & alerts)
- **Speaker.bot** configuration files for TTS (speaks every chat message + alerts to streamer)
- **YouTube Music App Integration**
- **Custom Alerts** with animations + randomized sounds from a folder
- **YouTube Music Overlays** with chat messages on song change
- **Channel Rewards** for adding songs or random song plays
- **Music Player Overlay** for YouTube Music
- **End Stream Credits**
- Common Twitch Commands: `!so`, `!lurk` With Custom Random Chat Message & Overlay
- **Be Right Back** Twitch clips overlay
- **Custom Shoutouts Overlay** with chat messages
- Pre-configured **OBS Scenes**: Starting Soon, BRB, Live, Ending, etc.
- Shoutout Player Playing Twitch Clips Using Streamer.bot
- Alerts, Shoutout Player, Overlays, Sound Alerts Are All Running Local Using Streamer.bot

---

## 🛠️ Setup Instructions

### Log In To The Following To Make Everything Work

#### Location: Unpack The OBS-Studio Folder To
```
C:\Program Files\
```

#### Shortcut: Make Desktop Shortcuts
```
C:\Program Files\OBS-Studio\bin\64bit\obs64.exe
```
```
C:\Program Files\OBS-Studio\Streamer.bot\Streamer.bot.exe
```
```
C:\Program Files\OBS-Studio\Speaker.bot\Speaker.bot.exe
```
```
C:\Program Files\OBS-Studio\YouTube_Music\YouTube Music.exe
```


#### Streamer.bot
- Platforms > **Twitch** > Accounts > Login (Broadcaster Account & Bot Account)  
- Integrations > **Streamlabs** > Login  
- Integrations > **StreamElements** > Login  
- Integrations > **Streamer.bot Website** > Login 

#### Speaker.bot
- Settings > Accounts > **Twitch** > Login  
- Settings > Accounts > **Streamer.bot Website** > Login  
- Settings > Accounts > **Streamlabs** > Login  
- Settings > Accounts > **StreamElements** > Login  

#### OBS-Studio
- Settings > **Stream** > Connect Account  


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
Add via Streamer.bot: `Platforms > Twitch > Channel Point Rewards`

#### Streamer.bot Rewards:

- **Addams Family Theme Song**
  - Thanks for the vibes, You're officially lurking in the shadows. Kick back, mute if needed, and let the stream play while you handle life stuff. Your support still counts big time!

- **Lurk Mode Activated**
  - Thanks for the vibes, You're officially lurking in the shadows. Kick back, mute if needed, and let the stream play while you handle life stuff. Your support still counts big time!

- **Official Tittie-o-Meter**
  - Step right up! The Tittie-o-Meter has spoken, and it’s time to reveal the official size. 100% accurate, totally scientific, and guaranteed to cause at least one giggle.

- **Peen-o-Meter 3000**
  - Think you’ve got what it takes? Redeem this and let the all-knowing Peen-o-Meter 3000 scientifically (and 100% accurately… not really) determine your official Twitch peen size. Results may shock you. Confidence may skyrocket. Viewer discretion advised.

- **SillyMeter**
  - Redeem this to find out just how silly you are. Get ready for some goofy fun and playful vibes in chat!


- **Wetness Meter**
  - Redeem this reward to see how wett you are right now! Get ready for some splashy fun and silly chat moments.

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

---

## 📜 License

This project is open-source and available under the **MIT License**.
