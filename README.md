# Site Sleuth

A Chrome extension that lets you search your browsing history using natural language queries powered by Google's Gemini AI.

## What it does

Ever visited a website but can't remember the URL? Site Sleuth helps you find it by describing what you're looking for in plain English.

**Examples:**
- "That Reddit post about Python best practices"
- "YouTube video I watched about cooking pasta"
- "GitHub repo with React components"
- "Article about machine learning I read last week"

## Features

- Natural language search through your browser history
- Smart filtering by platform (Reddit, YouTube, GitHub, etc.)
- AI-powered ranking of results using Gemini
- Google Search grounding for enhanced analysis
- Works with the last 30 days of browsing history

## Installation

1. Clone this repository
2. Open Chrome and go to `chrome://extensions/`
3. Enable "Developer mode" (toggle in top right)
4. Click "Load unpacked" and select this folder
5. Click the extension icon in your toolbar

## Setup

On first use, you'll be prompted for a Gemini API key:

1. Go to [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create a new API key
3. Paste it when prompted

The key is stored locally in Chrome's sync storage.

## Usage

1. Click the Site Sleuth icon in your browser toolbar
2. Type a description of what you're looking for
3. Press Enter
4. Browse the results with explanations of why each page matches

## Project Structure

```
src/
  index.html    - Extension popup UI
  main.js       - Core application logic
  style.css     - Styling
  background.js - Service worker for history access
manifest.json   - Chrome extension configuration
```

## Privacy

- All processing happens locally in your browser
- Your browsing history is never sent to external servers (only to Gemini API for analysis)
- API key is stored in Chrome's sync storage

## Requirements

- Google Chrome (or Chromium-based browser)
- Gemini API key (free tier available)
