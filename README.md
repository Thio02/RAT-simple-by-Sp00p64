# DiscordRAT
Discord Remote Administration Tool fully written in Python3.

This is a RAT controlled over Discord with over 20 post exploitation modules.

## **Disclaimer:**

This tool is for educational use only, the author will not be held responsible for any misuse of this tool.\
This is my first project on github as such it is far from perfect,I will listen to any criticism as long as it is constructive.

# Credits

This project was originally made by https://github.com/Sp00p64/DiscordRAT, this entire readme.md is made by him too.
Credit goes to him for all the original modules and readme.md

## **Setup Guide:**
You will first need to register a bot with the Discord developer portal and then add the bot to the Discord server that you want to use to control the bot (make sure the bot has administrator privileges in the Discord server).
Once the bot is created copy the token of your bot and paste it at line 20.

Install requirements :
```
pip3 install -r requirements.txt
```
Then if the steps above were successful, you can launch the python file by executing ```python DiscordRAT```. It will create a new channel and post a message on the server with a generated session number.\
Now your bot should be available to use ! 

**Requirements:**\
Python3,Windows(x64)

## **Modules**
```
Availaible commands are :
--> !message = Show a message box displaying your text / Syntax  = "!message example"
--> !shell = Execute a shell command /Syntax  = "!shell whoami"
--> !window = Get infected computer user current active window
--> !voice = Make a voice say outloud a custom sentence / Syntax = "!voice test"
--> !admincheck = Check if program has admin privileges
--> !sysinfo = Gives info about infected computer
--> !history = Get computer navigation history
--> !download = Download a file from infected computer
--> !upload = Upload file from website to computer / Syntax = "!upload file.png" (with attachment)
--> !cd = Changes directory
--> !write = Type your desired sentence on infected computer
--> !wallpaper = Change infected computer wallpaper / Syntax = "!wallpaper" (with image attachment)
--> !clipboard = Retrieve infected computer clipboard content
--> !geolocate = Geolocate computer using latitude and longitude of the ip adress with google map / Warning : Geolocating IP adresses is not very precise
--> !startkeylogger = Starts a keylogger / Warning : Likely to trigger AV 
--> !stopkeylogger = Stops keylogger
--> !dumpkeylogger = Dumps the keylog
--> !volumemax = Put volume at 100%
--> !volumezero = Put volume at 0%
--> !idletime = Get the idle time of user's on target computer
--> !sing = Play chosen video in background
--> !stopsing = Stop video playing in background
--> !blockinput = Blocks user's keyboard and mouse / Warning : Admin rights are required
--> !unblockinput = Unblocks user's keyboard and mouse / Warning : Admin rights are required
--> !screenshot = Get the screenshot of the user's current screen
--> !exit = Exit program
```
## **Advice:**
If you have problems with the installation of win32api or other modules , try installing it in a python virtual environment.\
Please avoid opening issues about module related errors as it is related to your python install and not a problem inherent of DiscordRAT.\
If you encounter "AttributeError: module 'enum' has no attribute 'IntFlag'" while compiling to Pyinstaller please do :
```
pip uninstall enum34
```
