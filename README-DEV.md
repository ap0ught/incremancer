# Incremancer - Development Environment

A development environment setup for the Incremancer idle necromancer game with debugging capabilities.

## 🚀 Quick Start

### Option 1: GitHub Codespaces (Recommended)
1. Click "Create codespace" in the GitHub repository
2. Wait for the environment to set up automatically
3. Run `npm run dev` to start the development server
4. Open the forwarded port (8080) to access the game

### Option 2: Local Development

#### Prerequisites
- Node.js 12+ 
- Git
- VS Code (recommended)

#### Setup
```bash
# Clone the repository
git clone https://github.com/ap0ught/incremancer.git
cd incremancer

# Install dependencies
npm install

# Start development server
npm run dev
```

## 🛠️ Development Scripts

- `npm run dev` - Start development server with live reload
- `npm run start` - Alias for dev
- `npm run debug` - Start server with verbose logging
- `npm run serve` - Simple Python HTTP server (fallback)

## 🐛 Debugging

### VS Code Debugging Setup

1. Open the project in VS Code using the workspace file:
   ```bash
   code incremancer.code-workspace
   ```

2. Install recommended extensions when prompted

3. Use the following debug configurations:
   - **Launch Chrome with Debugging** - Opens Chrome with DevTools
   - **Attach to Chrome** - Attaches to existing Chrome instance
   - **Launch with Live Server** - Starts live server and Chrome

### Browser DevTools

The development server automatically opens Chrome DevTools for debugging:
- **Console** - View logs, errors, and execute JavaScript
- **Sources** - Set breakpoints in source code
- **Network** - Monitor network requests
- **Application** - Inspect local storage, session data

### Debugging Features

1. **Console Logging**: Enhanced console output for game events
2. **Error Tracking**: Automatic error reporting in development
3. **Live Reload**: Automatic page refresh on file changes
4. **Source Maps**: Original source code visibility in debugger

## 📁 Project Structure

```
incremancer/
├── .devcontainer/          # GitHub Codespaces configuration
├── .vscode/               # VS Code settings (auto-generated)
├── dist/                  # Compiled game bundle
│   └── bundle.js         # Main game code
├── images/               # Game assets
├── js/                   # External libraries
├── sprites/              # Sprite configurations
├── templates/            # HTML templates
├── index.html           # Main game page
├── zombiemancer.css     # Game styles
├── package.json         # Development dependencies
└── incremancer.code-workspace # VS Code workspace
```

## 🎮 Game Development

### Key Files
- `index.html` - Main game entry point
- `dist/bundle.js` - Compiled game logic
- `templates/*.html` - Game UI components
- `zombiemancer.css` - Game styling

### Technologies
- **AngularJS** - Frontend framework
- **PixiJS** - 2D graphics rendering
- **HTML5** - Canvas and audio

## 🔧 Development Tips

1. **Live Reload**: Files are watched automatically, changes refresh the browser
2. **Console Debugging**: Use `console.log()` for debugging game state
3. **Network Monitoring**: Watch for asset loading issues in Network tab
4. **Performance**: Use DevTools Performance tab to profile game loops
5. **Mobile Testing**: Use Chrome DevTools device emulation

## 🚨 Troubleshooting

### Common Issues

**Port 8080 already in use:**
```bash
# Kill existing server
pkill -f live-server
# Or use different port
npx live-server --port=8081
```

**Chrome not opening with debug tools:**
```bash
# Manually open Chrome with debugging
google-chrome --remote-debugging-port=9222 --auto-open-devtools-for-tabs
```

**Live reload not working:**
- Check if files are being watched correctly
- Ensure browser allows local file access
- Try hard refresh (Ctrl+F5)

### Debug Console Commands

```javascript
// Access game state (if available globally)
window.Incremancer

// Monitor AngularJS scope
angular.element(document.body).scope()

// Check PixiJS renderer
window.PIXI
```

## 📝 Development Workflow

1. **Start development server**: `npm run dev`
2. **Open debugger**: Use VS Code launch configuration
3. **Make changes**: Edit files and see live updates
4. **Debug**: Set breakpoints and inspect variables
5. **Test**: Verify functionality across different browsers

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Use the development environment for testing
4. Submit a pull request with detailed description

---

**Happy coding!** 🧟‍♂️⚡