# Troubleshooting Guide

Common issues and solutions for template-based Devvit game development.

## 🖥️ Development Server Issues

### npm run dev Not Working

**Clear dependencies and reinstall:**
```bash
rm -rf node_modules package-lock.json
npm install
npm run dev
```

**Port already in use:**
```bash
# Find and kill process using the port
lsof -ti:3000 | xargs kill -9
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

- **r/redditdev**: Post questions with [Devvit] tag
- **Devvit Discord**: Real-time help from community

### When Asking for Help

Include:
- Node.js version: `node --version`
- Operating system
- Complete error messages
- Minimal code example that reproduces the issue
