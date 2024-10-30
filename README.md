# Hand Gesture-Controlled Keyboard Emulator

A Python-based project enabling keyboard control through hand gestures, powered by OpenCV and Mediapipe. This tool provides a hands-free interface, interpreting hand gestures captured via a webcam and emulating corresponding keyboard commands in real time.

## Overview

This project utilizes computer vision to track hand gestures, making it possible to control keyboard actions without physically pressing keys. The system captures gestures using Mediapipe's hand tracking module and maps them to keyboard inputs through Windows API calls, ideal for hands-free applications.

## Features

- **Real-Time Gesture Recognition**: Recognizes hand positions and gestures using Mediapipe's hand landmark detection.
- **Keyboard Emulation**: Maps gestures to specific keyboard keys (up, down, left, right) for hands-free control.
- **Customizable and Extensible**: Easily modify gesture mappings or add additional controls as needed.

## Installation

### Prerequisites

- **Python 3.6+**
- Required Python libraries: OpenCV, Mediapipe, and NumPy
- **Windows OS** (for keyboard emulation via `ctypes`)

## Controls
The system maps specific hand gestures to directional keyboard inputs:

 - Five Fingers Extended (Right Hand): Emulates the Right arrow key.
 - Five Fingers Extended (Left Hand): Emulates the Left arrow key.
 - One Finger Extended: Emulates the up arrow key.
 - No Fingers Extended (Closed Palm): Emulates the down arrow key.

## Limitations
 - Platform Dependency: Designed specifically for Windows, due to the ctypes dependency for keyboard emulation.
 - Lighting Sensitivity: Gesture detection may be less accurate in low-light conditions.

## Clone the repository
   ```bash
   git clone https://github.com/yourusername/hand-gesture-keyboard-emulator.git
   cd hand-gesture-keyboard-emulator
