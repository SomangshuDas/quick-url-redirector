# Quick URL Redirector

Quick URL Redirector is a lightweight, static redirection project built on **GitHub Pages**.
It automatically redirects visitors to a destination URL defined in a plain text file (`url.txt`) without exposing the final target to the end user.

This project works entirely on the client side and requires **no backend, no server configuration, and no paid services**.

---

## Overview

Many URLs—whether temporary or permanent—are difficult to manage or shorten using free URL shortening services. This includes, but is not limited to, dynamically generated links such as tunnels or proxy endpoints.

URL Redirector provides a clean and reliable redirection layer using GitHub Pages.
The generated GitHub Pages link can optionally be shortened further using any standard URL shortener.

In addition to dynamic URLs, this project can also be used for **general-purpose redirection**, such as websites, documentation links, campaigns, or service endpoints.

---

## Key Features

- Easy to duplicate and reuse
- Static, client-side URL redirection
- Compatible with all modern browsers
- No backend, database, or APIs required
- Destination URL stored in a simple text file
- Hosted on GitHub Pages for stability and availability
- Suitable for tunnels, proxies, services, websites, and standard URLs

---

## Redirection Flow

```
User → Shared Link → GitHub Pages → Destination URL
```

1. The user opens the shared link
2. GitHub Pages serves the redirect page
3. The page reads the destination from `url.txt`
4. The browser redirects automatically

The destination URL is not visible before redirection.

---

## Repository Structure

```
/
├── LICENSE         # Project license
├── README.md       # Documentation
├── favicon.ico     # Site favicon
├── index.html      # Redirect logic
└── url.txt         # Destination URL
```

---

## Setup Instructions

### 1. Create the Repository
- Fork this repository **or**
- Duplicate it under your GitHub account

Ensure the repository is set to **Public** to enable GitHub Pages.

---

### 2. Configure the Redirect URL
Edit `url.txt` and insert your destination URL:

```
https://example.com
```

Rules:
- No extra text
- One URL only
- No blank lines or trailing spaces

---

### 3. Enable GitHub Pages
1. Go to **Settings → Pages**
2. Configure:
   - Branch: `main`
   - Folder: `/ (root)`
3. Save changes

GitHub will generate a Pages URL similar to:

```
https://username.github.io/quick-url-redirector/
```

---

### 4. Optional: Shorten the Pages Link
For easier sharing:
1. Copy the GitHub Pages URL
2. Shorten it using any free URL shortening service
3. Share the shortened link

Users will be redirected transparently.

---

## Common Use Cases

- General URL redirection
- Tunnels, relays, and proxy URLs
- Campaign and distribution links
- Documentation and resource links
- Website or landing page forwarding
- Educational and testing environments
- Temporary or permanent service endpoints

---

## License

This project is released under the **MIT License**. You are free to use, modify, and redistribute it.
