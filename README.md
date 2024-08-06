# VRED-Downloads
This is a repositor for downloadable files for VRED.

To compile the UserPluginDemo example do the following:

Using Visual Studio 2017 (or higher)

- Open a Visual Studio 2017 (or higher) x64 Developer Command Prompt
- change the current directory to ...\VREDUserPlugin-xx.x\example
- run nmake

Using mingw64

- change the current directory to ...\VREDUserPlugin-xx.x\example
- open windows cmd and execute: g++.exe -static-libgcc -static-libstdc++ -shared vrUserPluginDemo.cpp -I../include -o vrUserPluginDemo.dll

There are two ways to install the plugin.
1. Set the VRED_USER_PLUGINS_PATH environment variable to the path of the plugin e.g. ...\VREDUserPlugin-xx.x\bin"
2. Copy vrUserPluginDemo.dll to C:\Program Files\Autodesk\VREDPro-xx.x\lib\plugins\WIN64\UserPlugins

execute VRED
