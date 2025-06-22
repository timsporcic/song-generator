# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an AI Song Generator Quiz - a static web application that helps users create prompts for AI music generation platforms (Suno, Udio, etc.). The project consists of two standalone HTML files with embedded CSS and JavaScript.

## Development Setup

### Local Development
Since this is a static site, you can either:
1. Open HTML files directly in a browser
2. Use a local server:
   ```bash
   npm install -g http-server
   http-server
   ```

### File Structure
- `index.html` - Original minimal design version
- `claude.html` - Enhanced version with gradient UI
- Both files are self-contained with inline CSS and JavaScript

## Architecture Notes

### Key Implementation Details
- **Pure vanilla JavaScript** - No frameworks or libraries
- **Self-contained HTML files** - All CSS and JS are inline
- **No build process** - Direct editing of HTML files
- **Client-side only** - No server interaction
- **Mobile-responsive** - Both versions adapt to screen sizes

### Core Functionality
The quiz collects 8 user inputs:
1. Genre (predefined options)
2. Mood/emotion (text input)
3. Subject matter (text input)
4. Theme/message (text input)
5. Setting/backdrop (text input)
6. Narrative perspective (predefined options)
7. Specific imagery (text input)
8. Chorus style (predefined options)

Results are formatted into a prompt and can be copied to clipboard.

## Common Tasks

### Adding New Genre Options
Look for the genre question section in either HTML file and add new radio button options to the existing list.

### Modifying Question Flow
Each question is in a separate `<div class="question">` block. The JavaScript handles showing/hiding questions based on the `currentQuestion` variable.

### Styling Changes
- `index.html`: Minimal CSS with Inter font, uses CSS variables for theming
- `claude.html`: Enhanced with gradients, animations, and Pacifico font for headers

## Testing Approach
Manual testing only - open in browser and verify:
1. All questions display correctly
2. Navigation between questions works
3. Validation prevents empty submissions
4. Results generate properly
5. Copy to clipboard functionality works
6. Responsive design on different screen sizes