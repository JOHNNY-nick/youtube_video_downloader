# YouTube Downloader (ytp.py)

A simple Python utility to download YouTube videos and playlists in high quality using `yt-dlp`.

## How to use

Follow these steps to set up and run the script:

### 1. Installing the dependencies
Ensure you have Python and FFmpeg installed on your system. Then, install the required Python library:
```bash
pip install -r requirements.txt
```

### 2. Installing "Get cookies.txt LOCALLY" on Chrome
To download restricted or private videos, the script needs your YouTube session cookies. 
- Go to the Chrome Web Store and install the extension [Get cookies.txt LOCALLY](https://chromewebstore.google.com/detail/get-cookiestxt-locally/ccmgnabimndgehpdbnneghjjffabbdie).
- This extension allows the script to access your login state securely.

### 3. Logging in on YouTube
- Open Google Chrome.
- Go to [YouTube.com](https://www.youtube.com) and log in with your account.
- Keep the tab open or ensure you don't log out, so the cookies remain valid.

### 4. Using the script
Run the script by providing the URL of a single video or an entire playlist. The script will automatically fetch the best quality (MP4).

**For a single video:**
```bash
python ytp.py "https://www.youtube.com/watch?v=VIDEO_ID"
```

**For a whole playlist:**
```bash
python ytp.py "https://www.youtube.com/playlist?list=PLAYLIST_ID"
```

---
**Note:** This script is designed for Windows. It will attempt to extract cookies from your Chrome profile automatically to authenticate your downloads.
