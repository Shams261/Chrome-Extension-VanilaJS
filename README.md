# Leads Tracker Chrome Extension

A simple Chrome extension for tracking and managing website URLs/leads while browsing.

## Features

- **Save URLs manually** - Type and save any URL
- **Save current tab** - Quickly save the URL of your active browser tab
- **Persistent storage** - All leads are saved in browser localStorage
- **Quick access** - View all saved leads as clickable links
- **Easy cleanup** - Double-click to delete all saved leads

## Installation

1. Clone or download this repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Build the extension:
   ```bash
   npm run build
   ```
4. Load the extension in Chrome:
   - Open Chrome and navigate to `chrome://extensions/`
   - Enable "Developer mode" (toggle in top right corner)
   - Click "Load unpacked"
   - Select the `dist` folder created after building

## Usage

1. Click the extension icon in your Chrome toolbar
2. The popup will display with three options:
   - **Text input + SAVE INPUT**: Manually enter and save any URL
   - **SAVE TAB**: Save the URL of your currently active tab
   - **DELETE ALL**: Double-click to clear all saved leads
3. All saved leads appear as clickable links below the buttons

## Development

- **Start dev server**: `npm run dev`
- **Build for production**: `npm run build`
- **Preview build**: `npm run preview`

## Tech Stack

- Vanilla JavaScript
- HTML/CSS
- Chrome Extension Manifest V3
- Vite (build tool)
- localStorage for data persistence

## Permissions

- `tabs` - Required to access current tab URL when using "SAVE TAB" feature