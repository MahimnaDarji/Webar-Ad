# AR Video Playback on Print Media

This project shows how a printed advertisement can trigger an interactive video overlay using WebAR. When a user scans the QR code, the browser opens an AR view, detects the printed artwork, and plays the video directly on the page through image tracking.

## Project Overview
Printed ads are static, and this setup turns them into interactive visuals without requiring an app. The system uses browser-based image tracking, so the video stays anchored to the physical page as long as the target image is visible.

This project includes:
- Image tracking using MindAR
- Stabilized video overlay aligned to the detected target
- Oversized projection for clearer visibility
- A complete AR workflow running entirely in the mobile browser

## Tech Stack
| Layer      | Tools Used                      |
|-----------|----------------------------------|
| AR Engine | A-Frame, MindAR Image Tracking   |
| Frontend  | HTML, JavaScript                 |
| Media     | MP4 video overlay                |
| Deploy    | GitHub Pages or static hosting   |

## Features Built

### Image Tracking
- Target detection powered by MindAR’s image tracking
- `.mind` file created from the same artwork used in the printed ad

### Stabilized Video Projection
- Oversized video plane for stronger on-page presence
- Pose-smoothing logic to reduce jitter and flicker
- Autoplay behavior with fallback for mobile restrictions

### Integrated Camera View
- Camera preview displayed behind the AR layer
- Video kept anchored to the physical page through continuous pose updates

## What Makes It Stand Out

### Browser-Based AR Experience
Runs directly in the browser after scanning the QR code. No apps or installations required.

### Stable Target Locking
Custom smoothing is applied on top of MindAR to stabilize the video against device movement or lighting changes.

### Simple Deployment
The entire experience can run from a static site. No server, backend, or external pipeline required.

### Print-Aligned Tracking Model
The artwork printed in the ad is the same artwork used to build the tracking model, ensuring reliable detection once deployed.

## Future Enhancements
- On-screen controls for mute, unmute, or replay
- Multi-target support for complex campaigns
- Better fallback handling for low-light conditions
- Optional branded loading screen before AR mode starts
