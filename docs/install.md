<h1>
  <img src="../assets/vixen_logo.svg" alt="Vixen Logo" width=64 style="vertical-align: -40%; margin-right: 20px;">
  Install Vixen Shell
</h1>

### Prerequisites

Before getting started with Vixen Shell, make sure you have the following:

1. **Operating System**:
    - A Linux distribution compatible with Wayland (e.g., Ubuntu, Fedora, Arch Linux, [Manjaro Linux](https://manjaro.org/)).

2. **Window Manager**:
    - Sway, Hyprland, or any other window manager compatible with Wayland.

3. **Languages and Technologies**:
    - **Python**: Ensure Python is installed (version 3.8 or higher).
    - **yarn**: For managing dependencies and building front-end components.

4. **Development Tools**:
    - A code editor or IDE (Visual Studio Code is recommended).
    - Git for version control (Recommended).

5. **Permissions and Access**:
    - Administrator or superuser access to install certain dependencies and perform system configurations.

## Install Vixen Shell

!!! warning "Yarn"
    - Before proceeding with the installation, ensure that Yarn is installed on your system. You can check if Yarn is installed by running the following command in your terminal:

        ``` bash
        yarn --version
        ```

    - If Yarn is not installed or if the command returns an error, you can install Yarn using the appropriate method for your system.

        ``` bash title="Arch Linux based distribution"
        sudo pacman -S yarn
        ```

- Go to the [Vixen Shell GitHub](https://github.com/vixen-shell/vixen-shell) page and download the project archive in ZIP format, or download it [here](https://github.com/vixen-shell/vixen-shell/archive/refs/heads/main.zip).

- Once the download is complete, locate the ZIP file in your download folder. Right-click on the archive and select the option to extract the files. You can also use the command line:

    ``` bash
    unzip vixen-shell-main.zip
    ```

- After extracting the files, navigate to the newly created directory:

    ``` bash
    cd vixen-shell-main
    ```

- In the extracted directory, run the installation script as an administrator with the following command:

    ``` bash
    sudo ./install
    ```
    Confirm your choice and this script will install Vixen Shell on your system.

## Uninstall Vixen Shell

- To uninstall Vixen Shell from your system, simply type the following command:

    ``` bash
    sudo vxm --setup remove
    ```
    Confirm your choice and Vixen Shell will be completely uninstalled (or not depending on your choice :smile:)