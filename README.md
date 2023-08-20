# Docker Ubuntu Doom Emacs

Run Ubuntu container with Doom Emacs installed.

# Requirements

* Host must be running Xserver.
  * For MacOS
    * Install `XQuartz`
      ``` bash
      brew install --cask xquartz
      ```
    * Launch `XQuartz`. Select `Preferences >> Security`, check "Allow connections from network clients".
    * Allow network `X11` connections from `localhost`.
      ``` bash
      xhost +localhost
      ```
* The following directories are expected to exist to mount into the container:
  * `../.config-emacs`
  * `../.doom.d`
  * `../org`
  * `~/workspace`

# Scripts

* `build-image`
* `launch-container`
