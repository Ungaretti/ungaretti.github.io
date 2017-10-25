# RED Language

A guide for those who want to get things done.
Windows only! 
Sorry, but that is the vast majority. If you use Linux you probably don't need this guide anyway, and my wife won't let me use her mac.

## Setting up an environment:
This section will explain how to make a nice standalone environment, almost an IDE, that fits on a single file or on a pendrive. After evaluating many free editors, I chose to use Notepad++. It's the best by far. However, it lacks a feature: it has no option to automatically save the file before running it. If you, like me, get annoyed by that, you can fix it installing a plugin named NppExec, but I will not cover this here. Crimson Editor can be configured to save before running and has Rebol syntax hightlighting, but lacks many other nice features that Notepad++ has.

1 - Download Notepad++ from <a href="https://notepad-plus-plus.org/download/v7.5.1.html"> Notepad website </a> . Make sure you download a non-installable version, I suggest the "minimalist package 32-bit x86". No real need for the extras or for a 64 bit version.

<img src="http://ungaretti.github.io/assets/1.jpg">

2 - Create a folder for the environment. I suggest calling it "RedIDE", inside the "Documents" folder.

3 - Unpack Notepad++ in this folder.

4 - Download RED <a href="http://www.red-lang.org/p/download.html"> HERE </a> and unpack it in this same folder.

5 - Donload RED syntax highlight file from <a href="https://github.com/Ungaretti/Notepad-config-file-for-Red-Language"> HERE </a> . Use the download zip button. Unpack it somewhere and move the "Red-lang.xml" file to the RedIDE folder too.

6 - I suggest you also create a "programs" folder inside RedIDE, so you keep your programs and your environment in the same place. You will end up with something like this:

<img src="http://ungaretti.github.io/assets/2.jpg">

7 - Open Notepad++ and goto "Language/Define your language..." . Click on "Import..." and choose the downloaded "Red-lang.xml". A popup will tell you that the import was sucessfull.

<img src="http://ungaretti.github.io/assets/3.jpg">

8 - Check the box "Ignore case" Click in "Save As..." and save as "Red". THEN and add "red" to the "Ext." box (never mind the image below, it's just illustrative, the "Ext." box comes after the save).

<img src="http://ungaretti.github.io/assets/4.jpg">

9 - Open the "Settings/Preferences/Auto Completion" window. Check the boxes for "()", "" "{}" and "[]". If you can't find those in the options, create a "matched pair".

<img src="http://ungaretti.github.io/assets/5.jpg">

9 - Open the "Run/Run.." window and write down the name of the RED executable file you donwloaded folowed by a space and "$(FULL_CURRENT_PATH)", with the quotes. Click on save, give it your favorite shortcut keys and a name like "Red_Run" (remember that  later you may want to add a "Red_Compile" etc.), and clik "OK"

<img src="http://ungaretti.github.io/assets/6.jpg">

10 - Close and reestart Notepad++

11 - Open a new file in Notepad++ and write the code below. Notice it is "Red", not "red", this is an exception as in most cases Red language is case insensitive:
```Red
Red[]
print "Hello world!"
```
12 - Save your program with .red extension ("myprogram.red"). You should see the syntax highlighted. I suggest saving it in the "programsClick "Run/Red_Run". You should see Red's console open up in the center of the screen. 

13 - Move your Notepad++ and your console so that you get a nice environment for developing and THEN close the console in the position you want. This will make it open there next time you run a program.

14 - I strongly suggest you make a copy of your "RedIDE" folder now and save it as "RedIDE_fresh" somewhere, so in case you mess up in the future you won't have to do it all over again.

14 - Happy coding!!


