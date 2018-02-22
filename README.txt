This is a slightly modified version of QQtimer for streaming that writes to files.
    
I pulled this version of QQ timer in january 2018, but the updates should work with any version as they are very minor.
    
The updates create text files in a directory of your choosing. The text files contain data for best/current single, MO3, Avg5, Avg12, etc. Additionally there is a time list and a short time list, which contains a fixed number of recent times.

The primary purpose of this is to be used for cube streaming. OBS software can pick up text files to display on stream. This allows you to format the output in whatever way you want, and not to be dependant on how the timer formats the times.



Since javascript doesn't naturally write to local files, these edits use ActiveX with internet explorer. You must run the timer in internet explorer and allow ActiveX to be used. The timer must be run locally.
     
<# Use instructions below are annoying because internet explorer won't prompt for ActiveX to run if you just download the github project and open it. You have to modify something you downloaded yourself. If anyone finds a fix please let me know #>
1. Download QQTimer
	1a. Go To https://www.qqtimer.net/
	1b. Right click -> Save As
	1c. Save in the location you want (Target Location)
2. Create folder for the times
	2a. In same location as where you saved QQTimer. Right Click -> New Folder
	2b. Name "Files" <- Has to be correct name
3. Replace default QQTimer.html with modified version
	3a. Navigate to https://github.com/HaysCubing/StreamQQTimer
	3b. Click "Clone or download" -> Download Zip
	3c. Go to downloads, Right click "StreamQQTimer-master" -> "Extract All"
	3d. Open QQTimer.html in notepad
	3e. Copy all content (Cntrl+A -> Cntrl+C)
	3e. Navigate to location where you downloaded QQTimer in step 1.
	3f. Open original QQTimer.html in notepad
	3g. Paste modified content (Cntrl+A -> Cntrl+V)
4. Use with internet explorer
	4a. Right click QQTimer.html -> Open with Internet Explorer
	4b. Click "Allow blocked content" at bottom of page
	4c. Click "Yes" on the ActiveX Prompt

The timer should now work and write the stats to the files in "Folder"!