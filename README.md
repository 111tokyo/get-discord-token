# 📜 get-discord-token
A simple guid on how to easily retrieve your Discord token using a web browser.
> [!WARNING]
> Unauthorized use of a Discord token may violate Discord's Terms of Service and result in account suspension. Use this information responsibly.

---

## ❓ How to Retrieve Your Discord Token?

### 1. Open Discord in a Browser
Log in to your Discord account through a web browser (Google Chrome, Firefox, Edge, etc.).

### 2. Open the Browser Console
- Windows/Linux: **Ctrl + Shift + I** then go to the **Console** tab
- Mac: **Cmd + Option + I** then go to the **Console** tab

### 3. Run the Following Script in the Console
```javascript
window.webpackChunkdiscord_app.push([
  [Math.random()],
  {},
  req => {
    if (!req.c) return;
    for (const m of Object.keys(req.c)
      .map(x => req.c[x].exports)
      .filter(x => x)) {
      if (m.default && m.default.getToken !== undefined) {
        return copy(m.default.getToken());
      }
      if (m.getToken !== undefined) {
        return copy(m.getToken());
      }
    }
  },
]);
window.webpackChunkdiscord_app.pop();
console.log('%cSuccess!', 'font-size: 50px');
console.log(`%cYour token has been copied to the clipboard!`, 'font-size: 16px');
```

### 4. Retrieve Your Token
The token is now copied to your clipboard. You can paste it (**Ctrl + V** or **Cmd + V**) wherever you need.

---

> [!CAUTION]
> - Never share your Discord token with anyone.
> - A token grants full access to your account, including messages, servers, and settings.
> - If your token is compromised, change your password immediately to generate a new one.

**This guide is intended for learning and understanding how Discord works. Any malicious use is strictly prohibited.**

