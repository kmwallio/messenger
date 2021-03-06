The best available desktop app for Facebook Messenger. Created for [elementary OS](https://elementary.io). Inspired by [this mockup](https://github.com/elementary/mockups/blob/master/apps/plank/with-chat-bubble.png). Many thanks to [purple facebook](https://github.com/dequis/purple-facebook)'s authors for creating API to communicate with Messenger service.

## Features

1. Native notifications of incoming messages (including notification badges)
2. Easy access to your conversations via chat bubbles
3. Simple, beautiful interface
4. No useless, Snapchat-like features :)

![alt text](https://raw.githubusercontent.com/aprilis/messenger/master/data/screenshot.png)

## Getting started

If you are using elementaryOS 0.4 Loki, follow [these steps](https://github.com/aprilis/messenger/blob/loki/README.md). Otherwise:

1. Download the repository and all necessary dependencies. Enter the terminal and type:

  ```
  git clone https://github.com/aprilis/messenger
  cd messenger
  sudo apt install elementary-sdk libwebkit2gtk-4.0-dev libunity-dev libsoup2.4-dev libnotify-dev libplank-dev libbamf3-dev libwnck-3-dev intltool meson
  ```

2. Build the app.

  ```
  meson build
  cd build
  ninja
  ninja install
  sudo ldconfig
  ```

## Updates

As this app isn't stable yet, updates may occur quite often. To download and install an update, you should open the terminal and navigate to the directory with cloned repository (probably it's named messenger) and type:

  ```
  git pull
  cd build
  ninja install
  ```

Now you have to restart the app. To do this, open the main window, click the gear icon and select 'Quit'. Now open the main window again - your app is up-to-date!

## Removing old Plank version

If you have installed old Messenger version you need to remove forked Plank which was required before. Open the terminal in the messenger folder and type:

  ```
  sudo script/uninstall-plank.sh
  ```
