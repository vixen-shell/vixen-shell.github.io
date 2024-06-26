# ![vixen logo](assets/vixen_logo.svg){ width=64 style="vertical-align: -40%; margin-right: 10px;" } Welcome to Vixen Shell

## Presentation

The **Vixen Shell** project is an initiative dedicated to creating a highly customizable desktop environment for [Wayland](https://wayland.freedesktop.org/) users on Linux. Designed with a focus on development, it allows users to code the various components necessary to build their own desktop environment. This project is particularly useful for users of window managers such as [Sway](https://swaywm.org/) or [Hyprland](https://hyprland.org/).

**Vixen Shell** stands out by using [Python](https://www.python.org/) for the back-end, while the user interface (front-end) is developed with modern web technologies such as [React](https://fr.legacy.reactjs.org/), [TypeScript](https://www.typescriptlang.org/) and CSS.

The project was initially intended for [Hyprland](https://hyprland.org/), but during its development, its flexibility has allowed it to be adapted to other window managers. This is why, as you will discover by reading this documentation, there are pre-existing features dedicated to [Hyprland](https://hyprland.org/) in Vixen Shell's extras and many references and examples related to [Hyprland](https://hyprland.org/).

??? quote "Prerequistes"
    Before getting started with **Vixen Shell**, make sure you have the following:

    1. **Operating System**:
        - A Linux distribution compatible with Wayland (e.g., Ubuntu, Fedora, Arch Linux, [Manjaro Linux](https://manjaro.org/)).

    2. **Window Manager**:
        - Sway, Hyprland, or any other window manager compatible with Wayland.

    3. **Languages and Technologies**:
        - **Python**: Ensure Python is installed (version 3.11 or higher).
        - **yarn**: For managing dependencies and building front-end components.

    4. **Development Tools**:
        - A code editor or IDE (Visual Studio Code is recommended).
        - Git for version control (Recommended).

    5. **Permissions and Access**:
        - Administrator or superuser access to install certain dependencies and perform system configurations.

!!! info "Version 1.0.0b1"
    Currently, **Vixen Shell** is in **Beta**. Installing it should not pose any particular risks to your system. Your feedback would be extremely valuable to me if you are interested in this project.

<div class="grid cards" markdown>

-   ![linux icon](#){src="assets/icons/linux.svg" width=32 style="vertical-align: -40%; margin-right: 10px; border-radius: 5px;"} __Linux__

    ---

    The free and open-source operating system for everyone.
    
-   ![python icon](#){src="assets/icons/python.svg" width=32 style="vertical-align: -40%; margin-right: 10px;"} __Python__

    ---

    Python is a programming language that lets you work quickly and integrate systems more effectively.

    [:octicons-arrow-right-24: Visit](https://www.python.org/)


-   ![typescript icon](#){src="assets/icons/typescript.svg" width=32 style="vertical-align: -40%; margin-right: 10px;"} __TypeScript__

    ---

    TypeScript is a strongly typed programming language that builds on JavaScript, giving you better tooling at any scale.

    [:octicons-arrow-right-24: Visit](https://www.typescriptlang.org/)

-   ![react icon](#){src="assets/icons/react.svg" width=32 style="vertical-align: -40%; margin-right: 10px;"} __React__

    ---

    A JavaScript library for building user interfaces.

    [:octicons-arrow-right-24: Visit](https://fr.legacy.reactjs.org/)

</div>

## Under the Hood

### Vixen Shell Core

- **[GTK3 (GIMP Toolkit 3)](https://www.gtk.org/):** GTK3, well-known among developers, is an open-source graphical library used to create graphical user interfaces (GUIs). It provides a wide range of widgets and controls for developing modern applications with attractive and responsive interfaces. In **Vixen Shell**, GTK3 is primarily used for window management.

- **[WebKitGTK (or GTKWebKit2)](https://webkitgtk.org/):** WebKitGTK is a version of the WebKit rendering engine adapted for integration with GTK. WebKit is used by browsers like Safari. WebKitGTK allows embedding web content into GTK applications, offering capabilities for web navigation and HTML content display. Through WebKitGTK, **Vixen Shell** can display web content to generate user interfaces.

- **[GTK Layer Shell](https://github.com/wmww/gtk-layer-shell):** GTK Layer Shell is a library enabling GTK applications to utilize the layer surfaces functionality of Wayland, a modern display server protocol for Linux. This is particularly useful for applications like panels, docks, or notifications that require precise control over their positioning and appearance on the screen.

- **[FastAPI](https://fastapi.tiangolo.com/):** FastAPI is a modern and high-performance web framework for building APIs with Python 3.7+ based on standard Python type annotations. It's designed to produce robust and efficient web applications. FastAPI primarily serves as the backend engine for **Vixen Shell**.

### Vixen Shell Features

With Vixen Shell, you can create your own user interface features. To generate these features, Vixen Shell requires two types of support to create the configuration:

- **[Python](https://www.python.org/):** A Python module will generate the root configuration for your feature and, if necessary, enrich the backend with customized data and actions.

- **[TypeScript](https://www.typescriptlang.org/):** The user interface will be implemented in TypeScript using the React framework.

These configuration files are automatically generated by the Vixen Shell manager's command line tool (vxm) when creating a new feature.

!!! note
    Vixen Shell requires no special dependency installations, except for Yarn, which is used to build the user interface content. This is possible because Vixen Shell operates within its own Python virtual environment.

## Similar Projects

There are many projects similar to Vixen Shell, each with their own architecture:

- [nwg-shell](https://nwg-piotr.github.io/nwg-shell/): A set of GTK-based tools designed to provide a feature-rich desktop environment for sway and other wlroots-based compositors.
- [Eww](https://github.com/elkowar/eww/): The ElKowar's Wacky Widgets (eww) framework allows you to create custom widgets for your desktop, using a flexible and scriptable XML configuration.
- [Waybar](https://github.com/Alexays/Waybar/): A highly customizable status bar for Wayland compositors, especially sway, written in C++.


## About the Autor

!!! note "Nohavye"
    [![GitHub Profile](https://avatars.githubusercontent.com/u/118626273?v=4){style="width: 128px; border-radius: 50%;" align=left}](https://github.com/Nohavye)
    I am passionate about application development and constantly seeking enriching experiences to deepen my skills. With recent training in JavaScript React Application Development, I am excited to contribute to innovative projects.

    Thank you for taking the time to read this documentation. Your interest and support are greatly appreciated. I hope you find Vixen Shell useful. If you have any questions, feedback, or contributions, please feel free to reach out via my [GitHub profile](https://github.com/your-github-username). Happy coding!
