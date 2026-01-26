


# InstaGrab - Instagram Downloader for Termux

**Download Instagram Reels, Stories, and more directly to your phone through Termux.**

🔗 **Full Documentation:** [Termux InstaGrab](https://termux-instagrab.pages.dev/)




## ✨ What This Does

I made InstaGrab because I wanted a quick way to save Instagram content without dealing with sketchy apps or watermarks. It's a Termux script that lets you share reels or stories directly to your terminal—everything downloads in the background and saves to your gallery.

**Why I built it:**
- No sketchy websites with 50 download buttons
- No watermarks or quality loss
- Works even with private accounts (if you follow them)
- Just share → done → get notified

## 🚀 Quick Start (Takes 2 minutes)

### 1. Setup Termux
```bash
termux-setup-storage
pkg update && pkg upgrade -y
pkg install python ffmpeg termux-api -y
pip install yt-dlp gallery-dl
mkdir -p ~/bin
```

### 2. Install the Script
Copy the script from our [setup page](https://termux-instagrab.pages.dev/#script) or run:

```bash
curl -o ~/bin/termux-url-opener https://raw.githubusercontent.com/PushpkGoat/Instagram-Reels-Stories-Downloader-Termux/main/termux-url-opener
chmod +x ~/bin/termux-url-opener
```

### 3. Use It
1. Open any Reel or Story on Instagram
2. Tap "Share" → Select "Termux"
3. That's it! Downloads run in background
4. Get a notification when it's done

## 📁 Where Files Go

- **Reels:** `/storage/emulated/0/DCIM/Instagram_Reels/`
- **Stories:** `/storage/emulated/0/DCIM/Instagram_Stories/`

Files are named like `@username_20241225_143022.mp4` so they're easy to find and organize.

## 🔧 Pro Tips

### For Private Accounts
If you want to download from private accounts you follow:
```bash
# Copy cookies from your browser and save them
nano ~/cookie.txt
```
Then paste your Instagram cookies there. The script will use them automatically.

### Want Different Folders?
Edit `~/bin/termux-url-opener` and change these lines:
```bash
DOWNLOAD_DIR="/storage/emulated/0/YourCustomFolder"
```

## 🤝 Want to Help Improve It?

Found a bug? Want a feature? Feel free to:
1. Open an Issue (tell me what's wrong)
2. Submit a Pull Request (if you fixed something)
3. Fork it and make your own version

## 📄 License

MIT License - basically means you can use, modify, and share it freely. Just credit me if you redistribute it. See the [LICENSE](LICENSE) file for the legal stuff.

## ⚠️ Quick Disclaimer

This is for personal use only. Please:
- Don't download stuff you don't have permission to save
- Respect copyright and people's privacy
- Check Instagram's Terms of Service



💡 **Check out the [full webpage](https://termux-instagrab.pages.dev/) for fancy setup experience.**

**Built because I was tired of sketchy download sites. Hope it helps you too.**

