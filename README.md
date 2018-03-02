# NeterraProxy

![NeterraProxy](https://raw.githubusercontent.com/sgloutnikov/NeterraProxy/master/app/src/main/res/mipmap-xxhdpi/ic_launcher.png)

[What/Why/How](#what)<br>
[Instructions](#instructions)<br>
[Perfect Player Example & Settings](https://github.com/sgloutnikov/NeterraProxy#perfect-player-example--settings)<br>
[Video on Demand (Видеотека) [BG]](https://github.com/sgloutnikov/NeterraProxy#video-on-demand-%D0%92%D0%B8%D0%B4%D0%B5%D0%BE%D1%82%D0%B5%D0%BA%D0%B0)<br>
[Perfect Player Video on Demand (Видеотека) Example [BG]](https://github.com/sgloutnikov/NeterraProxy#perfect-player-video-on-demand-%D0%92%D0%B8%D0%B4%D0%B5%D0%BE%D1%82%D0%B5%D0%BA%D0%B0-example)

## What?
NeterraProxy is an on-demand m3u8 playlist/playback daemon for Neterra.tv, running on Android. (4.0+).

## Why?
Have the freedom to watch on your desired IPTV player or TV (Perfect Player, Kodi IPTV Simple, Android Live Channels, GSE Smart IPTV Player, etc). Play links issued by Neterra expire after 12 hours to prevent abuse. Traditional playlist generators need to be run again in order to generate new links. This is not the case for NeterraProxy.

## How?
NeterraProxy generates a specialized playlist that points to itself rather than Neterra. When NeterraProxy receives a playback request it determines the context of the request and responds with a 301 redirect to a valid corresponding Neterra play link. It automatically re-authenticates if the session has expired.

---
## Instructions
1) Download the latest apk from the [releases](https://github.com/sgloutnikov/NeterraProxy/releases) section. You can use the following URL to more easily access and install the APK from a browser on your device: http://tinyurl.com/neterraproxy
2) Install/Side Load and launch NeterraProxy on your Android device. 
3) Enter your Neterra.tv **Username** and **Password** and press **Save**.
4) Back out of NeterraProxy (or press Home) to leave it running. **Exit** will terminate NeterraProxy.
5) Make sure HTML5 Player (not Flash) is selected in your account settings on http://neterra.tv.
6) Use the following URL to connect NeterraProxy with your favorite IPTV player:
    * Playlist URL: http://localhost:8889/playlist.m3u8
    * EPG URL: http://localhost:8889/epg.xml
    * VOD Favorites: http://localhost:8889/vod.m3u8
---
## Perfect Player Example
![PerfectPlayer1](https://raw.githubusercontent.com/sgloutnikov/NeterraProxy/master/screenshots/ppdemo1.png)

---
## Acknowledgments
* SmoothProxy
* KodiBG.org for providing the EPG source
