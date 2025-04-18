# 🎧 Advanced Music Player App

An Android Music Player App built with **Kotlin** using **MediaPlayer** and **MediaRecorder** APIs.  
It supports **play, pause, next song**, and also allows the user to **record audio** using the device's microphone.

---

## 📱 Features

- 🎵 **Play Music** – Plays audio files from device storage  
- ⏸️ **Pause Music** – Toggle between play and pause  
- ⏭️ **Next Song** – Move to next track in the playlist  
- 🔁 **Now Playing Animation** – Highlights the currently playing song  
- 🎙️ **Audio Recording** – Record audio using microphone and save it  
- 🎨 **Splash Screen** – Clean app opening with logo  
- 📁 **Permission Handling** – Storage and microphone permissions (supports Android 11+)

---

## 🧰 Tech Stack

| Component      | Details                     |
|----------------|-----------------------------|
| Language       | Kotlin                      |
| IDE            | Android Studio              |
| UI Design      | XML, View Binding           |
| Media Playback | Android `MediaPlayer` API   |
| Audio Recorder | Android `MediaRecorder` API |
| UI Animation   | Lottie / View animation     |

---

## 📂 App Structure

com.chinmoy09ine.musicplayer/ ├── activities/ │ ├── MainActivity.kt # Loads music list │ ├── MusicActivity.kt # Handles playback │ ├── RecorderActivity.kt # Records audio │ └── SplashActivity.kt # Splash screen │ ├── adapter/ │ └── MusicAdapter.kt # RecyclerView Adapter │ ├── model/ │ └── MusicModel.kt # Song data model │ ├── utils/ │ └── MyMediaPlayer.kt # Singleton MediaPlayer │ ├── res/ │ ├── layout/ # XML UI files │ ├── drawable/ # Images/icons │ └── raw/ # Audio (if any)

pgsql
Copy
Edit

---

## 🔐 Required Permissions

Make sure to add these in `AndroidManifest.xml`:

```xml
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" android:maxSdkVersion="32" />
<uses-permission android:name="android.permission.RECORD_AUDIO" />
<uses-permission android:name="android.permission.MANAGE_EXTERNAL_STORAGE" />
<uses-permission android:name="android.permission.READ_MEDIA_AUDIO" />
