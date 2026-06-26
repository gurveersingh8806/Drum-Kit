# Drum Kit

An interactive Drum Kit web application built with **HTML**, **CSS**, and **JavaScript**. Play different drum sounds with your mouse or keyboard and enjoy responsive visual animations.

## 🎸 [Play Now](https://gurveersingh8806.github.io/Drum-Kit/)

## Features

- **Dual Input Methods** - Play sounds by clicking buttons or pressing keyboard keys (W, A, S, D, J, K, L)
- **7 Unique Drum Sounds** - Tom drums, crash cymbal, kick bass, and snare
- **Visual Feedback** - Smooth animations and shadow effects on each drum hit
- **Responsive Design** - Clean, centered layout with styled drum buttons
- **Real-time Playback** - Instant audio response to user interactions

## How to Play

### Mouse Method
Click any of the seven drum buttons displayed on the screen.

### Keyboard Method
Press these keys to trigger sounds:
- **W** - Tom 1
- **A** - Tom 2
- **S** - Tom 3
- **D** - Tom 4
- **J** - Crash Cymbal
- **K** - Kick Bass
- **L** - Snare

Each press triggers a visual animation with shadow effects for immersive feedback.

## Project Structure

```
Drum-Kit/
├── index.html          # HTML structure with drum buttons
├── styles.css          # Styling with animations
├── index.js            # Event handling and sound logic
├── images/             # Drum button background images
│   ├── tom1.png
│   ├── tom2.png
│   ├── tom3.png
│   ├── tom4.png
│   ├── crash.png
│   ├── kick.png
│   └── snare.png
├── sounds/             # Audio files
│   ├── tom-1.mp3
│   ├── tom-2.mp3
│   ├── tom-3.mp3
│   ├── tom-4.mp3
│   ├── crash.mp3
│   ├── kick-bass.mp3
│   └── snare.mp3
└── README.md
```

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No additional dependencies required

### Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/gurveersingh8806/Drum-Kit.git
   cd Drum-Kit
   ```

2. **Open in browser:**
   - Simply open `index.html` in your web browser
   - Or use a local server:
     ```bash
     python -m http.server 8000
     # Then visit http://localhost:8000
     ```

3. **Start playing!**
   - Click buttons or press keyboard keys to play drum sounds

## Technical Highlights

- **DOM Manipulation** - Dynamic element selection and class management
- **Event Listeners** - Handles both `click` and `keydown` events
- **Audio API** - HTML5 Audio element for sound playback
- **CSS Animations** - Smooth transitions and visual feedback with `.pressed` class
- **Switch Statements** - Efficient sound mapping logic

## Visual Design

- **Color Scheme** - Dark background (#283149) with vibrant pink accents (#DA0463)
- **Typography** - Arvo font for bold, modern appearance
- **Button Styling** - 150x150px square buttons with borders and hover effects
- **Animations** - 100ms opacity and shadow effects on press

## Code Architecture

### Key Functions

**`makeSound(key)`**
- Maps keyboard/button input to audio files
- Creates and plays Audio objects based on the key pressed

**`addAnimation(event)`**
- Applies `.pressed` class to the corresponding button
- Removes class after 100ms for animation effect

**Event Listeners**
- Button clicks trigger `makeSound()` and `addAnimation()`
- Keyboard events trigger the same functions based on key press

## Learning Outcomes

This project reinforced understanding of:
- DOM traversal and manipulation
- Event handling (click and keyboard)
- JavaScript functions and switch statements
- Audio playback with HTML5 API
- CSS animations and transitions
- Responsive web design basics

## Future Enhancements

- Audio object pooling for better performance
- Input validation for keyboard events
- Mobile touch support
- Recording and playback functionality
- Different drum kits/themes
- Volume and tempo controls
- Accessibility improvements (ARIA labels)
- Responsive layout for mobile devices

## Contributing

Feel free to fork this project and submit pull requests for any improvements!

## License

This project is open source and available under the MIT License.

## Author

**Gurveer Singh** - [GitHub Profile](https://github.com/gurveersingh8806)
