# Bodger

A product showcase page for Bodger, an iOS app — featuring an accurate iOS 26 "Liquid Glass" device frame rendered entirely in React with no build step.

## Overview

This site serves as a marketing and preview page for the Bodger iOS application. The centerpiece is a custom-built iOS 26 device frame component (`ios-frame.jsx`) that recreates Apple's Liquid Glass design system using pure React and CSS — including the dynamic status bar, frosted-glass navigation pills, signal/wifi/battery icon reproductions, and the Dynamic Island. The page loads React and Babel directly from CDN, requiring no bundler or local toolchain.

## Tech Stack

- **React 18** (via CDN) — component-based UI with no build toolchain
- **Babel Standalone** — in-browser JSX compilation
- **Custom iOS 26 components** — `IOSDevice`, `IOSStatusBar`, `IOSNavBar`, `IOSGlassPill`, `IOSList`, `IOSListRow`, `IOSKeyboard`

## File Structure

| File | Purpose |
|------|---------|
| `index.html` | Page shell with embedded CSS, root mount, and CDN script tags |
| `ios-frame.jsx` | Reusable iOS 26 Liquid Glass device frame component library |

## Running Locally

No build step needed — open `index.html` in a browser, or serve it with any static file server:

```bash
npx serve .
```
