# Thrive - Mental Wellness Journaling App
## Development Guidelines & Project Information

### Project Overview
**Thrive** is a modern, gamified daily journaling application designed to help users develop consistent reflection habits, track emotional growth, and build positive mental health practices. The app features a user-friendly interface, gamification system with rewards and badges, and local data storage for complete privacy.

### Technology Stack
- **Frontend**: HTML5, CSS3, Vanilla JavaScript (ES6+)
- **Storage**: Browser localStorage API
- **Design**: Responsive CSS with gradient backgrounds
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)
- **No Backend Required**: Standalone application

### Project Requirements Met
✅ Daily journaling functionality for thoughts and emotions
✅ Gamified experience with rewards system
✅ User-friendly, intuitive interface
✅ Progress tracking with streaks and points
✅ Achievement badges (8 total)
✅ Emotion tracking (5 emotional states)
✅ Focus areas for life domain categorization
✅ Local data persistence
✅ Responsive design

### File Structure
```
Thrive/
├── index.html                 # Main application (all-in-one file)
├── README.md                 # User documentation
└── .github/
    └── copilot-instructions.md   # This file
```

### Key Features Implementation

#### 1. Journal Entry System
- Form for capturing daily reflections with:
  - Emotion selector (5 options)
  - Title field
  - Content textarea
  - Optional focus area selector
- Validation for required fields
- Quick entry save functionality (Ctrl+Enter shortcut)

#### 2. Gamification Features
- **Points System**:
  - 50 points per entry
  - +25 bonus for entries > 200 words
  - +15 bonus for using focus areas
  - Displayed in header with real-time updates

- **Levels & Progression**:
  - Level = floor(total_points / 500) + 1
  - Visual progress bar for next level
  - Points tracked toward next milestone

- **Streaks**: 
  - Consecutive days with entries
  - Calculated from entry dates
  - Display in header stats

- **Achievements**:
  - 8 unlockable badges
  - Text notification when unlocked
  - Persistent storage across sessions
  - Visual unlock animation

#### 3. Progress Dashboard
- Weekly entry count
- Monthly entry count
- Average words per entry
- Total entry count
- Current level display
- Points progress visualization

#### 4. Data Management
- localStorage-based persistence
- Automatic save on entry creation
- Data structure:
  ```javascript
  {
    entries: [
      {
        id: timestamp,
        date: ISO string,
        emotion: emoji,
        title: string,
        content: string,
        focusArea: string
      }
    ],
    unlockedAchievements: [string]
  }
  ```

### Code Organization

#### Core App Object
```javascript
app = {
  selectedEmotion: null,
  entries: [],
  achievements: {...},
  unlockedAchievements: []
}
```

#### Key Functions
- `loadData()` - Retrieve data from localStorage
- `saveData()` - Persist data to localStorage
- `getCurrentStreak()` - Calculate consecutive days
- `calculatePoints()` - Total points earned
- `updateAchievements()` - Check and unlock badges
- `updateUI()` - Refresh all displays
- `saveEntry()` - Create new journal entry
- `renderRecentEntries()` - Display latest entries
- `renderBadges()` - Show achievements panel

### Styling Approach
- CSS Grid and Flexbox for layout
- CSS custom properties for theming
- Responsive design with media queries
- Gradient backgrounds for visual appeal
- Smooth transitions and animations
- Color scheme:
  - Primary: Indigo (#6366f1)
  - Secondary: Pink (#ec4899)
  - Success: Green (#10b981)
  - Warning: Amber (#f59e0b)
  - Danger: Red (#ef4444)

### Running the Application

#### Method 1: Direct File Open
1. Locate `index.html` file
2. Double-click to open in default browser
3. Application launches immediately

#### Method 2: Local Web Server (Recommended)
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server
```
Then navigate to: `http://localhost:8000`

### Development & Customization

#### Adding New Achievements
Edit the `achievements` object in the app:
```javascript
newBadge: {
  icon: '🎯',
  name: 'Badge Name',
  desc: 'Description',
  condition: (entries) => /* condition logic */
}
```

#### Modifying Scoring System
Adjust points in the `calculatePoints()` function:
```javascript
points += 50;  // Base points
if (entry.content.length > 200) points += 25;  // Word bonus
if (entry.focusArea) points += 15;  // Focus area bonus
```

#### Customizing Emotions
Edit the emotion-grid HTML section and add to emotion checking logic.

#### Styling Changes
All CSS is in the `<style>` tag at the top. Modify using CSS custom properties or direct values.

### Data Privacy & Security
- All data stored locally in browser localStorage
- No external API calls
- No user tracking or analytics
- No cloud synchronization
- Complete user control over data

### Browser Compatibility
- Chrome/Chromium: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- Edge: ✅ Full support
- IE11: ❌ Not supported (uses ES6)

### Known Limitations
- Single device storage only (use localStorage export for backup)
- No cloud sync between devices
- localStorage size limit (~5-10MB depending on browser)
- Entries only visible on same browser/device

### Future Enhancement Ideas
- Dark mode toggle
- Data export/import functionality
- Cloud synchronization
- Mobile app version
- PDF export for entries
- Emotion trend analytics
- Reminder notifications
- Entry search functionality
- Tags/categories system
- Sharing capabilities

### Debugging Tips
- Open DevTools (F12) to check localStorage
- View console for any JavaScript errors
- Inspect network tab (should show no external requests)
- Use localStorage in console: `localStorage.getItem('thriveData')`

### Performance Considerations
- Single-file architecture minimizes load time
- Vanilla JavaScript ensures speed
- localStorage provides instant persistence
- Efficient DOM manipulation
- CSS animations use GPU acceleration

### Code Standards
- ES6+ JavaScript features
- Semantic HTML5
- BEM-style CSS organization
- Clear, descriptive variable names
- Comments for complex logic
- Functional programming style for utilities

### Testing Recommendations
1. Test emotion selection and form submission
2. Verify streak calculation with date changes
3. Confirm achievement unlock notifications
4. Check localStorage persistence across sessions
5. Test responsive design on mobile
6. Validate form inputs and error messages
7. Test with various entry lengths
8. Verify badge rendering and styling

### Support & Documentation
- README.md for user documentation
- Code comments for technical details
- Achievement condition explanations
- Function documentation in comments

### Version Control
- Initial release: v1.0
- Single file distribution
- Easy to version control with git

---

**Last Updated**: March 2026
**Status**: Production Ready
**Maintenance**: Community contributions welcome
