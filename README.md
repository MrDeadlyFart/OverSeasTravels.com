{
  "manifest_version": 2,
  "name": "Text Highlighter",
  "version": "1.0",
  "description": "Highlights specified text on a webpage.",
  "permissions": [
    "activeTab"
  ],
  "background": {
    "scripts": ["background.js"]
  },
  "content_scripts": [
    {
      "matches": ["<all_urls>"],
      "js": ["content.js"]
    }
  ],
  "browser_action": {
    "default_icon": "icon.png",
    "default_popup": "popup.html"
  }
}
