# Camera Application

A feature-rich iOS camera application built with Swift that enables users to capture, edit, and save media content. This app provides an intuitive interface for photo and video capture with real-time filtering capabilities.

## 📋 Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Architecture](#architecture)
- [Testing](#testing)
- [Permissions](#permissions)
- [Known Limitations](#known-limitations)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

The Camera Application includes the following capabilities:

1. **Media Capture**
   - Capture photos directly from the device camera
   - Record videos with a maximum duration of 15 seconds
   - Pick existing media from the device photo gallery

2. **Media Display**
   - Preview selected images on the screen
   - View captured or selected videos within the app
   - Real-time media rendering

3. **Media Editing**
   - Apply image filters to photos before saving
   - Transform media with visual effects

4. **Media Management**
   - Save edited images directly to the device gallery
   - Save recorded videos to the photo library
   - Organize and manage captured media

## 🔧 Requirements

- **iOS Version:** iOS 13.0 or later
- **Xcode:** 12.0 or later
- **Swift:** 5.3 or later
- **Device:** iPhone or iPad with camera capability

### Device Capabilities

The app requires:
- Camera access (for photo/video capture)
- Photo Library access (for importing and saving media)
- Microphone access (for video audio recording)

## 📦 Installation

### Prerequisites

1. Ensure you have Xcode installed on your Mac
2. Clone the repository:
   ```bash
   git clone https://github.com/Muskanarora17/Camera-Application.git
   cd Camera-Application
   ```

### Setup Steps

1. **Open the Project**
   ```bash
   open CameraTest.xcodeproj
   ```

2. **Configure Signing & Capabilities**
   - Select the `CameraTest` project in Xcode
   - Go to the "Signing & Capabilities" tab
   - Set your Team ID
   - Ensure all required capabilities are enabled

3. **Build & Run**
   - Select your target device or simulator (iOS 13.0 or later)
   - Press `Cmd + R` to build and run
   - Or use `Product → Run` from the menu

## 📁 Project Structure

```
Camera-Application/
├── CameraTest/                    # Main application source code
│   ├── AppDelegate.swift          # Application lifecycle management
│   ├── SceneDelegate.swift        # Scene session lifecycle
│   ├── ViewController.swift        # Main view controller (UI logic)
│   ├── Info.plist                 # Application configuration
│   ├── Main.storyboard            # UI layout and connections
│   └── Assets.xcassets/           # Images and app icons
├── CameraTest.xcodeproj/          # Xcode project configuration
├── CameraTestTests/               # Unit tests
│   └── CameraTestTests.swift      # Test cases
└── CameraTestUITests/             # UI automation tests
```

### Key Components

- **AppDelegate.swift** - Handles app initialization and scene management
- **SceneDelegate.swift** - Manages window and view controller lifecycle for the app scenes
- **ViewController.swift** - Contains the main UI logic for camera and gallery operations
- **Main.storyboard** - Defines the app's user interface and navigation flow

## 🚀 Usage

### Launching the App

1. Build and run the app on a physical device or simulator
2. Grant necessary permissions when prompted:
   - Camera access
   - Photo Library access
   - Microphone access

### Using the Features

1. **Capture a Photo**
   - Tap the camera button to open the camera
   - Take a photo and confirm
   - The photo will be displayed on screen

2. **Record a Video**
   - Access the camera in video mode
   - Press record and capture up to 15 seconds of video
   - Stop recording and confirm

3. **Import from Gallery**
   - Select the gallery option to browse existing photos/videos
   - Choose media to import
   - Media will be displayed in the app

4. **Apply Filters**
   - With an image displayed, access the filter options
   - Select and apply your desired filter
   - Preview the filtered result

5. **Save to Gallery**
   - After editing or capturing media, tap save
   - The media will be stored in your device's photo library

## 🏗️ Architecture

The app follows a Model-View-Controller (MVC) architecture:

- **View Layer:** Storyboard-based UI defined in `Main.storyboard`
- **Controller Layer:** `ViewController` manages user interactions and coordinates between views and models
- **Model Layer:** Media data and filtering logic

### UIKit Framework

The application uses Apple's UIKit framework for:
- Camera access via `UIImagePickerController`
- Image/Video display
- Filter application and rendering

## 🧪 Testing

The project includes test bundles for different testing approaches:

### Running Tests

1. **Unit Tests**
   ```
   Product → Scheme → CameraTestTests
   Press Cmd + U to run
   ```

2. **UI Tests**
   ```
   Product → Scheme → CameraTestUITests
   Press Cmd + U to run
   ```

Test files are located in:
- `CameraTestTests/` - Unit tests
- `CameraTestUITests/` - UI automation tests

## 🔐 Permissions

The app requires the following permissions in `Info.plist`:

| Permission | Usage |
|-----------|-------|
| **Camera** | To capture photos and videos |
| **Photo Library** | To import media and save edited content |
| **Microphone** | To record audio with videos |

Users will be prompted to grant these permissions on first use.

## ⚠️ Known Limitations

1. **Video Duration:** Videos are limited to a maximum of 15 seconds
2. **Device Support:** Requires iOS 13.0 or later
3. **Camera Requirement:** Device must have camera hardware
4. **Photo Library:** Depends on device having accessible photo storage

## 🛠️ Development

### Building the App

```bash
# Build for development
xcodebuild -scheme CameraTest -configuration Debug

# Build for release
xcodebuild -scheme CameraTest -configuration Release
```

### Code Standards

- Follow Swift naming conventions (camelCase)
- Keep view controller logic modular
- Use storyboards for UI definition
- Document complex functions with comments

## 📱 Supported Devices

- iPhone 6s and later
- iPad (5th generation) and later
- All devices with camera capability
- iOS 13.0 and above

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is currently unlicensed. For licensing information, please contact the repository owner.

## 👤 Author

**Muskan Arora**
- GitHub: [@Muskanarora17](https://github.com/Muskanarora17)
- Project Created: December 2020

## 📞 Support

For issues, questions, or suggestions:
1. Open an issue on the GitHub repository
2. Provide detailed description of the problem
3. Include device model and iOS version
4. Attach screenshots if applicable

## 🔄 Version History

- **v1.0** (December 2020) - Initial release with core camera and filter features

---

**Last Updated:** July 2026  
**Repository:** [Muskanarora17/Camera-Application](https://github.com/Muskanarora17/Camera-Application)
