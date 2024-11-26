# Cyborg

Cyborg is a comprehensive environment designed to transform your Android device into a fully functional Linux desktop. By leveraging Termux and XFCE, Cyborg provides a seamless and customizable user experience, enabling productivity and versatility on the go.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Directory Structure](#directory-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Features

- **Full XFCE Desktop Environment**: Enjoy a complete desktop experience with window management, panels, and customizable themes.
- **Debian Proot Integration**: Access a Debian-based filesystem within Termux, allowing the installation of a wide range of packages.
- **Termux-X11 Support**: Utilize the Termux-X11 server to run graphical applications seamlessly.
- **Robust Hardware Acceleration**: Achieve optimal performance using native drivers and Mesa Turnip drivers for both in-proot and out-of-proot acceleration, supporting Vulkan and OpenGL.
- **Minimal Emulation for Windows Applications**: Run DOS, Windows 95, Windows 2000/NT, Windows XP SP2, Windows 10, and Windows 11 applications with minimal emulation using Hangover and Wine.
- **Steam Integration**: Work in progress to run Steam with minimal emulation, balancing performance and ease of use between Linux and Windows versions.
- **Termux API Integration**: Future plans to unify with Android OS by expanding Termux API, enabling native use of USB, Bluetooth, camera, and other hardware components.
- **No Root Access Required**: Designed to function without the need for root access, ensuring accessibility and security.

## Installation

To install Cyborg, follow these steps:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/Cyborg.git
   ```

2. **Navigate to the Setup Directory**:

   ```bash
   cd Cyborg/setup
   ```

3. **Run the Setup Script**:

   ```bash
   ./install.sh
   ```

   *Note: Ensure that Termux has the necessary permissions and that you have a stable internet connection during installation.*

## Usage

After installation, you can start the XFCE desktop environment by running:

```bash
./start.sh
```

This script initializes the Termux-X11 server and launches the XFCE session. To stop the environment, execute:

```bash
./kill_termux_x11.sh
```

For detailed usage instructions and customization options, refer to the [documentation](documentation/README.md).

## Directory Structure

The Cyborg project is organized as follows:

- **assets/**: Contains icons, images, patches, templates, configurations, fonts, and other resources for the environment.
- **scripts/**: Includes scripts utilized by the environment during operation.
- **setup/**: Houses tools and scripts necessary for the installation and setup process.
- **root-fs/**: Contains the root filesystem of the environment, offering both minimal and complete setups for plug-and-play or customization.
- **packages/**: Stores Debian packages for the Cyborg environment, along with source files when available.
- **tools/**: Features portable, self-contained tools and scripts that can be executed without additional setup.
- **documentation/**: Provides comprehensive guides, manuals, and references for users and contributors.

## Contributing

We welcome contributions to enhance Cyborg. To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes with clear and concise messages.
4. Push your changes to your fork.
5. Open a pull request detailing your modifications.

Please adhere to the [contribution guidelines](documentation/CONTRIBUTING.md) and maintain code quality and consistency.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

We extend our gratitude to the developers and communities of Termux, XFCE, Debian, and Termux-X11 for their invaluable tools and support. Their contributions have been instrumental in making Cyborg possible.

*Note: Replace `https://github.com/yourusername/Cyborg.git` with the actual URL of your Cyborg repository.* 