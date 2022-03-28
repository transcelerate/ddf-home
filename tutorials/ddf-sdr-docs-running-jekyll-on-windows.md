---
title: Running the DDF Document Repository on Windows using Jekyll
description: Walkthrough on cloning local, opening and running the document repository using Visual Studio Code and Jekyll on Windows
---

## Steps to run the [ddf-sdr-docs](https://github.com/transceleratebiopharmainc/ddf-sdr-docs) repo locally on Windows

Below are the short steps to get up and running on the ddf-sdr-docs repo. You can watch a video of these steps [here](https://www.youtube.com/watch?v=HCd2LSYeOPI).

- Install Visual Studio Code from [here](https://code.visualstudio.com/), picking the **User Installer**
- Install Git for Windows from [here](https://git-scm.com/download/win), accepting the defaults, and choosing Visual Studio Code as the default editor
- Install the Ruby development package from [here](https://jekyllrb.com/docs/installation/windows/)
  - RubyInstaller -> Downloads -> pick the latest "WITH DEVKIT" option (x64)
  - Once installed, there will be a Ruby command window that appears.  Follow the instructions to install the default.
- Once that's done, click start and launch the **Start Command Prompt with Ruby** shortcut
  - Type the following to run `gem install jekyll bundler webrick`
- Open Visual Studio Code, and go to the command palette (CRTL+SHIFT+P)
  - Type in "Clone" and choose "Git: Clone"
  - Enter the url for the ddf-sdr-docs repo - https://github.com/transceleratebiopharmainc/ddf-sdr-docs
    - You will be prompted to select a folder on your computer for the cloned repository
    - You may have to authenticate at this point if the repo is private
    - If not, you'll authenticate when pushing any changes back to GitHub
- Start a new Command Prompt with Ruby
  - Navigate to the folder that the code sits in.  NOTE: A repository subfolder will automatically be created.  You must be at this folder level. 
  - Type the following to run `bundle install`
  - Type the following to run `bundle exec jekyll serve`
- The web server should now be running at [http://127.0.0.1:4000](http://127.0.0.1:4000)
- Configure Git with your username and email to commit changes using the Visual Studio Code editor. 
  - Start a new Command Prompt with Ruby in the same folder above
  - Set your username by typing:  `git config --globaluser.name "FIRST_NAME LAST_NAME"`
  - Set your email address by typing:  `git config --global user.email "MY_NAME@example.com"`
- Make any changes you want in the Visual Studio Code editor, and they will be automatically replicated on the locally served website
- Remember to periodically synchronize updates
