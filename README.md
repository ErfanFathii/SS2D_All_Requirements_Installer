# SS2D_All_Requirements_Installer
Shell Script for installing all of the SS2D requirements on Wsl/Ubuntu20.04 or later

![License](https://img.shields.io/github/license/ERFANFATHI-E/SS2D_All_Requirements_Installer?color=blue)

![image](https://user-images.githubusercontent.com/1832537/49242985-f69a3c00-f3ea-11e8-97f5-9b0bfdfc4e1c.png)

- The RoboCup Soccer Simulator: http://github.com/rcsoccersim/
- RoboCup Official Homepage: http://www.robocup.org/
- Install qt5 https://wiki.qt.io/Install_Qt_5_on_Ubuntu

## :package: Download

- QT  

```
sudo apt-get install build-essential mesa-common-dev libfontconfig1 libglu1-mesa-dev -y
```
```
sudo apt update 
sudo apt install -y qtcreator qtbase5-dev qt5-qmake cmake vulkan-sdk qt6-base-dev qt6-base-private-dev qt6-declarative-dev qt6-declarative-private-dev qt6-tools-dev qt6-tools-private-dev qt6-scxml-dev qt6-documentation-tools libqt6core5compat6-dev qt6-tools-dev-tools qt6-l10n-tools qt6-shader-baker libqt6shadertools6-dev qt6-quick3d-dev qt6-quick3d-dev-tools libqt6svg6-dev libqt6quicktimeline6-dev libqt6serialport6-dev build-essential cmake ninja-build git clang-15 clangd-15 libclang-15-dev libgl1-mesa-dev libvulkan-dev libxcb-xinput-dev libxcb-xinerama0-dev libxkbcommon-dev libxkbcommon-x11-dev libxcb-image0 libxcb-keysyms1 libxcb-render-util0 libxcb-xkb1 libxcb-randr0 libxcb-icccm4

```
```
wget https://download.qt.io/new_archive/qt/5.7/5.7.0/qt-opensource-linux-x64-5.7.0.run
```
```
chmod +x qt-opensource-linux-x64-5.7.0.run ./qt-opensource-linux-x64-5.7.0.run
```

- File
```
git clone https://github.com/ERFANFATHi-E/SS2D_All_Requirements_Installer
```


## :star: Just Use!

 If you are using ubuntu20.04 run the following command and ignore Qt installation method. :
 
```
sudo apt install qt5-default
```
- Recommended commands for ubuntu 22.04 :

```
sudo apt install -y qtcreator qtbase5-dev qt5-qmake cmake
```

Run as administrator 
 
```
./MakeInstall
```

## :arrow_forward: Using the Server

To start only the server either type `./rcssserver` from the directory
containing the executable or `rcssserver` if you installed the executables
in your PATH.
```bash
rcssserver
```
rcssserver will look in your home directory for the configuration files:

- ~/.rcssserver/server.conf
- ~/.rcssserver/player.conf
- ~/.rcssserver/CSVSaver.conf
- ~/.rcssserver-landmark.xml  (optional)

If these files do not exist they will be created and populated with default values.

To start the sample client, type `./rcssclient` or `rcssclient` as above.  Then type
`(init sample)`.  This will connect the sample client to the server.  You can then
type in client command to move the client around the field. You will also need a
monitor to be able to see whats happening on the field.

If you installed the server and the monitor successfully, you can use the
`rcsoccersim` script. To start the simulator (server and monitor) either type:

```bash
rcsoccersim
```

# Any problems
fathye897@gmail.com
