# Replit Agent Guide

## Overview

This is a romantic/love-themed interactive web page ("فاجأة حب" - "Love Surprise" in Arabic). It features an animated envelope that users can interact with, likely revealing a love message or surprise animation. The project is a single-page, client-side web application with all code consolidated into a single `index.html` file. It's designed as a gift/greeting card-style experience with Arabic text support (RTL layout).

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Single-file approach**: All HTML, CSS, and JavaScript are consolidated into `index.html`. The `script.js` and `style.css` files exist but are empty placeholders with comments indicating the code was moved to the HTML file "for simplicity in fast mode."
- **No build tools or frameworks**: This is a vanilla HTML/CSS/JavaScript project with no bundler, no framework, and no package manager.
- **RTL Layout**: The page is configured for right-to-left (Arabic) text direction (`dir="rtl"`, `lang="ar"`).
- **CSS Custom Properties**: Uses CSS variables for theming (colors like primary red, soft pink, white, and text color).
- **Google Fonts**: Uses 'Amiri' (Arabic serif font) and 'Dancing Script' (decorative Latin script font) loaded via Google Fonts CDN.
- **Responsive design considerations**: Uses viewport meta tag and percentage-based sizing for the container.

### Design Patterns
- The envelope interaction pattern suggests a reveal/animation UX where clicking an envelope triggers content display.
- CSS transitions are used for smooth visual effects (background color transitions, transform on hover).
- The z-index layering suggests multiple visual layers (background effects, envelope, content).

### Key Decisions
- **Problem**: Need a simple, shareable love greeting page.
- **Solution**: Single HTML file with everything inlined — easy to share, deploy, or send as a file.
- **Pros**: Zero dependencies, no build step, instant deployment, easy to modify.
- **Cons**: Harder to maintain as complexity grows, no code splitting or modularity.

## External Dependencies

- **Google Fonts CDN**: Loads 'Amiri' and 'Dancing Script' font families. Requires internet connection for fonts to render properly.
- **No backend services**: This is a purely static, client-side application.
- **No database**: No data persistence needed.
- **No APIs**: No external API integrations.
- **No npm packages**: No server-side or build dependencies.

If expanding this project, consider keeping the single-page simplicity but potentially splitting CSS and JS back into their respective files (`style.css`, `script.js`) for better maintainability.