# Kiro Setup Guide

Kiro is an agentic IDE that helps you do your best work with AI-powered development features.

**Prerequisites:** You should have already created a Devvit project using the templates from [Step 1](step-01-devvit-templates.md).

## Installation

### Download and Install Kiro

1. Go to [kiro.dev/downloads](https://kiro.dev/downloads/) and download the installer
2. Open the downloaded file and follow installation instructions for your OS (Windows, macOS, or Linux)
3. Open Kiro IDE

### First Run Setup

1. **Login**: Choose from social or AWS login options
2. **Import Settings**: Optionally import VS Code settings and extensions
3. **Theme Selection**: Choose your preferred theme
4. **Shell Integration**: Allow Kiro to execute commands on your behalf

---

## 🎮 Using Kiro for Game Development

### Step 1: Open Your Devvit Project

Navigate to your project directory and open it in Kiro:

```bash
cd my-devvit-app
kiro .
```

Or use **File > Open Folder** to select your project directory.

**Note:** Kiro may ask if you trust the authors of the files in this folder. Click "Yes" or "Trust" to proceed.

![Trust Prompt](../assets/images/kiro-trust-prompt.png)

![Open Project](../assets/images/kiro-open-project.png)

### Step 2: Create Your Game

1. Click the **Kiro Ghost icon** in the activity bar (left sidebar)
2. This opens Kiro's features panel with chat interface

![Kiro Panel](../assets/images/kiro-panel-overview.png)

Kiro offers two approaches for building features:

**Vibe (Recommended for Quick Development):**
- Direct, conversational approach
- Start building immediately without formal planning
- Best for rapid prototyping and simple features

**Spec (Alternative for Structured Development):**
- Formal requirements, design, and task phases
- Best for complex features requiring detailed planning

**Workflow:**
```
1. Select the Vibe option in the panel
2. Enter your prompt: 
   "Modify this Reddit Devvit app to create a tetris-like game with the following functionality:
   
   - Game grid with falling blocks
   - Score display and tracking
   - Reddit username integration
   - Mobile-responsive design
   - Line clearing mechanics
   - Restart button for new games
   
   Note: Don't change the app's name. Do NOT run any build commands or npm scripts, I will handle all building and deployment."
3. Kiro starts building immediately based on your description
```

![Game Prompt](../assets/images/kiro-game-prompt.png)

Kiro will start building your game step by step:

![Game Building](../assets/images/kiro-game-building.png)

After completion, Kiro will show a summary of everything that was built:

![Game Complete](../assets/images/kiro-game-complete.png)

### Step 3: Test Your Game

Run the development server to see your game in action:

```bash
npm run dev
```

![Terminal URL](../assets/images/kiro-terminal-url.png)

Open the provided URL in your browser to play your Tetris-like game:

![Game Running](../assets/images/kiro-game-running.png)

---

## 🎮 Game Development Examples

### Building Different Game Types

**Memory Card Game:**
```
Modify this Reddit Devvit app to create a memory card matching game with the following functionality:

- 4x4 grid of cards with flip animations
- Score tracking and timer
- Win condition with celebration
- Reddit username integration
- Mobile-responsive design

Note: Don't change the app's name. Do NOT run any build commands or npm scripts, I will handle all building and deployment.
```

**Clicker Game:**
```
Modify this Reddit Devvit app to create a clicker game with the following functionality:

- Large clickable button that increases score
- Score display with animated counter
- Upgrade system (auto-clicker, multipliers)
- Reddit username integration
- Mobile-responsive design

Note: Don't change the app's name. Do NOT run any build commands or npm scripts, I will handle all building and deployment.
```

---

## ⭐ Best Practices

- **Be Specific**: Include exact requirements and functionality in your prompts
- **Break Down Features**: Create detailed descriptions for complex game mechanics
- **Iterate with Chat**: Refine implementations through conversation
- **Test Frequently**: Build and test games regularly during development

## 🔧 Troubleshooting

**Installation Issues:**
- Verify system requirements for your OS
- Run installer as administrator (Windows) or with proper permissions

**Project Not Loading:**
- Ensure project directory contains valid code files
- Check file permissions in project folder
- Restart Kiro and try reopening project

**Authentication Problems:**
- Clear browser cache if using social login
- Verify AWS credentials if using AWS login
- Try alternative login method
