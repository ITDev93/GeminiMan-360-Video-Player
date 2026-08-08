# 🌍 GeminiMan 360 Video Player

<p align="center">
  <strong>Local, online, 360°, panoramic and immersive video playback for Android.</strong>
</p>

<p align="center">
  Watch immersive videos using touch and motion controls, browse websites for playable streams, save useful links, and even give ordinary flat videos a curved Fake 360 viewing experience.
</p>

---

## ✨ About

**GeminiMan 360 Video Player** is an Android video player built for flexible local and online playback.

I originally created it because I wanted an easy way to enjoy panoramic and immersive videos without always needing a VR headset.

Over time, the project has grown into much more than a basic 360° player. It now includes a built-in video browser, stream detection, saved video and website libraries, multiple projection modes, playback caching, browser privacy controls, localization, and an experimental Fake 360 mode for ordinary videos.

The app is designed to remain simple to use while still giving users control over how and where their videos are played.

---

## 🎬 Features

### 🌐 Local & Online Playback

Play videos from:

- Local device storage
- Direct video URLs
- Saved Library entries
- HLS streams
- DASH streams
- Signed and redirected links
- Streams detected through the built-in browser

Playback is powered by **AndroidX Media3 / ExoPlayer**.

---

### 🌎 360° Viewing

Watch compatible panoramic and 360° videos with:

- Touch look-around
- Motion / gyroscope controls
- Recenter controls
- Full-screen playback
- Landscape VR viewing

A VR headset is not required.

---

### 🌀 Fake 360

Ordinary flat videos can also be displayed using the experimental **Fake 360** renderer.

Instead of pretending that missing 360° imagery exists, the video is wrapped around a configurable curved viewing area.

Fake 360 supports:

- Adjustable curvature
- Adjustable field of view
- Touch look-around
- Motion look-around
- Recenter
- Optional repeated rear view
- Landscape Cardboard presentation

> Fake 360 does not convert ordinary footage into genuine captured 360° video. It provides an immersive curved presentation of existing flat

> Fake 360 does not convert ordinary footage into genuine captured 360° video. It provides an footage.

---

### 🥽 Cardboard View

Landscape mode supports split-screen Cardboard viewing for compatible phone VR headsets.

Cardboard controls are intentionally hidden in portrait mode.

---

## 🌐 Built-in Video Browser

Browse websites directly inside the app when a video is not available as a simple direct link.

The browser can:

- Detect playable streams
- Display detected stream information
- Let you choose which detected stream to play
- Preserve website login sessions when enabled
- Navigate normal webpage history
- Copy the current page link
- Open pages externally
- Switch between mobile and desktop browsing
- Pin useful websites
- Keep a lightweight Recent Sites list

### Recent Sites

The browser remembers recent websites by domain rather than filling the list with repeated pages from the same site.

The five most recently used unique websites are available from the website-entry screen for quick access.

---

## 🎞️ Stream Detection

When supported media is detected, the app presents the available stream candidates instead of automatically opening the first one.

Depending on what the website exposes, detected information may include:

- Stream type
- Resolution / quality
- Duration
- File size
- HLS or DASH information
- Request-header requirements
- Source information

Some streams require cookies, referer information, user-agent information, or other request headers in order to remain playable.

---

## 📚 Video Library

Successfully played online videos can be saved for later.

Library entries can contain:

- Display name
- Video URL
- Playback position
- Media type
- Required playback headers
- Last-played information
- Pinned state

### 📌 Pinned Videos

Important videos can be pinned.

Pinned videos are protected from **Clear History**.

To delete a pinned video:

1. Unpin it.
2. Delete it normally.

This prevents important saved links from being removed accidentally.

---

## 🔖 Saved Websites

Websites are stored separately from video history.

Useful websites such as search engines or frequently visited video pages can be pinned and reopened directly from the Library.

Saved websites do **not** store browser cookies or authentication sessions inside the bookmark itself.

---

## ▶️ Continue Watching

When a resumable video is available, the Home screen provides a **Continue Watching** entry.

The player session can also remain loaded while returning temporarily to the Home menu, allowing the user to return to the video without starting over.

---

## 💾 Video Cache

Media3 playback caching can reduce unnecessary re-downloading and improve repeat playback.

Video cache controls are kept separate from browser cache.

---

## 🧹 Browser Data Controls

Browser data can be cleared selectively from Settings.

Available categories include:

- Recent sites
- Cached images and files
- Cookies and website sessions
- Website storage

Clearing browser data does **not** automatically remove:

- Saved videos
- Pinned videos
- Saved websites
- Media3 video cache
- Playback headers attached to saved video records

---

## 🔐 Saved Playback Authentication

Some online videos cannot be replayed using their URL alone.

When required, the app can save the request information associated with a video, such as cookies or request headers, so that the saved video remains usable for as long as those credentials remain valid.

These credentials remain private to the application.

Temporary links and authentication can still expire, in which case the website may need to be opened and authenticated again.

---

## ☁️ Privacy-aware Backup

The app does **not** transfer complete application data through Android cloud backup or device migration.

Backup is deliberately sanitized.

Eligible restored data can include useful Library metadata and safe URLs, while sensitive information such as:

- Cookies
- Sessions
- Authorization headers
- Playback authentication
- Browser storage
- Cached media
- Local URI permissions

is excluded.

A restored protected entry may therefore require the user to sign in again before the stream can be refreshed.

---

## 🍪 Browser Privacy Options

The built-in browser provides lightweight controls for:

- Cookies
- Website local storage
- Third-party cookies
- Login popups
- Do Not Track

The goal is to provide the controls relevant to video browsing without trying to turn the app into a full general-purpose browser.

---

## 🌍 Languages

GeminiMan 360 Video Player currently supports **23 languages**:

- Arabic
- Chinese (Simplified)
- Chinese (Traditional)
- Dutch
- English
- French
- German
- Hindi
- Hungarian
- Indonesian
- Italian
- Japanese
- Korean
- Malay
- Persian
- Polish
- Portuguese (Brazil)
- Portuguese (Portugal)
- Russian
- Spanish
- Turkish
- Ukrainian
- Vietnamese

The default option is **Device language**, with an optional in-app language selector.

Arabic and Persian layouts include RTL support.

---

## 🔄 Updates

The app supports Google Play in-app update checking.

It can:

- Check silently when the app starts
- Check manually from Settings
- Notify when an update is available
- Download a flexible update
- Prompt when the update is ready to install

---

## 🛠️ Technology

The project is primarily written in **Java** and uses technologies including:

- AndroidX Media3 / ExoPlayer
- Android WebView
- OpenGL ES
- MD360Player4Android
- AndroidX AppCompat
- Google Play Billing
- Google Play In-App Updates

---

## ⚠️ Website Compatibility

Not every online video can be detected or played.

Websites may use:

- DRM
- Encrypted media
- Temporary URLs
- Expiring authentication
- Region restrictions
- Browser-only playback
- Unsupported codecs
- Custom JavaScript players
- Server-side anti-bot or anti-embedding protections

Playback availability therefore depends on the website, stream, authentication state, network and Android device capabilities.

---

## 🐞 Bugs & Feature Requests

Found a problem or have an idea for improving the app?

Please use the GitHub issue tracker:

**https://github.com/ITDev93/GeminiMan-360-Video-Player/issues**

When reporting a playback problem, including the following can help:

- Android version
- Device model
- Whether the source is local, direct-link or browser-detected
- What you expected to happen
- What actually happened
- Relevant Logcat output, if available

Please avoid posting private cookies, authentication headers, signed URLs or other account credentials in public issues.

---

## ❤️ Support My Projects

I build these projects as a hobby and because I genuinely enjoy creating useful tools for the community.

My vision has always been simple: **no ads, no paywalls, and no features locked behind a purchase**. If a feature is part of the app, I want everyone to be able to use it.

If you enjoy my work and would like to support what I do, you can:

- ❤️ [Support me through PayPal](https://www.PayPal.me/Dante63)
- 🎗️ [Support me on Patreon](https://www.patreon.com/c/xda_dante63/membership)
- ⭐ Star my projects on GitHub
- ★ Leave a review for the apps you enjoy
- 🐛 Report bugs and issues
- 💡 Share suggestions and ideas
- 📢 Recommend the projects to others who may find them useful

Your support and feedback help keep development going and improve the projects for everyone, and they always motivate me to keep creating, giving back, and doing more for the community.

---

## 🔒 Privacy

GeminiMan 360 Video Player does not require broad storage access for selecting local videos. Android's document picker is used instead.

Browser and playback information required for app functionality is stored locally.

Sensitive browser sessions and playback authentication are intentionally excluded from sanitized cloud/device-transfer backups.

---

## 📄 License

Please refer to the repository's license file for the terms that apply to the source code and project assets.

---

## 👨‍💻 Developer

**GeminiMan**

Built with passion, experimentation, and a lot of testing ♡

---

<p align="center">
  <strong>GeminiMan 360 Video Player</strong><br>
  Local • Online • 360° • Fake 360 • Cardboard • Stream Detection
</p>
