# Kim Orb Rive Preview

This is a Flutter web app to preview the `kim_orb.riv` file.

## Features

- **Loading**: Automatically loads `assets/kim_orb.riv`.
- **Triggers**: exposed triggers for `talking`, `listening`, `reset`, `thinking`.
- **Inputs**: exposed `voiceLevel` number input via a slider.
- **State Machine**: Allows changing the state machine name dynamically if the default "State Machine 1" is incorrect.

## Setup

1.  Navigate to the project directory:
    ```
    cd kim_orbs
    ```
2.  Install dependencies:
    ```
    flutter pub get
    ```
3.  Run the app locally with Chrome:
    ```
    flutter run -d chrome
    ```
    Or build for web:
    ```
    flutter build web
    ```
    Then serve the `build/web` directory using any static file server (e.g. `python3 -m http.server 8000 --directory build/web`).

## Note on Rive Version

This project uses `rive: ^0.11.17` for compatibility with the current Flutter web environment. If you need features from later versions (0.13+), ensure your environment supports `rive_native` correctly on web or check documentation for enabling WASM/CanvasKit specifically.
