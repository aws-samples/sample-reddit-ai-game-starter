# Game Examples and Templates

Ready-to-use prompts and examples for building Devvit games with AI tools.

*These are example prompts to inspire your game development. Use them as starting points or modify them for your specific needs.*

## 🎯 Simple Games

### Clicker Game

**AI Prompt:**
```
Create a complete React clicker game for Devvit with:
- Large clickable button that increases score
- Score display with animated counter
- Click multiplier that increases every 10 clicks
- Auto-clicker upgrade (costs 100 points, adds 1 point/second)
- Reddit username display from Devvit context
- Mobile-responsive design
```

### Memory Card Game

**AI Prompt:**
```
Create a complete 4x4 memory card matching game for Devvit with:
- Grid of face-down cards with flip animation
- Match detection (2 cards with same symbol)
- Move counter and timer
- Win condition with celebration animation
- Difficulty levels (4x4, 6x6, 8x8)
- Leaderboard integration with Reddit usernames
```

### Quiz Game

**AI Prompt:**
```
Create a complete trivia quiz game for Devvit with:
- Multiple choice questions (4 options)
- Score tracking with streak bonuses
- Timer per question (15 seconds)
- Progress bar showing question number
- Final score screen with Reddit username
- Questions about the current subreddit
```

## 🤖 AI Prompt Templates

### 🏗️ Complete Game Generation
```
Update the existing Devvit project: build a [GAME_TYPE] game for Reddit's Devvit platform with:
- [SPECIFIC_FUNCTIONALITY]
- Uses TypeScript with proper types
- Includes error handling
- Is mobile-responsive
- Integrates with Reddit context for [USER_DATA/SUBREDDIT_INFO]
```

### 🎨 Styling Prompts
```
Generate CSS for a [THEME] game interface with:
- Color scheme: [PRIMARY_COLORS]
- Layout: [GRID/FLEXBOX] for [MOBILE/DESKTOP]
- Animations: [HOVER_EFFECTS/TRANSITIONS]
- Typography: [FONT_STYLE] that's readable on mobile
- Accessibility: High contrast, keyboard navigation
```

### 🎯 Game Logic Prompts
```
Implement game logic for [GAME_TYPE] that handles:
- Player actions: [CLICK/DRAG/KEYBOARD]
- Win/lose conditions: [SPECIFIC_CONDITIONS]
- Score calculation: [SCORING_RULES]
- Reddit integration for user data
- Performance: Optimized for 60fps on mobile
```

### 🐛 Bug Fixing Prompts
```
Debug this [COMPONENT/FUNCTION] that's having issues with:
- Problem: [SPECIFIC_ISSUE]
- Expected behavior: [WHAT_SHOULD_HAPPEN]
- Current behavior: [WHAT_ACTUALLY_HAPPENS]
- Environment: Devvit web view on [MOBILE/DESKTOP]

[PASTE_CODE_HERE]
```

## 🔗 Reddit Integration Examples

### User Authentication
**AI Prompt:**
```
Help me get current user information from Devvit context and handle anonymous users:
- Get userId and username from context
- Display appropriate name for anonymous users
- Handle cases where username might be undefined
```

### Subreddit-Specific Content
**AI Prompt:**
```
Help me customize my game based on the current subreddit:
- Access subreddit name from Devvit context
- Create different themes for different subreddits
- Handle cases where subreddit info isn't available
```

### Leaderboard Integration
**AI Prompt:**
```
Create a leaderboard system for my Devvit game that:
- Saves scores with Reddit usernames using Redis
- Retrieves and displays top 10 scores
- Handles score updates and duplicates
- Shows current user's rank in the leaderboard
```
