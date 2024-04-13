# Flutter on Codespaces ❤

This is a repository for developing with [Flutter](https://flutter.dev/) on the web on [GitHub Codespaces](https://github.com/features/codespaces).

Flutter is a cross-platform UI framework by Google for building apps. Codespaces is a cloud-based development environment that lets you run a full-featured IDE in the cloud. This repository lets you get started with Flutter on Codespaces in just a few clicks.

**Table of Contents**
- [Setup](#setup)
  - [Getting started](#getting-started)
- [Flutter Development](#flutter-development)
  - [Developing for mobile](#developing-for-mobile)
- [Codespaces Usage](#codespaces-usage)
  - [Managing your codespace](#managing-your-codespace)

## Setup

### Getting started

1. Fork this repository.

2. In your new repository, press "Code", select "Codespaces", then press "Create codespace on main". A container with everything you need to get started will be created automatically, then you'll be taken to your new codespace (VS Code in your browser).

3. Press the "Extensions" icon in the left sidebar. You'll see that the Flutter and Dart extensions are already being installed. The environment won't work properly until the installation is complete, so wait for it to finish.

4. In your integrated terminal (the TERMINAL tab), run `flutter pub get` to install the missing Flutter dependencies.

5. In the ports view (the PORTS tab), port 3000 should be listed there already. Right click on it, and, under "Port Visibility", select "Public". This is important so the app can access services on your client from other server ports without getting blocked due to CORS.

6. Run `./run.sh` (or copy-paste the code from run.sh file) in the terminal to start the app. A notification will appear saying that an app opened on port 3000. You can press "Open in Browser" to open it, but it won't load until the terminal shows that it's ready. You can refresh once the app is loaded (as indicated by a prompt to press "R" to reload).

    > You can find the link to access the app in your browser at any time by going to the ports view, right clicking on port 3000, and pressing "Open in Browser".

    > If you get "Permission denied", use `chmod +x ./run.sh` and after that `./run.sh`

7. That's it! Make changes in `lib/main.dart`, press "R" in the terminal, then refresh the page to see your changes appear quickly.

## Flutter Development

### Developing for mobile

Running Flutter in Codespaces makes it a bit difficult to run the app in a mobile simulator. However, developing for the web is basically the same as developing for mobile. I'd recommend opening your browser's developer tools and selecting a mobile device to emulate.

If you're using Chrome or another Chromium-based browser, you can open DevTools like [this](https://developer.chrome.com/docs/devtools/open/) and emulate a device like [this](https://developer.chrome.com/docs/devtools/device-mode/). It'll be pretty similar for other browsers like Safari and Firefox.

## Codespaces Usage

### Managing your codespace

When you're not using your codespace, deactivate it by going to [Codespaces](https://github.com/codespaces), pressing the 3 dots on the right side of the codespace, and pressing "Stop codespace". You can also deactivate it within the codespace by pressing "Codespaces" at the bottom left of VS Code and selecting "Stop Current Codespace".

