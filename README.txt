This is a slightly modified version of QQtimer for streaming that writes to files.
    
I pulled this version of QQ timer in january 2018, but the updates should work with any version as they are very minor.

    

The updates create text files in a directory of your choosing. The text files contain data for best/current single, MO3, Avg5, Avg12, etc. 
    
Additionally there is a time list and a short time list, which contains a fixed number of recent times.

    


    

Since javascript doesn't naturally write to local files, these edits use ActiveX with internet explorer. You must run the timer in internet explorer and allow ActiveX to be used. The timer must be run locally.
     
    

To use, download and save locally. Search QQtimer.html for "WriteToFileReplace". Here replace path 'FileRootPath' with the path that you want the text files to be written to. 
Note: in javascript you need 2 backslashes per backslash in the filename. Reference the dummy filepath for info.
Open QQtimer.html in internet explorer, and allow activeX. Setup OBS to read the text files.

If you want to look at the modified versions of code, search "WriteToFile", all modified instances have comments wrapped with this phrase.