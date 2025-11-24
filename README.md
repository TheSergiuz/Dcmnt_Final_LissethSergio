# RadioApp - Christian Radio Streaming Application

## Project Information

- **Course:** Software Models and Documentation
- **Professor:** Ing. Hely Suárez Marín
- **Team Members:**
  - Lisseth Andrea Orduz Sanchez
  - Sergio Andrés Acosta Navarro
- **Date:** November 2025
- **Institution:** Fundación de Estudios Superiores Comfanorte

## Documentation

### Core Documents
- [Executive Document](./docs/executive-document.md) - Complete project overview and business case
- [Technical Specifications](./docs/technical-specifications.md) - Detailed technical requirements
- [Bibliography & References](./docs/bibliography.md) - Academic and technical references

## Project Overview

**RadioApp** is a simplified mobile application designed to provide Christian radio streaming access to rural Venezuelan communities. The application addresses the digital divide by offering an intuitive, single-button interface optimized for users over 45 years old with limited technical experience.

### Key Features
- One-button operation ("Reproducir Radio")
- 70% bandwidth reduction through audio compression
- Automatic reconnection for unstable networks
- Support for older Android devices (5+ years old)
- High-contrast, accessible interface design
- Minimal data consumption for expensive rural plans

## UML Diagrams

### Static Diagrams

| Diagram | Preview | Source File |
|---------|---------|-------------|
| **Class Diagram** | [View PNG](./diagrams/static/class-diagram.png) | [Edit (.drawio)](./diagrams/source/class-diagram.drawio) |
| **Package Diagram** | [View PNG](./diagrams/static/packages-diagram.png) | [Edit (.drawio)](./diagrams/source/packages-diagram.drawio) |
| **Object Diagram** | [View PNG](./diagrams/static/objects-diagram.png) | [Edit (.drawio)](./diagrams/source/objects-diagram.drawio) |
| **Component Diagram** | [View PNG](./diagrams/static/components-diagram.png) | [Edit (.drawio)](./diagrams/source/components-diagram.drawio) |
| **Deployment Diagram** | [View PNG](./diagrams/static/deployment-diagram.png) | [Edit (.drawio)](./diagrams/source/deployment-diagram.drawio) |

### Dynamic Diagrams

| Diagram | Preview | Source File |
|---------|---------|-------------|
| **Use Case Diagram** | [View PNG](./diagrams/dynamic/use-case-diagram.png) | [Edit (.drawio)](./diagrams/dynamic/use-case-diagram.drawio) |
| **Activity Diagram** | [View PNG](./diagrams/dynamic/activity-diagram.png) | [Edit (.drawio)](./diagrams/dynamic/activity-diagram.drawio) |
| **Sequence Diagram** | [View PNG](./diagrams/dynamic/sequence-diagram.png) | [Edit (.drawio)](./diagrams/dynamic/sequence-diagram.drawio) |
| **Communication Diagram** | [View PNG](./diagrams/dynamic/communication-diagram.png) | [Edit (.drawio)](./diagrams/dynamic/communication-diagram.drawio) |
| **Timing Diagram** | [View PNG](./diagrams/dynamic/timing-diagram.png) | [Edit (.drawio)](./diagrams/dynamic/timing-diagram.drawio) |
| **State Diagram** | [View PNG](./diagrams/dynamic/state-diagram.png) | [Edit (.drawio)](./diagrams/dynamic/state-diagram.drawio) |

## System Architecture

### Main Components

1. **User Interface Layer**
   - MainActivity (single-screen approach)
   - Large, accessible play button
   - High-contrast visual design

2. **Audio Processing Layer**
   - AudioStreamManager for stream control
   - Opus codec integration (70% compression)
   - Adaptive bitrate based on connection

3. **Network Management Layer**
   - NetworkMonitor for connection state
   - Auto-reconnection logic
   - Bandwidth optimization

4. **Data Management Layer**
   - DataManager for preferences
   - CacheManager for offline buffering
   - Minimal storage footprint

## Problem Statement

Rural Venezuelan adults over 45 face significant barriers accessing Christian radio through existing mobile applications. Current streaming apps assume users are comfortable with complex interfaces, consume excessive mobile data, and perform poorly on older Android devices common in these communities.

## Solution Approach

The RadioApp eliminates complexity through radical simplification:
- **One-touch operation**: Single button to start/stop radio
- **Invisible complexity**: All technical decisions handled internally
- **Data-conscious**: Advanced compression reduces bandwidth by 70%
- **Inclusive design**: Works on 5-10 year old Android devices
- **Resilient streaming**: Automatic handling of connection interruptions

## Technical Requirements

### Minimum Device Requirements
- Android 5.0 (API Level 21) or higher
- 1GB RAM
- 50MB available storage
- 3G/4G network connection

### Development Stack
- **Language:** Kotlin 1.9.0
- **IDE:** Android Studio Hedgehog 2023.1.1
- **Architecture:** MVVM Pattern
- **Min SDK:** Android 5.0 (API 21)
- **Target SDK:** Android 14 (API 34)

## Installation & Setup
```bash
# Clone the repository
git clone https://github.com/TheSergiuz/Dcmnt_Final_LissethSergio.git

# Navigate to project directory
cd Dcmnt_Final_LissethSergio

# Open project documentation
# All diagrams can be edited using draw.io (https://app.diagrams.net/)
```

## Project Structure
```
Parcial2Documentacion/
├── README.md                          # This file
├── docs/                              
│   ├── executive-document.md         # Business case & overview
│   ├── technical-specifications.md   # Technical details
│   └── bibliography.md               # References & citations
└── diagrams/                         
    ├── static/                       # Static UML diagrams (PNG)
    │   ├── class-diagram.png
    │   ├── packages-diagram.png
    │   ├── objects-diagram.png
    │   ├── components-diagram.png
    │   └── deployment-diagram.png
    ├── dynamic/                      # Dynamic UML diagrams (PNG)
    │   ├── use-case-diagram.png
    │   ├── activity-diagram.png
    │   ├── sequence-diagram.png
    │   ├── communication-diagram.png
    │   ├── timing-diagram.png
    │   └── state-diagram.png
    └── source/                       # Editable diagram files
        ├── class-diagram.drawio
        ├── packages-diagram.drawio
        └── ... (all .drawio files)
```

## Target Audience

**Primary Users:**
- Rural Venezuelan adults (45+ years)
- Limited technical expertise
- Basic smartphones (often older models)
- Expensive/limited data plans
- Strong desire for Christian content

**User Needs:**
- Simple, frustration-free interface
- Minimal data consumption
- Reliable streaming on poor connections
- Works on older devices
- Immediate access to content (no complex navigation)

## Success Metrics

1. **Accessibility**: 90% of users can start streaming within 2 taps
2. **Data Efficiency**: 70% reduction in data usage vs. standard apps
3. **Device Compatibility**: Runs on Android devices 5+ years old
4. **Connection Resilience**: Auto-reconnects within 10 seconds
5. **User Retention**: 80% daily active usage after first week

## Future Enhancements

- [ ] Offline recording for later playback
- [ ] Multiple station presets (maintaining simplicity)
- [ ] Schedule-based automatic start/stop
- [ ] Data usage reports and warnings
- [ ] Voice control for accessibility

## License

This proposal is developed for academic purposes as part of the Software Models and Documentation course at Fundación de Estudios Superiores Comfanorte.

## Acknowledgments

- Rural Venezuelan communities for inspiration and user feedback
- Professor Ing. Hely Suárez Marín for guidance
- UML 2.5.1 specification by Object Management Group (OMG)

---

*"Simple Technology for Rural Communities"* - Making digital radio accessible to everyone.
