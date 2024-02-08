# Setting Up a Mac for Development

This repository contains checklists and configuration files for setting up a web development environment on MacOS.

## Checklists

### User Accounts

- [X] Create a user/admin account
- [X] Perform System Updates

### System Preferences

- [X] Show Hidden Files in Finder

    ```
    Finder > Command + Shift + .
    ```

- [X] Show Path Bar in Finder

    ```
    Finder > View > Show Path Bar
    ```

- [X] Show File/Directory Status in Finder

    ```
    Finder > Show Status Bar
    ```

- [ ] Show All File and Directory Sizes 
    - [ ] Confirm available on Monterey

    ```
    Finder > View > Show View Options > (Check) Calculate all sizes
    ```

- [X] Show File Name Extensions

    ```
    Finder > Preferences > Advanced > (Check) Show all filename extensions
    ```

- [X] Show Reference to User in Finder Sidebar

    ```
    Finder > Preferences > <user> on the sidebar
    ```

- [X] Auto Hide Docks

    ```
    System Preferences > Dock & Menu Bar > (Check) Automatically hide and show the Dock
    ```

- [X] Turn Off Natural Scrolling (Mouse Wheel)

    ```
    System Preferences > Mouse > (Uncheck) Scroll direction: Natural
    ```

- [X] Disable Auto Correct Settings

    ```
    System Preferences > Keyboard > Text > 
        (Uncheck) "Correct spelling automatically"
        (Uncheck) "Capitalize words automatically"
        (Uncheck) "Add period with double-space"
        (Uncheck) "Use smart quotes and dashes"
    ```

- [X] Switch to Dark Theme

    ```
    System Preferences > Appearance > Dark
    ```

- [X] Remap Caps Lock Key to Escape

    ```
    System Preferences > Keyboard > Modifier Keys > Caps Lock Key
        (Choose) Escape
    ```

- [X] Show Most Frequently Folder in New Finder Windows

    ```
    Finder > Preferences > New Finder windows show > (Choose) "your custom folder"
    ```

- [X] Hide Sidebar's Infrequently Used Items 

    ```
    Finder > Preferences > Sidebar
    ```

- [X] Limit Search to Current Folder

    ```
    Finder > Preferences > Advanced > When performing a search > (Select) Search the Current Folder
    ```

- [X] Set Numbered Shortcuts for Switching Workspaces

    ```
    System Preferences > Keyboard > Shortcuts > Mission Control > (Check) Switch to Desktop <Num>
    ```

### Install software

- [X] [Homebrew](https://brew.sh/) - package manager
- [X] [Git](https://git-scm.com/download/mac) - version control
- [X] [Kitty](https://sw.kovidgoyal.net/kitty/) - terminal multiplexer
- [X] [Neovim](https://neovim.io/) - code editor 
    - [X] [My Config](https://github.com/ge3224/nvim_cfg)
- [X] [Maccy](https://maccy.app/) - clipboard manager
- [X] [Amethyst](https://github.com/ianyh/Amethyst) - tiling window manager
- [X] [Ansible](https://www.ansible.com/) - automation
    - [ ] Start Personal Mac Dev Playbook

#### Shell

- [ ] Create `~/.zprofile` config file 
- [X] Check `zsh` version, upgrade if necessary


    ```sh 
    brew install zsh                            # Install latest `zsh` via HomeBrew
    which zsh                                   # Show path to brew version of `zsh`
    dscl . -read /Users/<username> UserShell    # Check default shell
    sudo vim /etc/shells                        # Add path to brew version of `zsh` at the bottom of file
    chsh -s /usr/local/bin/zsh                  # Change default shell to new version 
    dscl . -read /Users/<username> UserShell    # Confirm the change
    brew upgrade zsh                            # Upgrade via brew
    ```

- [X] Symlink [`zsh` config](zsh/.zshrc) at `~/.zshrc`
- [ ] Create Keyboard Shortcut for Kitty

#### SSH Keys

- [X] Set up SSH Key
- [X] Add SSH to github account
- [ ] Configure SSH Agent to start with system

#### Programming Language Compilers, Tooling, Etc.

- [X] [Node.js](https://nodejs.org/en) - JavaScript Development
- [X] [Docker](https://docs.docker.com/get-docker/) - containerized apps
- [X] [Go](https://go.dev/dl/) - programming language
- [X] [Rust](https://www.rust-lang.org/learn/get-started) - programming language
- [X] [pnpm](https://pnpm.io/installation) - JavaScript package manager
- [X] [pipx](https://github.com/pypa/pipx) - Virtual Environment for Python
- [X] [poetry](https://python-poetry.org/docs/) - python package manager
- [ ] [Composer](https://getcomposer.org/download/) - PHP package manager
    - [ ] Install in local project (virtually)
- [X] [Dart](https://dart.dev/get-dart) - programming language

#### Browsers

- [X] [Brave](https://brave.com/)
- [X] [Firefox](https://www.mozilla.org/en-US/firefox/new/)
- [X] [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/)
- [x] [Firefox Nightly](https://www.mozilla.org/en-US/firefox/124.0a1/releasenotes/)
- [X] [Google Chrome](https://www.google.com/chrome/index.html)
- [X] [Google Chrome Canary](https://www.google.com/chrome/canary/)
- [X] [Microsoft Edge](https://www.microsoft.com/en-us/edge?ep=313&form=MA13M0&es=40&ch=1)
- [ ] [Safari Technology Preview](https://developer.apple.com/safari/technology-preview/) 
    - [ ] Requires macOS 13 or later
- [X] [Tor Browser](https://www.torproject.org/download/)

#### Mobile development

- [ ] [Xcode](https://developer.apple.com/xcode/) (App Store) - iOS development
- [ ] [Android Studio/SDK](https://developer.android.com/studio) - Android development
- [ ] [Expo](https://reactnative.dev/docs/environment-setup?guide=native) - React Native
- [ ] [Flutter](https://docs.flutter.dev/get-started/install) - Skia-based mobile development

## References

- [Apple Device Support Tutorials](https://it-training.apple.com/tutorials/apt-support)
- [Latest MacOS Patch: Monterey 12.7.3](https://support.apple.com/en-us/HT214057) 

## zsh:

- [Z Shell Doc](https://zsh.sourceforge.io/Guide/zshguide.html)
- [No oh-my-zsh config](https://www.youtube.com/watch?v=bTLYiNvRIVI)

Amethyst

- [Getting Started](https://www.youtube.com/watch?v=7Z9-Ry4yGNc) 

Ansible

- [Mac Dev Playbook Example](https://github.com/geerlingguy/mac-dev-playbook)
