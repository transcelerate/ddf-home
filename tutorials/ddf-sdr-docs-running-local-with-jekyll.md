---
title: Running the DDF SDR Docs local
description: Walkthrough on getting WSL2, Jekyll running, cloning local, and running the docs repo to develop custom code
# key items
# - if just editing pages, hit '.' on the repo and edit in the browser
# - this is only needed if you're developing liquid custom code, scripting, etc
---

### Installing Git and Visual Studio Code

- Install [Visual Studio Code](https://code.visualstudio.com/insiders/) - making sure to pick the user installer
- Install [VSCode Remote Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)
- Install [Git](https://git-scm.com/downloads) - on the screen for which editor you want to use, pick Visual Studio Code

### Installing Windows Subsystem for Linux on Windows 11 and the Jekyll tooling

- Install WSL on Windows 11 by running "`wsl --install`" in an elevated command prompt, then reboot windows. If you're on Windows 10, follow the instructions from Microsoft at [Install WSL](https://docs.microsoft.com/en-us/windows/wsl/install)
- Once you've rebooted and set your username/password, update the linux distribution
  - `touch .hushlogin`
  - `sudo apt-get update && sudo apt-get -y upgrade`
- Open up Visual Studio Code and open a bash terminal (CTRL + `). Run the following commands:
  - `sudo apt-get install ruby-full build-essential`
  - `sudo gem update`
  - `sudo gem install bundler`
  - `sudo gem install jekyll`
- Clone the repo locally
  - CTRL + SHIFT + P, choose Git: Clone, and enter https://github.dev/transceleratebiopharmainc/ddf-sdr-docs
  - Choose yes to open that directory in a new folder
- In the terminal (CTRL + `) run the following commands:
  - `bundle install`
  - `bundle exec jekyll serve`