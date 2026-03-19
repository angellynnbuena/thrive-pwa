# 🌱 Thrive - Mental Wellness Journaling App

A modern, gamified daily journaling application designed to help users develop consistent reflection habits, track emotional growth, and build positive mental health practices.

## 🎯 Features

### 📝 Daily Journaling
- **Emotion Tracking**: Select from 5 emotional states (😢 😟 😐 😊 🤩)
- **Flexible Entries**: Write titled reflections with detailed thoughts and feelings
- **Focus Areas**: Categorize entries by life domains (Work, Relationships, Health, Learning, Finance, Creative, Personal Growth, Goals)
- **Recent History**: View and manage your last 5 entries instantly

### 🏆 Gamification System
- **Points System**: Earn rewards for consistency and depth
  - 50 points per entry (base)
  - +25 bonus points for entries over 200 words
  - +15 bonus points for using focus areas
- **Level Progression**: Track your growth with a visual progress bar
- **Streak Counter**: Maintain consecutive days of journaling
- **Achievement Badges**: Unlock 8 unique achievements as you journal

### 🎖️ Achievements to Unlock
1. **First Steps** 📝 - Write your first entry
2. **Week Warrior** 🔥 - Complete 7 entries in a week
3. **Month Master** 🌟 - Write 30 total entries
4. **Emotional Intelligence** 🎯 - Track all 5 emotions
5. **Philosopher** 🧠 - Write 1,000+ total words
6. **Focused Mind** 💎 - Use 5 different focus areas
7. **Consistent Voice** 🎭 - Maintain 15-day streak
8. **Eloquent** ✨ - Reach 5,000+ total words

### 📊 Progress Dashboard
- **Streak Counter**: Current consecutive days
- **Points Display**: Total accumulated points and level
- **Weekly Stats**: Entries completed this week
- **Monthly Stats**: Entries completed this month
- **Writing Analytics**: Average words per entry

## 🚀 Getting Started

### Requirements
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No installation or Node.js required

### Running the App
1. Open `index.html` directly in your browser
2. Or use a local web server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js
   npx http-server
   ```
3. Navigate to `http://localhost:8000` (or appropriate port)

## 📱 How to Use

### Writing an Entry
1. **Select Your Emotion**: Click one of the 5 emotion buttons
2. **Add a Title**: Give your reflection a meaningful title
3. **Write Your Thoughts**: Share detailed thoughts and feelings
4. **Choose Focus Area** (optional): Select a life domain to track
5. **Save Entry**: Click "Save Entry" or press `Ctrl+Enter` (Cmd+Enter on Mac)

### Viewing Progress
- **Header Stats**: See your streak, points, and total entries at a glance
- **Right Panel**: Monitor weekly/monthly activity and level progress
- **Badges**: Check which achievements you've unlocked

### Managing Entries
- **Recent Entries**: View your last 5 entries in the left panel
- **Delete**: Remove any entry with the delete button

## 💾 Data Storage

All your entries and progress are saved locally in your browser using **localStorage**:
- Entries are stored securely on your device
- Data persists between sessions
- No account or internet connection required
- Data is private and never sent to external servers

### Exporting Your Data
To backup your journal:
1. Open developer console (F12)
2. Run: `JSON.stringify(JSON.parse(localStorage.getItem('thriveData')), null, 2)`
3. Copy the output and save to a text file

## 🎨 Interface Overview

### Left Column
- **Today's Reflection**: Form to create new entries
- **Recent Entries**: Quick view of your latest 5 entries

### Right Column
- **Your Progress**: Personal statistics and level progression
- **Achievements**: Visual display of unlocked badges

### Header
- App branding and logo
- Real-time stats (streak, points, total entries)

## 🔒 Privacy & Security

- **100% Private**: All data stored locally in your browser
- **No Cloud Sync**: Your entries never leave your device
- **No Tracking**: No analytics or user tracking
- **No Ads**: Completely ad-free experience

## 🎯 Tips for Success

1. **Build a Habit**: Journal at the same time each day
2. **Be Honest**: Write freely without judgment
3. **Vary Your Focus**: Use different focus areas to track all life domains
4. **Track Progress**: Watch your streak grow and badges unlock
5. **Reflect Regularly**: Review past entries to track emotional growth

## 🛠️ Technical Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Storage**: Browser localStorage API
- **Styling**: Custom CSS with responsive design
- **Compatibility**: Works on all modern browsers

## 📦 File Structure

```
Thrive/
├── index.html          # Main application file (all-in-one)
├── README.md          # This file
└── .github/
    └── copilot-instructions.md  # Development guidelines
```

## 🌟 Future Enhancements

Potential features for future versions:
- Cloud backup and sync
- Dark mode toggle
- Export entries as PDF
- Emotion trend graphs
- Mood insights and patterns
- Reminder notifications
- Mobile app version
- Collaborative features
- AI-powered insights

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Have ideas to improve Thrive? Feel free to fork, modify, and enhance the app!

## 💬 Support

For issues or feature requests, please document them and consider improvements to the codebase.

---

**Start your Thrive journey today! 🌱**

Remember: Mental wellness is a journey, not a destination. One entry at a time, you're building a better you.
