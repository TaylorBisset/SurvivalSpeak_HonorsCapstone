# Project Log 

Follow installation instructions for **Virtual Machine (Recommended)** VirtualBox and Xubuntu 

https://www.theodinproject.com/lessons/foundations-installations#step-1-download-virtualbox-and-xubuntu
- Base Memory: 8192 MB 
- Processors: 4 
- Storage: Controller SATA with Xubuntu.vdi 60.00 GB

Follow installation instructions for VSCode 

https://www.theodinproject.com/lessons/foundations-text-editors#step-1-download-vscode

VS Code Extenstions 
- Prettier - Code formatter 
  - Prettier.io 
- Code Spell Checker 
  - streetsidesoftware.com 

## Set up Development Environment 

#### Step 1: Download Flutter SDK (software development kit) 
```
cd ~/Downloads
curl -LO https://storage.googleapis.com/flutter_infra_release/releases/stable/linux/flutter_linux_3.3.10-stable.tar.xz
```

#### Step 2: Extract the SDK 
```
sudo tar xf ~/Downloads/flutter_linux_3.3.10-stable.tar.xz -C /opt
``` 

#### Step 3: Add Flutter to PATH 
```
export PATH="$PATH:/opt/flutter/bin"
echo 'export PATH="$PATH:/opt/flutter/bin"' >> ~/.bashrc
source ~/.bashrc
```

#### Step 4: Verify Installation 
```
flutter doctor
``` 

#### Step 5: Install Dependencies 
```
sudo apt-get update
sudo apt-get install clang cmake ninja-build pkg-config libgtk-3-dev
```

#### Step 6: Download Android Studio 
Web Search: https://developer.android.com/studio#:~:text=Download%20the%20latest%20version%20of%20Android%20Studio
<br> 
##### Linux (64-bit) *android-studio-2024.1.1.11-linux.tar.gz* 
<br> 

#### Step 7: Install Android Studio 
```
cd ~/Downloads
sudo unzip android-studio-ide-*.zip -d /opt
sudo tar -xzvf android-studio-2024.1.1.11-linux.tar.gz -C /opt
sudo /opt/android-studio/bin/studio.sh
```

#### Step 8: Launch and Set up Android SDK 
```
/opt/android-studio/bin/studio.sh
```

#### Step 9: Accept Android Licenses 
```
flutter doctor --android-licenses 
```



<br><br>

## 24 - 26 June 2024
Setup of the programming environment. 
Issues with memory management in the virtual machine. 
Linux working memory allocation research and implementation. 

<br><br> 
- - - - - - - - - - - - - - - - - - - - 

#### *Sample Logs*

### 29 September 2024 
Built the tentative roadmap. 

Emails were sent to instructors to discuss mentorship for this project. 

### 30 September 2024 
Flutter extension was installed for VS Code. 

GitHub repository created for the project. 
