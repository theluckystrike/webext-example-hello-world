# Hello World Chrome Extension

The simplest possible Chrome extension - a "hello world" example for learning Chrome extension development.

## What It Does

This extension demonstrates the minimum required files for a Chrome extension:
- A `manifest.json` file that declares the extension's metadata
- Icon files for the extension

When loaded in Chrome, it appears in the extensions list but doesn't add any functionality - it's the starting point for building more complex extensions.

## How to Install

1. Open Chrome and navigate to `chrome://extensions/`
2. Enable "Developer mode" in the top right corner
3. Click "Load unpacked"
4. Select the `src` folder of this extension

## Project Structure

```
webext-example-hello-world/
├── src/
│   ├── manifest.json    # Extension configuration
│   └── icons/          # Extension icons
├── screenshots/        # Screenshots of the extension
├── README.md           # This file
├── LEARN.md            # Learning guide for this pattern
└── package.json        # Package configuration
```

## Learning Path

This is the first example in our Chrome extension learning path:

1. **Hello World** (you are here) - Minimal extension
2. [Popup Basic](../webext-example-popup-basic) - Add a popup UI
3. [Content Script](../webext-example-content-script-basic) - Interact with web pages
4. [Background Service Worker](../webext-example-background-basic) - Background processing
5. [Options Page](../webext-example-options-page) - Add settings

## Related Patterns

- [webext-options-page](https://github.com/zovo/webext-options-page) - Full options page framework
- [webext-popup-router](https://github.com/zovo/webext-popup-router) - Router for popup UIs

## License

MIT
