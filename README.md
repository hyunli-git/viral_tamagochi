# 🥚 Tomo - Virtual Pet Game

Raise your own cute digital pet! A retro-style virtual pet game with analog vibes.

![Tomo Game Preview](preview.png)

## ✨ Features

- **Retro Analog Design**: 90s virtual pet-inspired UI
- **CRT Scanline Effect**: Classic LCD screen vibes
- **4 Stats Management**: Hunger, Happiness, Energy, Cleanliness
- **Level Up System**: Earn EXP by taking good care of your pet
- **Evolution System**: Pet evolves at certain levels
- **Auto Save**: Game saves automatically to local storage
- **Offline Time**: Time passes even when you're away
- **Responsive Design**: Works on mobile & desktop

## 🎮 How to Play

1. **🍖 Food**: Fill hunger stat
2. **🍬 Snack**: Fill happiness (but increases weight!)
3. **🎮 Game**: Play mini-game for happiness & EXP
4. **💡 Light**: Turn off for sleep, recover energy
5. **🧹 Clean**: Clean up poop, restore cleanliness
6. **💊 Med**: Cure sickness
7. **👍 Praise**: Increase discipline

## ⚠️ Warning

- If hunger or happiness reaches 0, your pet will die!
- Take care of your pet regularly

## 🚀 Getting Started

### Run Locally
```bash
npx serve .
# or
python -m http.server 8000
```

Open `http://localhost:8000` in browser

### Deploy

Static files - host anywhere:
- **Cloudflare Pages** (free)
- **GitHub Pages** (free)
- **Netlify** (free)
- **Vercel** (free)

## 💰 Google AdSense Setup

1. Sign up at [Google AdSense](https://www.google.com/adsense)
2. Get site approved
3. Uncomment AdSense code in `index.html` and replace `YOUR_PUBLISHER_ID`

## 📁 Project Structure

```
tomo/
├── index.html      # Main game file (HTML + CSS + JS)
├── README.md       # Project docs
└── privacy.html    # Privacy policy (for AdSense)
```

## 📄 License

MIT License - free to use, modify, and distribute

---

Made with ❤️ for virtual pet lovers
