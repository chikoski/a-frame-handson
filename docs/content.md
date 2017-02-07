# A-Frame hands-on 

2017/01/29 Yoichi Sugii 

 (Original document is written in Japanese. Translated by N.Shimizu)

---

## Acknowledgement

This hands-on event targets people who are familiar with JavaScript progarmming and writing HTML documents

---

## Prerequisites

- PC / Mac
- Internet connectivity
- Software installation
  - [Firefox Nightly](https://www.mozilla.org/firefox/channel/desktop/#nightly) or [WebVR enabled Chromium](https://webvr.info/get-chrome/)
  - [Node.js](https://nodejs.org/)
  - Text editor, such as [Visual Studio Code](https://code.visualstudio.com/), [Atom](https://atom.io/) and [SublimeText](https://www.sublimetext.com/)

----

## "A-Frame Boilarplate" setup

1. Download "[A-Frame Boilarplate](https://github.com/aframevr/aframe-boilerplate)" and extract it
2. Open your terminal and go to the extracted folder
3. Run `npm install` to insall dependencies
4. Start a web server with this command: `npm start`

Note: hit `Ctrl-c` to terminate the web server. Please check README.md for details.

---

## Table of contents

- Introduction of A-Frame
- 3D graphics fundamentals 
- source code layout / entities
- DOM manipulation / component system / additonal component installation
- Defining a component / debugging

---

## WebVR

- A technology to make the web first class VR platform
- WebVR API,
   - Core API 
   - Providing abstruction of VR HMDs / sensors
- Mozilla, Google, Microsoft, Oculus, Samsong, etc are eager to support WebVR
- Firefox Nightly and custom build Chromium support this API for now

----

### A-Frame

- A component based WebVR framework
   - Using Three.js to handle 3D graphics
   - Entity-Component-System
- Resources: 
   - [Web site](https://aframe.io/) / [GitHub](https://github.com/aframevr/aframe) / [Document](https://aframe.io/docs/)
   - [A list of awesome resources](https://github.com/aframevr/awesome-aframe)

---

## 3D graphics fundamentals

----

### Position / direction

- Positon is represented by triplets of numbers
   - X-axis / Y-axis / Z-axis
   - Right-handed Cartesian coordinate system
   - Unit: m (meter) 
   - e.g. set 1.6 to Y coordinate to put entity to the average hight of human eye
- Direction is represented as degree of rotation

----

### Terminologies

- Scene: 3D space consists of camera, light, and entity
- Camera
- Light
- Entity: Objects in a 3D space

----

### PerspectiveCamera

- Default camera of A-Frame
- Parameters
  - FOV: field of vision
  - FAR: thresold for far cliping
  - NEAR: threshold for near cliping
  - ASPECT: width / height

----

### Light

- Directional light
- Ambient light
- Point light
- Spot light

