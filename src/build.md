# Chapter 2: How to Compile

## Building Wazuh Agent from Source

### Prerequisites

To compile Wazuh Agent, ensure that you have the following dependencies installed:

- **Operating System**: Linux, macOS, or Windows
- **Compilers**: GCC or Clang for Linux/macOS, Visual Studio for Windows
- **Build Tools**:
  - `make`
  - `cmake`
  - `ninja` (optional)
- **Libraries**:
  - `openssl`
  - `libssl-dev`
  - `zlib`
  - `libsystemd-dev` (for systemd support on Linux)

### Steps to Compile on Linux/macOS

1. **Clone the Wazuh repository**:
   ```bash
   git clone https://github.com/wazuh/wazuh.git
   cd wazuh/src
   ```

2. **Configure the build environment**:
   ```bash
   mkdir build
   cd build
   cmake ..
   ```

3. **Compile the source code**:
   ```bash
   make
   ```

4. **Install the agent**:
   ```bash
   sudo make install
   ```

### Steps to Compile on Windows

1. **Clone the Wazuh repository**:
   Open a terminal in Visual Studio and run:
   ```bash
   git clone https://github.com/wazuh/wazuh.git
   cd wazuh/src
   ```

2. **Open the CMake GUI** and configure the project using the appropriate toolchain (Visual Studio, Ninja, etc.).

3. **Build the solution**:
   After configuration, click "Generate" and "Open Project" in Visual Studio. Then, compile the solution from the Visual Studio interface.

4. **Install the agent**:
   Run the generated executable to complete the installation process.

### Additional Options

- **Debugging**: Use the `-DCMAKE_BUILD_TYPE=Debug` flag during the `cmake` configuration step to enable debugging symbols.
- **Cross-compilation**: To build for a different architecture (e.g., ARM64), set up a cross-compiler toolchain during the `cmake` configuration.
