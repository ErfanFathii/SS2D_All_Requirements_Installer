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

 If you are using ubuntu20.04 :
 
```
sudo apt install qt5-default
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
