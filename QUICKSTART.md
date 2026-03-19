# 🚀 Quick Start Guide - Thrive

Get started with your mental wellness journey in seconds!

## ⚡ Instant Launch

### Option 1: Open Directly (Fastest)
1. Navigate to the Thrive folder
2. Double-click `index.html`
3. Your browser opens and the app is ready to use!

### Option 2: Use a Web Server (Recommended)
**Windows (PowerShell):**
```powershell
python -m http.server 8000
# or
npx http-server
```

**macOS/Linux:**
```bash
python3 -m http.server 8000
# or
npx http-server
```

Then open: `http://localhost:8000`

## 🎯 First Steps

### Your First Entry (2 minutes)
1. **Pick an emotion** - Click how you're feeling (😢 😟 😐 😊 🤩)
2. **Add a title** - Something short and meaningful
3. **Write freely** - Share your thoughts and feelings (no minimum length!)
4. **Optional:** Choose a focus area (Work, Health, Personal Growth, etc.)
5. **Save** - Click "Save Entry" or press `Ctrl+Enter`

### Watch Your Progress
- **Header Stats** - See your streak, points, and entry count
- **Right Panel** - Track weekly/monthly activity
- **Achievements** - Unlock badges as you journal

## 💡 Pro Tips for Maximum Benefits

### Build Your Streak
- Journal every day to build consistency
- Even 2 sentences counts!
- Your streak is displayed in the header

### Earn More Points
- Write longer entries (+25 bonus points)
- Use focus areas (+15 bonus points)
- 50 base points per entry

### Unlock All Achievements
1. **First Steps** - Just write your first entry ✅
2. **Week Warrior** - Complete 7 entries in a week
3. **Month Master** - Reach 30 total entries
4. **Emotional Intel** - Use all 5 emotions
5. **Philosopher** - Write 1,000+ total words
6. **Focused Mind** - Use 5 different focus areas
7. **Consistent Voice** - Build a 15-day streak
8. **Eloquent** - Write 5,000+ total words

## 📊 Understanding Your Dashboard

### Stats Card (Bottom Right)
- **This Week** - Entries written in last 7 days
- **This Month** - Entries written in last 30 days
- **Avg Words** - Average length of your entries

### Progress Bar
- Shows how close you are to next level
- Each level = 500 points
- Current level in center

### Achievements Section
- Gray badge = locked
- Gold badge with glow = unlocked! 🎉

## 🔒 Your Privacy

- ✅ Everything stays on YOUR device
- ✅ No accounts needed
- ✅ No passwords
- ✅ No internet connection required
- ✅ No data sent anywhere
- ✅ 100% private

## 🎨 Customization Tips

### Want to Export Your Data?
1. Open Developer Console (F12)
2. Copy & paste this:
```javascript
JSON.stringify(JSON.parse(localStorage.getItem('thriveData')), null, 2)
```
3. Save the output to a text file - that's your backup!

### Clear Everything (Start Fresh)
```javascript
localStorage.removeItem('thriveData');
location.reload();
```

## ❓ FAQ

**Can I use this on my phone?**
Yes! Open `index.html` on your phone's browser (responsive design works great).

**Will my entries sync across devices?**
Not automatically, but you can export data and import on another device using the developer console.

**What if I close the browser?**
Your entries are saved! They'll be there when you reopen the app.

**How many entries can I save?**
Thousands! Browser storage is usually 5-10MB, plenty for years of journaling.

**Is there a dark mode?**
Not yet, but you can modify the CSS colors in the index.html file.

## 🎯 30-Day Challenge

Try this to build the habit:
- Week 1: 3 entries (focus on consistency over length)
- Week 2: 5 entries (start unlocking achievements)
- Week 3: Daily entries (build your streak!)
- Week 4: Daily + longer entries (unlock more badges)

## 🌟 Remember

There's no "right way" to journal. Some days you'll write a lot, some days just a sentence or two. What matters is showing up and reflecting on your thoughts and feelings.

**You've got this! Let's Thrive together! 🌱**

---

**Need help?** Check the README.md for more detailed documentation.

**Have ideas?** Feel free to customize and enhance the code!
