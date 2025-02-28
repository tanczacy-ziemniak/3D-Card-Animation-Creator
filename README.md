# 3D Card Animation Creator

A web application that allows users to create and record custom 3D card animations by uploading front and back images.

## Demo

![Alt Text](https://github.com/ziemniak-kr/3D-Card-Animation-Creator/blob/main/demo/card-animation-720p.gif)

## Features

- Upload custom images for the front and back of the card
- Preview the 3D rotating card animation
- Record the animation as a video
- Download the recorded animation as a WebM video file
- Responsive design that works on desktop and mobile devices


## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge recommended for recording functionality)
- Local web server (optional for local development)

### Installation

1. Clone the repository or download all the files from the repository:
   ```
   git clone https://github.com/ziemniak-kr/3D-Card-Animation-Creator.git
   ```

2. Navigate to the project directory:
   ```
   cd 3d-card-animation-creator
   ```

3. Open `index.html` in your web browser or serve it using a local web server.

## How to Use

1. **Upload Images**: 
   - Click on the "Front Image" and "Back Image" upload buttons to select images from your device.
   - Both images will be displayed in their respective preview areas.

2. **Preview Animation**: 
   - Once both images are uploaded, click the "Preview Animation" button to see how your card animation will look.

3. **Record Animation**: 
   - Click the "Record Animation" button to capture the animation as a video.
   - The recording will automatically stop after the animation completes (approximately 2 seconds).

4. **Download Video**: 
   - After recording, a "Download Video" button will appear.
   - Click it to save the animation as a WebM video file to your device.

## Customization

### Changing the Background Color

To change the video background color:

1. Open the `script.js` file
2. Find the `initScene()` function
3. Locate the line: `scene.background = new THREE.Color(0xf0f0f0);`
4. Change the hex color code `0xf0f0f0` to your desired color
   - For example, for a blue background: `scene.background = new THREE.Color(0x0088ff);`
   - For a black background: `scene.background = new THREE.Color(0x000000);`

### Other Customizations

- **Animation Duration**: To change how long the animation takes, modify the `animationDuration` variable (in milliseconds) near the top of the script.js file.
- **Card Dimensions**: To alter the card size and corner radius, find the `createCard()` function and adjust the `width`, `height`, and `radius` variables.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Three.js - For 3D rendering
- RecordRTC - For video recording

## Browser Compatibility

- The app works in all modern browsers
- Recording functionality works best in Chrome, Firefox, and Edge
- Safari has limited support for the recording feature

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Three.js for the 3D rendering library
- RecordRTC for the video recording functionality
