The reason of using obs-studio and streamer.bot is to make everything run local off your local computer, using OBS-Studio, Streamer.bot And Speaker.bot

Included:
- OBS-Studio Software
- Streamer.bot Software
- Speaker.bot Software
- YouTube Music App
- Alerts With Animated Alert With Random Sound From Folder
- YouTube Music Overlay With Chat Message When Song Change
- YouTube Music Add Songs & Random Song Channel Reward
- YouTube Music Music Player Overlay
- End Stream Credits
- Includes Commands Like !so and !lurk
- Be Right Back Twitch Clips Overlay
- Shoutouts Overlay With Custom Chat Message
- Includes Starting Stream, Be Right Back, Live, End Stream Scenes In OBS-Studio

________________________________________________________________________________________

-----------------
Things To Change:
-----------------

Shoutout Player: [OSB-STUDIO]
-----------------
- Scenes > Alerts > Shoutouts Player Overlay > URL:
[Change Username]
file:///C:/Program%20Files/OBS-Studio/Files/Sources/Alerts/twitch_shoutout/shoutout.html?channel=USERNAME&showClip=true&showMsg=false&showText=false&showImage=true&raided=false&raidCount=3&delay=10&modsOnly=true&timeOut=60&command=so&customMsg=&customTitle=&showDetails=false&detailsText=&dateRange=60&themeOption=3&ref=

Twitch Clips: [OSB-STUDIO]
-----------------
- Scenes > Be Right Back > Twitch_Clips > URL:
[Change Username][Change Twitch Client ID]
file:///C:/Program%20Files/OBS-Studio/Files/Sources/Be%20Right%20Back/twitch_clips/clips.html?channel=USERNAME&exclude=&limit=100&dateRange=360&themeOption=2&preferFeatured=false&showText=false&showDetails=true&detailsText=%7Btitle%7D%0AWhile%20streaming%20%7Bgame%7D%0AClipped%20by%20%7Bcreator_name%7D%20%7Bcreated_at%7D&mainAccount=sally_budz&command=&customText=&showFollowing=false&ref=&clientId=TWITCH-CLIENT-ID-HERE


----------------
SoundAlerts.com: [OSB-STUDIO]
----------------
- Scenes > Alerts > Shoutouts Player Overlay > URL:
[Change URL]
https://source.soundalerts.com/alert/YOUR-SOUND-ALERT-KEY


---------------
Twitch Suggests: [FILE] [https://twitchtokengenerator.com/]
---------------
- C:\Program Files\OBS-Studio\Files\OBS-Studio_Docks\twitch
- Open 'index.html' In Notepad
- Change
const clientId = "TWITCH-CLIENT-ID";
const clientSecret = "TWITCH-CLIENT-SECRET";
- Click File > Save

---------------
Twitch Viewers: [FILE] [https://twitchtokengenerator.com/]
---------------
- C:\Program Files\OBS-Studio\Files\OBS-Studio_Docks\
- Open 'viwer_list.html' In Notepad
- Change
        const CLIENT_ID = "CHANGE-ME"; // Twitch Client ID
        const ACCESS_TOKEN = "CHANGE-ME"; // OAuth Token
        const BROADCASTER_ID = "CHANGE-ME"; // Your Twitch Channel ID
        const MODERATOR_ID = "CHANGE-ME"; // Your Moderator User ID
        const REFRESH_INTERVAL = 10000; // Update every 30 seconds

// Twitch usernames to display
const usernames = ['stefxx96', 'spidermandingo', 'mrrzed0', 'anita_togo_box', 'diciestzebra'];
- Click File > Save



________________________________________________________________________________________

-----------------
OBS-Studio Setup:
-----------------

Scenes:
-------
- Starting Stream
- Live [PC]
- Live [Console]
- Live [Full_Screen]
- Webcam [FullScreen]
- Be Right Back
- Ending Stream
- -------------------
- Live_Overlay
- Alerts
- Transition

Docks:
------
- Music Player
- Hot Words From Chat
- Viewer List
- Twitch Activity Feed
- Twitch Chat
- Event List
- Scenes
- Sources
- Countrol



________________________________________________________________________________________


-------------
Streamer.bot:
-------------

Twitch Alerts With Sounds:
--------------------------
- New Bits/Cheers With Bits Rain Overlay
- New Follower
- New Gift Bomb Subscriber
- New Gift Subscriber
- New Prime Upgrade
- New Raid
- New Resubscribed
- New Shoutout
- New Subscriber
- Guest Star
- Hype Train Started
- Hype Train Ended
- Raid Started
- New Lurk [Using !lurk command or lurk reward]
- Game Change



________________________________________________________________________________________



---------------
Custom Overlay:
---------------

Most Custom Overlay Packs Will Included The Files That Is Needed To Be Replace

The Following Files Will Need To Be Replace:
- C:\Program Files\OBS-Studio\Files\Sources\logo.png
- C:\Program Files\OBS-Studio\Files\Sources\Alerts\Alert.webm
- C:\Program Files\OBS-Studio\Files\Sources\Be Right Back\BRB Screen.webm
- C:\Program Files\OBS-Studio\Files\Sources\Ending_Stream\Ending Screen.webm
- C:\Program Files\OBS-Studio\Files\Sources\Intro_Music\1.flac
- C:\Program Files\OBS-Studio\Files\Sources\Intro_Music\2.flac
- C:\Program Files\OBS-Studio\Files\Sources\Live [Full_Screen]\Webcam.webm
- C:\Program Files\OBS-Studio\Files\Sources\Live_Overlays\Background_Overlay.png
- C:\Program Files\OBS-Studio\Files\Sources\Live_Overlays\Top Overlay.webm
- C:\Program Files\OBS-Studio\Files\Sources\Starting Stream\Starting Screen.webm
- C:\Program Files\OBS-Studio\Files\Sources\Transition\Transition.webm
- C:\Program Files\OBS-Studio\Files\Sources\Webcam [FullScreen]\Background_Overlay.png
