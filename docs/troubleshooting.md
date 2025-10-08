# Troubleshooting Guide

Common issues and solutions for template-based Devvit game development.

## 🖥️ Development Server Issues

### Playtest Subreddit Creation Failed

**Error message:**
```
Error: Something went wrong: we could not find the newly created playtest 
subreddit. Please playtest on a different subreddit using `devvit playtest
<your_subreddit>` instead.
```

**This is a known issue** where Devvit fails to automatically create the test subreddit.

**Solution: Create your own test subreddit**

1. **Create a new subreddit** at https://www.reddit.com/subreddits/create
   - Choose any name (e.g., `myapp_testing`, `devvit_test_123`)
   - Set it to Private or Restricted for testing

2. **Option A: Update `package.json` (Recommended)**
   ```json
   "scripts": {
     "dev:devvit": "devvit playtest r/YOUR_SUBREDDIT_NAME"
   }
   ```
   Then run:
   ```bash
   npm run dev
   ```

3. **Option B: Test directly with command**
   ```bash
   devvit playtest r/YOUR_SUBREDDIT_NAME
   ```
   Note: This only works for the current session and doesn't persist.

**Why this happens:**
- Reddit API fails to create auto-generated subreddit
- Subreddit name conflicts or already taken
- Rate limiting on subreddit creation
- Temporary Reddit API issues

### npm run dev Not Working

**Clear dependencies and reinstall:**
```bash
rm -rf node_modules package-lock.json
npm install
npm run dev
```

### Browser Issues

**Game not loading:**
- Hard refresh: Ctrl+Shift+R (Windows/Linux) or Cmd+Shift+R (Mac)
- Clear browser cache and cookies
- Try incognito/private browsing mode

**Mobile viewport problems:**
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
```

## 🆘 Getting Help

### Community Support

- **[r/redditdev](https://reddit.com/r/redditdev)**: Post questions with [Devvit] tag
- **[Devvit Discord](https://discord.gg/devvit)**: Real-time help from community

### When Asking for Help

Include:
- Node.js version: `node --version`
- Operating system
- Complete error messages
- Minimal code example that reproduces the issue
