# Learning: The Simplest Chrome Extension

## What is a Chrome Extension?

A Chrome extension is a small software program that customizes the Chrome browsing experience. Extensions are built using standard web technologies (HTML, CSS, JavaScript) and the Chrome Extensions API.

## Key Concept: Manifest V3

Chrome extensions use a `manifest.json` file to declare:
- Extension name, version, and description
- Permissions the extension needs
- Background scripts, content scripts, or popup UI
- Browser actions (toolbar icons, etc.)

This example uses **Manifest V3** (MV3), the current standard.

## The Absolute Minimum

A Chrome extension requires ONLY a `manifest.json` file. That's it! 

Here's the simplest possible manifest:

```json
{
  "manifest_version": 3,
  "name": "My Extension",
  "version": "1.0.0"
}
```

This is sufficient for Chrome to recognize and load the extension.

## Our Manifest Explained

```json
{
  "manifest_version": 3,     // MV3 is the current standard
  "name": "Hello World",     // Display name
  "version": "1.0.0",         // Semantic version
  "description": "The simplest possible Chrome extension",
  "icons": {                 // Optional but recommended
    "16": "icons/icon16.png",
    "48": "icons/icon48.png",
    "128": "icons/icon128.png"
  }
}
```

## Common Mistakes

1. **Wrong manifest version**: Must be `3` for new extensions (MV2 is deprecated)
2. **Missing required fields**: `name` and `version` are required
3. **Invalid JSON**: Use a JSON validator

## Next Steps

To make this extension do something, you would add:

1. **Popup**: Add a browser action with a popup HTML file
2. **Content Script**: Inject JavaScript into web pages
3. **Background Script**: Run code in the background

See the next examples in this learning path!

## Resources

- [Chrome Extensions Documentation](https://developer.chrome.com/docs/extensions/)
- [Manifest V3 Migration Guide](https://developer.chrome.com/docs/extensions/mv3/intro/)
- [Extension Best Practices](https://developer.chrome.com/docs/extensions/develop/best-practices)
