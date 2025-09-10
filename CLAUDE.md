
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Flutter application for Misfits Admin, built with Flutter SDK ^3.8.1. The project targets multiple platforms including Android, iOS, Linux, macOS, Windows, and Web.

## Development Commands

### Flutter Commands

```bash
# Get dependencies
flutter pub get

# Run the app
flutter run

# Run on specific device/platform
flutter run -d chrome     # Web
flutter run -d windows    # Windows
flutter run -d macos      # macOS
flutter run -d linux      # Linux

# Build the app
flutter build apk         # Android APK
flutter build appbundle   # Android App Bundle
flutter build ios         # iOS
flutter build web         # Web
flutter build windows     # Windows
flutter build macos       # macOS
flutter build linux       # Linux

# Code analysis and formatting
flutter analyze           # Run static code analysis
flutter format .          # Format all Dart files
flutter test              # Run tests

# Clean build artifacts
flutter clean

# Upgrade dependencies
flutter pub upgrade
```

### Running Tests

```bash
# Run all tests
flutter test

# Run specific test file
flutter test test/widget_test.dart

# Run tests with coverage
flutter test --coverage
```

## Project Structure

The codebase follows standard Flutter project structure:

- **lib/** - Main application source code
  - `main.dart` - Application entry point with MyApp and MyHomePage widgets
  
- **android/** - Android-specific configuration and native code
  - Uses Kotlin for native Android code
  - Gradle build system with Kotlin DSL (.kts files)
  
- **ios/** - iOS-specific configuration and native code
  - Uses Swift for native iOS code
  - Xcode project configuration
  
- **web/** - Web-specific assets and configuration
  - Contains PWA manifest and icons
  
- **windows/**, **linux/**, **macos/** - Desktop platform configurations
  - Native platform runners and CMake configurations

## Code Style and Linting

The project uses `flutter_lints` package (^5.0.0) for code quality. Configuration is in `analysis_options.yaml`.

Key lint rules:
- Follows Flutter's recommended linting rules
- Custom rules can be enabled/disabled in `analysis_options.yaml`

## Dependencies

### Production Dependencies
- Flutter SDK
- `cupertino_icons: ^1.0.8` - iOS-style icons

### Development Dependencies
- `flutter_test` - Testing framework
- `flutter_lints: ^5.0.0` - Linting rules

## Platform-Specific Notes

### Android
- Minimum SDK version defined in `android/app/build.gradle.kts`
- Uses Material Design
- Kotlin-based MainActivity

### iOS
- Swift-based Runner
- Requires Xcode for building
- iOS deployment target defined in Runner.xcodeproj

### Web
- PWA-ready with manifest.json
- Responsive icons included
- Single-page application structure

## Hot Reload and Development

Flutter supports hot reload for rapid development:
- Save changes to see them instantly (hot reload)
- Press 'r' in terminal for hot reload
- Press 'R' for hot restart (resets app state)
- State is preserved during hot reload, reset with hot restart

## Venue Management System - Venue Admin App Context

### Project Overview
This Flutter application is the **Venue Admin App** for venue managers in the Misfits Venue Management System (VMS). The VMS aims to replace WhatsApp-based venue management with a structured platform that connects club leaders with venues.

### App Purpose
The Venue Admin App enables venue managers to:
- Centralize management of all events and bookings
- Receive and respond to association requests from Misfits club leaders
- Manage venue details, calendars, and partnerships efficiently

### Core Features

#### 1. Venue Setup and Configuration
- **Amenities Management**: Detail available amenities (sound systems, projectors, seating, catering, Wi-Fi, accessibility)
- **Interactive Map Integration**: Location details, landmarks, and directions
- **Image Gallery**: Upload images and virtual tours of spaces
- **Terms of Association**: Define pricing, cancellation policies, operational hours, event rules, cover charges

#### 2. Association Request Management Dashboard
- **Centralized Request Viewing**: View incoming requests with:
  - Requesting club details
  - Proposed event type
  - Desired dates
  - Estimated attendance (footfall)
  - Equipment requirements
  - Fee collection preferences
- **Approval/Rejection Workflow**: Approve, reject, or modify terms for requests
- **Request Status**: In-process, Complete, or Rejected

#### 3. Calendar Management
- **Integrated Event Scheduling**: Manage Misfits events and external events in unified view
- **Automatic Event Integration**: Approved events auto-added to calendar
- **Blackout Dates**: Mark unavailable dates
- **Conflict Prevention**: Optimize venue utilization

### Operational Framework

#### Account Management
- Individual secure accounts for each venue manager
- Multi-venue support with seamless switching between venues
- Guided initial setup flow → Dashboard redirection

#### Partnership Workflow
1. **Request Reception**: Receive requests (leaders limited to 2 venue queries)
2. **Review & Response**: Accept/Reject/Modify terms
3. **Mutual Acceptance**: Both parties must approve final terms
4. **Discrepancy Handling**: Leaders can raise issues, venues revise terms

#### Meeting Coordination
- Request meetings through operations team
- Operations team facilitates scheduling between venue manager and club leader

### Key Business Rules
- Club leaders can query maximum 2 venues
- Mutual acceptance required for partnerships
- Transparent terms definition
- Auto-calendar integration upon approval

### Data Requirements from Club Leaders
- Estimated footfall per meetup
- Equipment requirements
- Fee collection preferences (upfront payment details)
- Activity type
- Geographic area

### Development Focus Areas
1. **Initial Setup Flow**: Complete venue profile configuration
2. **Dashboard**: Primary interface for request management
3. **Request Management**: Quick approve/reject/modify workflow
4. **Calendar Integration**: Seamless event scheduling
5. **Terms Management**: Clear definition and modification tools

### Integration Points
- Club leader frontend system connection
- Operations team communication
- Automatic calendar synchronization
- Real-time status updates

## Design Theme Guidelines

### Light Theme Color Palette

#### Background
- **Primary Background**: `#FCFCFD`
- **Bottom Sheet Background**: `#F4F4F5`

#### Typography
- **Font Family**: Always use **Lato** font (follow Figma file instructions)

#### Text Colors
- **Headings**: `#191C20`
- **Disabled/Hint Text (TextFields)**: `#717175`
- **Bottom Sheet Text**: `#46474A`
- **Error Messages**: `#BA1A1A`
- **Hint Text/Labels**: `#46474A`

#### Borders and Strokes
- **Border Color**: `#ABABAE`

#### Button States
- **Enabled Button**: `#1E7ACC`
- **Disabled Button**: `#E5E5E5`

### Implementation Notes
- Always follow the Figma file specifications for exact implementation details
- Maintain consistency across all screens and components
- Use these colors as the foundation for the light theme throughout the application

### Dark Theme Color Palette

#### Background
- **Primary Background**: (To be defined)
- **Bottom Sheet Background**: `#32353A`

#### Text Colors
- **Headings and Labels**: `#FCFCFD`
- **Subheadings/Icons**: `#C6C6CA`
- **Disabled/Hint Text**: `#ABABAE`

### Common Theme Elements (Both Light and Dark)

#### Button States
- **Enabled Button**: `#1E7ACC`
- **Disabled Button**: `#E5E5E5`

#### Borders and Strokes
- **Border Color**: `#ABABAE`

#### Special Buttons
- **Background Color**: `#4D3500`
- **Stroke Color**: `#FABB22`
- **Text Color**: `#FFDEA3`

