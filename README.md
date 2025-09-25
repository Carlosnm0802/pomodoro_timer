# Pomodoro Timer

A modern and fully customizable Pomodoro Timer built with vanilla JavaScript. Designed to enhance productivity through focused work sessions and strategic breaks.

## Live Demo

[View Demo](https://tu-usuario.github.io/pomodoro-timer) *(Update with your GitHub Pages link)*

## Features

### Core Functionality
- Complete Pomodoro technique implementation with automatic work/break cycles
- Four configurable timing presets:
  - **Classic**: 25 min work / 5 min break / 15 min long break
  - **Short**: 15 min work / 3 min break / 10 min long break
  - **Extended**: 45 min work / 10 min break / 30 min long break
  - **Custom**: User-defined intervals (1-120 minutes)

### User Interface
- Clean, modern design with glassmorphism effects
- Fully responsive layout for desktop and mobile devices
- Visual state indicators with color-coded work and break periods
- Smooth transitions and hover effects
- Real-time progress display in browser tab title

### Data Management
- Session tracking with completed cycles counter
- Persistent configuration storage using localStorage
- Automatic settings restoration between sessions
- Optional auto-start functionality between intervals

### Notifications
- Visual notifications for session completion
- Browser audio notifications using Web Audio API
- Customizable alert messages for different session types

## Technical Implementation

### Technologies Used
- HTML5 with semantic markup
- CSS3 featuring Flexbox, Grid, and modern styling techniques
- JavaScript ES6+ with object-oriented programming principles
- Browser APIs: LocalStorage, Web Audio API, Notifications API

### Architecture
The application follows a modular class-based structure:

```javascript
class PomodoroTimer {
  constructor() {
    // Configuration management
    // State tracking
    // DOM element initialization
  }
  
  // Timer control methods
  start() { /* ... */ }
  pause() { /* ... */ }
  reset() { /* ... */ }
  
  // Configuration methods
  saveSettings() { /* ... */ }
  loadSettings() { /* ... */ }
  
  // UI update methods
  updateDisplay() { /* ... */ }
  showNotification() { /* ... */ }
}
```

## Installation

### Option 1: Clone Repository
```bash
git clone https://github.com/your-username/pomodoro-timer.git
cd pomodoro-timer
```

### Option 2: Download ZIP
1. Download the ZIP file from the GitHub repository
2. Extract files to your desired directory
3. Open `index.html` in your web browser

## Usage

### Getting Started
1. Open the application in your web browser
2. Click the settings icon to configure timer intervals
3. Select a preset or create custom timing configuration
4. Click "Start" to begin your first Pomodoro session

### Workflow
The Pomodoro Technique follows a structured workflow:
1. Work for the configured time period (default 25 minutes)
2. Take a short break when the session completes
3. Repeat the work-break cycle
4. After every fourth work session, take a longer break

### Configuration Options
Access the settings panel to customize:
- Work session duration
- Short break duration
- Long break duration
- Choose from preset configurations or create custom timings

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

The application uses modern JavaScript features and Web APIs that require current browser versions.

## Performance Considerations

- Minimal resource usage with vanilla JavaScript implementation
- Efficient timer management using `setInterval`
- Optimized DOM updates to prevent unnecessary reflows
- Lightweight design with no external dependencies

## Customization

### Styling
Modify the CSS variables within the `<style>` section to customize appearance:

```css
/* Work session styling */
.timer-circle.work {
    border-color: #ff6b6b;
    box-shadow: 0 0 20px rgba(255, 107, 107, 0.5);
}

/* Break session styling */
.timer-circle.break {
    border-color: #4ecdc4;
    box-shadow: 0 0 20px rgba(78, 205, 196, 0.5);
}
```

### Audio Notifications
Customize notification sounds by modifying the `playNotificationSound()` method:

```javascript
oscillator.frequency.value = 800; // Frequency in Hz
gainNode.gain.value = 0.1;        // Volume level
```

## Deployment

### GitHub Pages
1. Push your code to a GitHub repository
2. Navigate to repository Settings > Pages
3. Select "Deploy from a branch" and choose main branch
4. Access your timer at `https://your-username.github.io/pomodoro-timer`

### Alternative Hosting
- **Netlify**: Drag and drop deployment at netlify.com
- **Vercel**: Connect repository at vercel.com
- **Local Server**: Use any static file server for local development

## Development

### Project Structure
```
pomodoro-timer/
├── index.html          # Main application file
├── README.md           # Project documentation
└── LICENSE            # License file (optional)
```

### Code Quality
- Consistent ES6+ JavaScript syntax
- Semantic HTML5 structure
- Modern CSS with logical organization
- Comprehensive error handling
- Clear variable and method naming

