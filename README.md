# 🚀 WebRTC Video Calling & Media Processing Full-Stack Project

This is an independently developed full-stack project that integrates high-quality WebRTC video calling, signaling exchange, device management, and media processing (recording, format conversion) functionalities. The project clearly demonstrates complete skills from frontend UI interaction, backend signaling coordination to media processing.

## 📁 Project Architecture & Repository Links

This project consists of two core components. Click the links below to view detailed code and documentation for each part:

| Service Name | Technology Stack | Repository Link | Core Features |
| :--- | :--- | :--- | :--- |
| **Signaling & Media Backend Service** | Node.js, Express, Socket.io, FFmpeg | [webrtc_nodejs](https://github.com/lauchiwai/webrtc_nodejs) | WebRTC signaling exchange (Offer/Answer/ICE), room management, WebM to MP4 video conversion |
| **Frontend Video Application** | React, TypeScript, Zustand, Ant Design | [webrtc_react](https://github.com/lauchiwai/webrtc_react) | Video calling interface, device management, remote screen recording & screenshots, real-time connection status monitoring |

## 🛠️ Technical Highlights

### 🔐 Communication & Negotiation
- **Complete WebRTC Signaling Flow**: Implemented a stable signaling server based on Socket.io, reliably handling the exchange and negotiation of `offer`, `answer`, and `ICE candidate`.
- **Room Management Mechanism**: Implemented a simple and efficient room number system, allowing users to easily join the same call session.

### 🎥 Media & Device Control
- **Dynamic Device Management**: The frontend can dynamically detect, enumerate, and switch audio input devices, providing a seamless device switching experience.
- **Media Track Control**: Independently control the enable/disable of audio and video tracks, implementing mute, camera off, and other functions.
- **Advanced Media Processing**: Implemented `MediaRecorder API` for remote screen recording with multi-format output, and provided real-time screenshot functionality.

### ⚙️ Backend Media Processing
- **FFmpeg Integration**: The backend service integrates FFmpeg, providing the service to convert WebM format videos recorded by the frontend to the more universal MP4 format.
- **RESTful API Design**: Provides clear API endpoints (`/convert`) for submitting conversion tasks and downloading converted files.

### 🚀 Frontend Architecture & Experience
- **Modern Frontend Stack**: Built type-safe components using React and TypeScript, using Zustand for clear reactive state management.
- **High-Quality User Interface**: Developed based on the Ant Design component library, providing a professional and intuitive user operation interface.
- **Real-time Status Feedback**: Clearly displays connection status, recording timers, and other information on the UI to ensure user awareness.
