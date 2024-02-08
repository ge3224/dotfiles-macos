# Setting Up a Mac for Development

This repository contains checklists and configuration files for setting up a web development environment on MacOS.

## Checklists

### System Preferences

- [ ] Show Hidden Files in Finder

    ```
    Finder > Command + Shift + .
    ```

- [ ] Show Path Bar in Finder

    ```
    Finder > View > Show Path Bar
    ```

- [ ] Show File/Directory Status in Finder

    ```
    Finder > Show Status Bar
    ```

- [ ] Show All File and Directory Sizes

    ```
    Finder > View > Show View Options > (Check) Calculate all sizes
    ```

- [ ] Show File Name Extensions

    ```
    Finder > Preferences > Advanced > (Check) Show all filename extensions
    ```

- [ ] Show Reference to User in Finder Sidebar

    ```
    Finder > Preferences > <user> on the sidebar
    ```

- [ ] Auto Hide Docks

    ```
    System Preferences > Dock & Menu Bar > (Check) Automatically hide and show the Dock
    ```

- [ ] Disable Auto Correct Settings

    ```
    System Preferences > Keyboard > Text > 
        (Uncheck) "Correct spelling automatically"
        (Uncheck) "Capitalize words automatically"
        (Uncheck) "Add period with double-space"
        (Uncheck) "Use smart quotes and dashes"
    ```

- [ ] Switch to Dark Theme

    ```
    System Preferences > Appearance > Dark
    ```

- [ ] Remap Caps Lock Key to Escape

    ```
    System Preferences > Keyboard > Modifier Keys > Caps Lock Key
        (Choose) Escape
    ```

- [ ] Show Most Frequently Folder in New Finder Windows

    ```
    Finder > Preferences > New Finder windows show > (Choose) "your custom folder"
    ```

- [ ] Hide Sidebar's Infrequently Used Items 

    ```
    Finder > Preferences > Sidebar
    ```

- [ ] Limit Search to Current Folder

    ```
    Finder > Preferences > Advanced > When performing a search > (Select) Search the Current Folder
    ```

- [ ] Set Numbered Shortcuts for Switching Workspaces

    ```
    System Preferences > Keyboard > Shortcuts > Mission Control > (Check) Switch to Desktop <Num>
    ```

### Install software

- [ ] [Homebrew](https://brew.sh/) - package manager
- [ ] [Git](https://git-scm.com/download/mac) - version control
- [ ] [Kitty](https://sw.kovidgoyal.net/kitty/) - terminal multiplexer
- [ ] [Neovim](https://neovim.io/) - code editor 
    - [ ] [My Config](https://github.com/ge3224/nvim_cfg)
- [ ] [Maccy](https://maccy.app/) - clipboard manager
- [ ] [Amethyst](https://github.com/ianyh/Amethyst) - tiling window manager
- [ ] [Ansible](https://www.ansible.com/) - automation
    - [ ] Start Personal Mac Dev Playbook

#### Shell

- [ ] Create `~/.zprofile` config file 
- [ ] Check `zsh` version, upgrade if necessary
- [ ] Symlink [`zsh` config](zsh/.zshrc) at `~/.zshrc`
- [ ] Create Keyboard Shortcut for Kitty

#### Programming Language Compilers, Tooling, Etc.

- [ ] [Docker](https://docs.docker.com/get-docker/) - containerized apps
- [ ] [Go](https://go.dev/dl/) - programming language
- [ ] [Rust](https://www.rust-lang.org/learn/get-started) - programming language
- [ ] [pnpm](https://pnpm.io/installation) - JavaScript package manager
- [ ] [poetry](https://python-poetry.org/docs/) - python package manager
- [ ] [Composer](https://getcomposer.org/download/) - PHP package manager
- [ ] [SQLite](https://www.sqlite.org/download.html) - serverless SQL database engine
- [ ] [Dart](https://dart.dev/get-dart) - programming language

#### Browsers

- [ ] [Brave](https://brave.com/)
- [ ] [Firefox](https://www.mozilla.org/en-US/firefox/new/)
- [ ] [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/)
- [ ] [Firefox Nightly](https://www.mozilla.org/en-US/firefox/124.0a1/releasenotes/)
- [ ] [Google Chrome](https://www.google.com/chrome/index.html)
- [ ] [Google Chrome Canary](https://www.google.com/chrome/canary/)
- [ ] [Microsoft Edge](https://www.microsoft.com/en-us/edge?ep=313&form=MA13M0&es=40&ch=1)
- [ ] [Safari Technology Preview](https://developer.apple.com/safari/technology-preview/)
- [ ] [Tor Browser](https://www.torproject.org/download/)

#### Mobile development

- [ ] [Xcode](https://developer.apple.com/xcode/) (App Store) - iOS development
- [ ] [Android Studio/SDK](https://developer.android.com/studio) - Android development
- [ ] [Expo](https://reactnative.dev/docs/environment-setup?guide=native) - React Native
- [ ] [Flutter](https://docs.flutter.dev/get-started/install) - Skia-based mobile development

## References

- [Apple Device Support Tutorials](https://it-training.apple.com/tutorials/apt-support)

## zsh:

- [Z Shell Doc](https://zsh.sourceforge.io/Guide/zshguide.html)
- [No oh-my-zsh config](https://www.youtube.com/watch?v=bTLYiNvRIVI)

Amethyst

- [Getting Started](https://www.youtube.com/watch?v=7Z9-Ry4yGNc) 

Ansible

- [Mac Dev Playbook Example](https://github.com/geerlingguy/mac-dev-playbook)
