OmniNet
A cross-router administration platform built with C++ and Qt.**

OmniNet is a desktop application concept designed to simplify router management through a unified, user-friendly interface. Its long-term goal is to provide a consistent administration experience across different router manufacturers without requiring users to navigate each router's individual interface.

Project Overview

Router administration can be unnecessarily complicated, particularly for users managing different router models. OmniNet aims to address this by introducing a unified interface supported by structured, model-specific router profiles.

The project initially focuses on the **Tenda F3**, with an architecture intended to accommodate additional router models and manufacturers as development progresses.
Planned Capabilities

- Router configuration and administration.
- Wi-Fi network name and password management.
- Wireless security configuration.
- Network and device information.
- Connected-device management.
- Wireless settings and available configuration options.
- Router-specific functionality through structured profiles.
- Support for additional router models through extensible profiles.

Feature availability will depend on the capabilities of the connected router.
Architecture

OmniNet is being developed around a profile-based architecture.

Rather than hardcoding every router model into the application, the intended design allows router-specific configuration information to be represented through structured profiles. This provides a foundation for extending support to other manufacturers and models.

Technology Stack

- Language:C++
- Framework:Qt 6
- Build System:CMake
- UI:Qt Widgets
- Networking:Qt Network
- Standard: C++17

Development Status

<badge color="warning">Early development</badge>

OmniNet is actively being developed. The initial application foundation and desktop interface are being established, beginning with the Tenda F3 router profile.

Planned capabilities are not necessarily implemented or available yet.

Project Goals

1. Build a clean and intuitive router administration experience.
2. Establish a modular architecture that supports multiple router models.
3. Reduce the complexity of everyday network management.
4. Make router administration more accessible without compromising configuration safety.
5. Expand compatibility through extensible router profiles.

Building from Source

Requirements

- C++17 compatible compiler
- Qt 6 with Widgets and Network modules
- CMake 3.21 or later

Build

```bash
git clone https://github.com/lam3c/OmniNet.git
cd OmniNet

cmake -S . -B build
cmake --build build
```

Open the project in Qt Creator or another compatible CMake development environment.

Project Philosophy

OmniNet is built around one central idea: router administration should not require users to understand the complexities of every manufacturer's interface.

A unified experience, modular architecture, and extensible router support form the foundation of the project.

---

OmniNet — Simplifying Network Administration.**