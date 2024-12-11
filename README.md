# TopEmbed Live TV & Sports Playlists

TopEmbed is a platform that offers free live tv and sports streaming across selected categories. Users can stream and watch sports directly through their browser without the need for an account or subscription.

For added flexibility, this repository provides an M3U playlist featuring TopEmbed's channels. With this, you can load the streams into any IPTV application that supports M3U-formatted playlists.

You can view the full list of channels provided by TopEmbed [here](https://href.li/?https://topembed.pw/).

The latest events added to the playlist can be found [here](https://github.com/dtankdempse/topembed-m3u/blob/main/events.txt).

**Note:** These streams provide a mix of HD and 600kbps SD quality, with many events delivered in lower resolutions.

## Playlist Formats

---

### Standard Playlist Information

**Playlist.m3u8**  
This is a standard M3U playlist. To use it, ensure your IPTV application supports custom headers, specifically `Referer` and `User-Agent` (optional). The Referer header is required to access the streams, and not setting it will result in a 403 error.

#### Playlist URLs
- **Events Only:** `https://bit.ly/topembed-m3u1`
- **All Channels:** `https://bit.ly/topembed-m3u1-all`
  
#### Guide URLs
- **EPG (XML):** `https://bit.ly/topembed-epg`
- **EPG (GZ):** `https://bit.ly/topembed-epg-gz`

#### Required Headers
- **Referer:** `https://topembed.pw/`
---

### TiviMate Playlist Information

- **tivimate_playlist.m3u8:**  
  This playlist is specifically formatted for use with TiviMate. Simply load the URL provided in this repository into TiviMate as an "M3U Playlist." No additional setup is needed, as TiviMate automatically manages the required headers for playback.

#### Playlist URLs
  - **Events Only:** `https://bit.ly/topembed-m3u2`
  - **All Channels:** `https://bit.ly/topembed-m3u2-all`
    
#### Guide URLs
  - **EPG (XML):** `https://bit.ly/topembed-epg`
  - **EPG (GZ):** `https://bit.ly/topembed-epg-gz`

**Headers:** *(Automatically handled by TiviMate)*
  - **Referer:** `Included`    
---

### Kodi Playlist Information    

- **kodi_playlist.m3u8:**  
  This playlist is designed for Kodi, utilizing `#KODIPROP` properties to handle the necessary stream settings, including the required headers. It is optimized for Kodi's PVR IPTV Simple Client, ensuring compatibility with your Kodi setup.

#### Playlist URLs
  - **Events Only:** `https://bit.ly/topembed-m3u3`
  - **All Channels:** `https://bit.ly/topembed-m3u3-all`
  
#### Guide URLs
  - **EPG (XML):** `https://bit.ly/topembed-epg`
  - **EPG (GZ):** `https://bit.ly/topembed-epg-gz`

  **Headers:** *(Automatically handled by Kodi)*
  - **Referer:** `Included`      
---

### VLC Playlist Information

- **vlc_playlist.m3u8:**  
  Optimized for VLC Media Player. This playlist uses VLC-specific formatting to ensure streams play correctly, including setting the necessary headers via `#EXTVLCOPT`.

#### Playlist URLs
  - **Events Only:** `https://bit.ly/topembed-m3u4`
  - **All Channels:** `https://bit.ly/topembed-m3u4-all`

#### Guide URLs
  - **EPG (XML):** `https://bit.ly/topembed-epg`
  - **EPG (GZ):** `https://bit.ly/topembed-epg-gz`

  **Headers:** *(Automatically handled by VLC)*
  - **Referer:** `Included`
---
## M3U Playlist Proxy

If none of these playlists work with your IPTV application, you can try using the [m3u-playlist-proxy](https://github.com/dtankdempse/m3u-playlist-proxy). This proxy acts as a middle layer to help resolve potential issues with playing the playlists, especially if your IPTV app doesn't support setting the required headers.

## Usage Instructions:

1. Choose the playlist format that suits your application or media player.
2. Add the playlist URL to your IPTV application.
3. Ensure that your application supports the required settings, such as setting the required headers for streams to play.

## Disclaimer:

This repository has no control over the streams, links, or the legality of the content provided by topembed.pw (including all mirror sites). It is the end user's responsibility to ensure the legal use of these streams, and we strongly recommend verifying that the content complies with the laws and regulations of your country before use.

