# mastertype ⌨️

> A modern, competitive typing game with real-time multiplayer racing, live leaderboards, and professional UI design.

**🎮 [Play Now on Vercel](https://mastertype-nine.vercel.app/)** 


## ✨ Features

### 🏆 Competitive Multiplayer
- **Real-time racing** with live progress tracking
- **Instant leaderboards** updated every 200ms
- **Winner announcements** when players take the lead
- **Perfect synchronization** using Firebase timestamps
- **6-character room codes** for easy joining

### ⚡ Real-time Experience
- **Live WPM/Accuracy updates** on both screens simultaneously
- **Leader highlighting** with crown indicators
- **Typing status indicators** showing who's actively typing
- **Smooth animations** and professional transitions
- **Auto-scaling difficulty** with infinite word generation

### 🎮 Host Controls
- **Time management** - hosts can set and update game duration
- **Room management** with automatic cleanup
- **Game flow control** - start races when ready
- **Synchronized settings** across all players

### 🎨 Professional UI
- **Clean, minimal design** with modern aesthetics
- **Dark/Light theme** toggle
- **Responsive layout** for all devices
- **Professional typography** using Inter + JetBrains Mono
- **Subtle animations** without overwhelming effects

### 📊 Advanced Analytics
- **Real-time statistics** - WPM, Accuracy, Errors, Progress
- **Historical tracking** with average WPM calculation
- **Comprehensive rankings** with medals for top 3
- **Live progress bars** with shimmer effects

## 🚀 Quick Start

### Option 1: One-Click Deploy
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/manumishra12/mastertype)

### Option 2: Manual Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/manumishra12/mastertype.git
   cd mastertype
   ```

2. **Set up Firebase**
   - Create a [Firebase project](https://console.firebase.google.com/)
   - Enable Realtime Database
   - Copy your config from Project Settings
   - The config is already set up in the code

3. **Deploy to Vercel**
   ```bash
   npm i -g vercel
   vercel
   ```

4. **Start playing!**
   - Share your Vercel URL with friends
   - Create rooms and compete in real-time

## 🎯 How to Play

### Solo Practice
1. Select "Solo" mode
2. Choose your preferred time (15s - 2min)
3. Click "Start" and begin typing
4. Focus on accuracy and speed

### Multiplayer Racing
1. **Host:** 
   - Enter your name and click "Set"
   - Click "Create" to generate a room code
   - Set game duration using host controls
   - Share the 6-character code with friends
   - Click "Start" when everyone joins

2. **Join:**
   - Enter your name and click "Set"
   - Enter the room code and click "Join"
   - Wait for host to start the race

3. **Racing:**
   - Watch the live leaderboard during gameplay
   - See real-time progress of all players
   - Get announcements when someone takes the lead
   - Compete for the top spot!

## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Database:** Firebase Realtime Database
- **Hosting:** Vercel
- **Fonts:** Inter, JetBrains Mono
- **Real-time:** WebSocket connections via Firebase

## 📱 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## 🏗️ Architecture

```
mastertype/
├── mastertype.html          # Main application file
├── vercel.json             # Vercel deployment config
└── README.md               # This file
```

### Key Components

- **Game Engine:** Handles typing logic, word generation, and statistics
- **Multiplayer System:** Real-time synchronization with Firebase
- **UI Controller:** Manages themes, animations, and responsive design
- **Progress Tracker:** Live updates every 200ms for smooth experience

## 🔧 Configuration

### Firebase Setup
The Firebase configuration is already included in the code:
```javascript
const firebaseConfig = {
  apiKey: "AIzaSyBY_Zw7pJQkuxqsS7ySO-YgIco-FTMUFWg",
  authDomain: "mastertype-d87b6.firebaseapp.com",
  databaseURL: "https://mastertype-d87b6-default-rtdb.firebaseio.com",
  // ... rest of config
};
```

### Vercel Deployment
The included `vercel.json` handles routing:
```json
{
  "rewrites": [
    { "source": "/(.*)", "destination": "/mastertype.html" }
  ]
}
```

## 🎮 Game Mechanics

### Word Generation
- **Dynamic word bank** with 70+ common English words
- **Infinite generation** - automatically adds more words as needed
- **Smart detection** - adds 50 new words when 20 remaining
- **Synchronized across players** for fair competition

### Scoring System
- **WPM Calculation:** (Correct Characters ÷ 5) ÷ Minutes
- **Accuracy:** (Correct Characters ÷ Total Characters) × 100
- **Real-time Updates:** Statistics refresh every 50ms
- **Average WPM:** Historical tracking throughout the game

### Multiplayer Sync
- **Server timestamps** ensure perfect synchronization
- **Countdown coordination** - all players start simultaneously  
- **Progress tracking** with 200ms update intervals
- **Leader detection** with instant announcements

## 🚀 Performance

- **Lightweight:** Single HTML file under 50KB
- **Fast loading:** No external dependencies except Firebase
- **Smooth animations:** 60 FPS rendering where possible
- **Efficient updates:** Optimized Firebase calls
- **Responsive:** Works on all screen sizes

## 🎨 Customization

### Themes
- Toggle between light and dark themes
- Professional color scheme
- Consistent design system

### Typography
- Primary: Inter (clean, readable)
- Monospace: JetBrains Mono (code/stats)
- Optimized font weights and sizes

## 🤝 Contributing

We welcome contributions! Here's how:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add amazing feature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

### Development Guidelines
- Keep the single-file architecture
- Maintain clean, readable code
- Test multiplayer functionality thoroughly
- Ensure responsive design
- Follow existing code style

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Firebase** for real-time database services
- **Vercel** for seamless deployment
- **Inter & JetBrains Mono** for beautiful typography
- **Open source community** for inspiration

## 📞 Support

- **GitHub Issues:** [Report bugs or request features](https://github.com/manumishra12/mastertype/issues)
- **Discussions:** [Community discussions](https://github.com/manumishra12/mastertype/discussions)

---

<div align="center">

**🚀 [Start Playing Now](https://mastertype.vercel.app) | ⭐ [Star on GitHub](https://github.com/manumishra12/mastertype) | 🐛 [Report Issues](https://github.com/manumishra12/mastertype/issues)**

Made with ❤️ for the typing community

</div>

## 🏆 Leaderboard

*Share your best scores!*

| Player | WPM | Accuracy | Date |
|--------|-----|----------|------|
| 🥇 Your Name | 120 | 98% | 2024-12-XX |
| 🥈 | | | |
| 🥉 | | | |

*Add your scores via PR to appear on the leaderboard!*

---

### 🎯 Roadmap

- [ ] **Tournament Mode** - Bracket-style competitions
- [ ] **Custom Word Lists** - Programming, quotes, custom themes
- [ ] **Profile System** - Track personal progress
- [ ] **Sound Effects** - Audio feedback for typing
- [ ] **Mobile App** - Native iOS/Android versions
- [ ] **Analytics Dashboard** - Detailed performance insights
- [ ] **Spectator Mode** - Watch races without participating
- [ ] **Team Competitions** - Group vs group racing

Want to contribute to any of these features? [Open an issue](https://github.com/manumishra12/mastertype/issues) to discuss!
