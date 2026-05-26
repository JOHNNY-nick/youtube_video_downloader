# YouTube Downloader (ytp.py)

A simple and efficient Python script to download YouTube videos and playlists in the best possible quality (MP4) using `yt-dlp`. This tool automatically handles authentication using your Chrome session cookies.

---

## 🚀 Quick Start Guide

This guide is designed for absolute beginners using the **Windows Command Prompt (Invite de commande)**.

### Step 0: Prerequisites (One-time setup)
Before running the script, you need two things installed on your computer:

1. **Python**: Download from [python.org](https://www.python.org/downloads/).
   - **⚠️ IMPORTANT:** During installation, check the box **"Add Python to PATH"**.
   - *Pro Tip:* You can also install it via command line: `winget install -e --id Python.Python.3`
2. **FFmpeg**: Needed to merge video and audio into a single MP4 file.
   - Download the "essentials" build from [gyan.dev](https://www.gyan.dev/ffmpeg/builds/).
   - Unzip it and add the `bin` folder to your System PATH.

---

### Step 1: Download the Project
Open your **Command Prompt** (Press `Win + R`, type `cmd`, and press Enter) and run:
```cmd
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

### Step 2: Install Dependencies
Install the required Python library by running:
```cmd
python -m pip install -r requirements.txt
```

### Step 3: Setup Browser Cookies
To download age-restricted or private videos, the script uses your Chrome login:
1. **Install Extension:** Add [Get cookies.txt LOCALLY](https://chromewebstore.google.com/detail/get-cookiestxt-locally/ccmgnabimndgehpdbnneghjjffabbdie) to your Google Chrome.
2. **Log in:** Open [YouTube.com](https://www.youtube.com) and log in to your account.
3. Keep Chrome open or don't log out. The script will find the cookies automatically.

---

## 📥 How to Use

To download, navigate to the folder in your Command Prompt and use these commands:

### Download a Single Video
```cmd
python ytp.py "https://www.youtube.com/watch?v=VIDEO_ID"
```

### Download a Full Playlist
```cmd
python ytp.py "https://www.youtube.com/playlist?list=PLAYLIST_ID"
```

---

## 💡 Windows Survival Tips
- **Where am I?** Type `dir` to see the files in your current folder (like `ls` on Linux).
- **Fast Access:** Open your folder in File Explorer, click the address bar, type `cmd`, and press Enter to open the terminal right there.
- **Errors?** If `pip` doesn't work, always try `python -m pip`.

---

## ⚖️ License & Security
- **License:** This project is under the **MIT License**.
- **Security:** Do **NOT** upload your `cookies.txt` or `.mp4` files to GitHub. They are for your local use only.

**Disclaimer:** This tool is for personal use and educational purposes only. Please respect YouTube's Terms of Service.
