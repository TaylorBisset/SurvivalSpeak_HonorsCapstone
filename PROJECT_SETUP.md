# Project Setup Instructions

## Step 1: Set Up Virtual Machine

### Install VirtualBox and Xubuntu

1. Follow the installation instructions for VirtualBox and Xubuntu:
   [VirtualBox and Xubuntu Installation Guide](https://www.theodinproject.com/lessons/foundations-installations#step-1-download-virtualbox-and-xubuntu)
2. Configure the virtual machine:
   - **Base Memory:** 8192 MB
   - **Processors:** 4
   - **Storage:** Controller SATA with Xubuntu.vdi *60.00* GB

## Step 2: Install Visual Studio Code

### Download and Install VSCode
1. Follow the installation instructions for Visual Studio Code:
   [VSCode Installation Guide](https://www.theodinproject.com/lessons/foundations-text-editors#step-1-download-vscode)

### Install VS Code Extensions
1. Prettier - Code formatter ([Prettier.io](https://prettier.io))
2. Code Spell Checker ([streetsidesoftware.com](https://streetsidesoftware.com))
3. Live Server ([Ritwick Dey](https://ritwickdey.com))
4. GitLens — Git supercharged ([gitkraken.com](https://gitkraken.com))
5. Flutter ([dartcode.org](https://dartcode.org))
6. Dart ([dartcode.org](https://dartcode.org))
7. HTML CSS Support ([ecmel](https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css))
8. ESLint ([microsoft.com](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint))
9. JavaScript Debugger (Nightly) ([microsoft.com](https://marketplace.visualstudio.com/items?itemName=ms-vscode.js-debug-nightly))
10. Path Intellisense ([christiankohler.net](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense))
---
## Step 3: Set Up Development Environment

### Update and Install Essential Packages
```
sudo apt-get update
sudo apt-get install git
git --version
```
```
export PATH="$PATH:/usr/bin"
source ~/.bashrc
```
```
sudo apt install clang cmake ninja-build pkg-config
sudo snap install curl
```
### Install Java Development Kit
```
sudo apt update
sudo apt install openjdk-8-jdk
java -version
```
```
export JAVA_HOME=/usr/lib/jvm/openjdk-8
export PATH=$JAVA_HOME/bin:$PATH
source ~/.bashrc
```
### Install GTK Library
```
sudo apt install libgtk-3-dev
sudo apt install libgtk-3-dev
dpkg -l libgtk-3-dev
```
## Step 4: Install Flutter SDK
### Download and Extract Flutter SDK
```
cd ~/Downloads
curl -LO https://storage.googleapis.com/flutter_infra_release/releases/stable/linux/flutter_linux_3.3.10-stable.tar.xz
sudo tar xf ~/Downloads/flutter_linux_3.3.10-stable.tar.xz -C /opt
```
### Add Flutter to PATH
```
export PATH="$PATH:/opt/flutter/bin"
echo 'export PATH="$PATH:/opt/flutter/bin"' >> ~/.bashrc
source ~/.bashrc
```
### Verify Installation
```
flutter doctor
```
### Install Flutter Dependencies
```
sudo apt-get update
sudo apt-get install clang cmake ninja-build pkg-config libgtk-3-dev
```
## Step 5: Install Android Studio
## Download Android Studio
Visit the Android Studio download page and download the latest Linux (64-bit) version: android-studio-2024.1.1.11-linux.tar.gz.
### Install Android Studio
```
cd ~/Downloads
sudo tar -xzvf android-studio-2024.1.1.11-linux.tar.gz -C /opt
sudo /opt/android-studio/bin/studio.sh
```
### Launch and Set Up Android SDK
```
/opt/android-studio/bin/studio.sh
```
### Accept Android Licenses
```
flutter doctor --android-licenses
```
