<div align="center">

# BuilderAI Mobile starter

### An AI agent builder for iPhone and Android, with its own server.

The starter repo for **BuilderAI Mobile + Server from Scratch**, a free course on YouTube. You build a phone app
with Expo and React Native, and the NestJS API behind it: sign-in with email codes, a visual agent builder,
streaming chat with Claude, run history, Stripe plans and credits, then Docker and EAS builds.

**[📝 React B D on Medium](https://medium.com/@reactbd)** · **[🌐 reactbd.com](https://reactbd.com)**

</div>

---

## What's in this repo

A read me and the app's images, the files that can't be typed:

| File | What it is |
| --- | --- |
| `assets/images/icon.png` | the app icon |
| `assets/images/splash-icon.png` | the splash screen picture |
| `assets/images/favicon.png` | the web favicon |
| `assets/images/android-icon-background.png` | the Android adaptive icon's background layer |
| `assets/images/android-icon-foreground.png` | its foreground layer |
| `assets/images/android-icon-monochrome.png` | its monochrome layer (themed icons) |

## How to use it

Clone it, and the clone is your project folder:

```bash
git clone https://github.com/noorjsdivs/builder-ai-mobile-starter.git
```

Or, in VS Code: Welcome → **Clone Git Repository**, paste the address, pick a folder and open it.

The course then makes both projects inside it, the official way:

- `server/` with `nest new server --strict --skip-git` (the folder already is a repository)
- `mobile/` with `npx create-expo-app@latest mobile`, which copies these images in with
  `cp ../assets/images/*.png assets/images/`

## Keep your keys out of git

The server's settings live in `server/.env`, which `.gitignore` keeps out of the repository. Commit `.env.example`
with empty values instead, and never put a key in the app: everything secret stays on the server.
