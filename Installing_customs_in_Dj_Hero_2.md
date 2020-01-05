Assuming you already have a jailbroken/modded console or an emulator set up, and all the DJH2 files extracted.

[Available customs](https://docs.google.com/spreadsheets/d/12-2cq5ghomO-UDt1xWEqXLt4_f0gP1m7G4o-h4HW1_c/)

# Tools needed

[Notepad++](https://notepad-plus-plus.org/)

[djh\_text\_csv\_convert](https://github.com/shockdude/djhtools/releases/tag/djh_text_csv_convert_v0.41) 

[DJHCP](https://github.com/MatteoGodzilla/DJHCP/releases/tag/v1.0) 

# Formatting TrackListing.xml for easier editing

This is a one-time step.

* Locate TrackListing.xml and **make a backup**
  * TrackListing.xml location: [Wii, PS3, X360]/Audio/Audiotracks/TrackListing.xml

# Installing the Custom

A custom should include the Song Folder(s), "Info for TrackListing.xml", and "Info for TRAC.csv."

See the README.txt included in the custom for more info.

## Setting up the Audiotracks folder

* Navigate to the Audiotracks folder
  * [Wii, PS3, X360]/Audio/Audiotracks/
* Copy the custom's Song Folder into the Audiotracks folder.
  * The Song Folder should contain files like "DJ.fsb" and "DJ_Expert.xmk".
* Open DJHCP, then drag & drop "tracklisting.xml" in the "Add from xml" button
* Drag & drop the "Info for Tracklisting.xml" from the custom's folder into the "Add from xml" button
* Check if at the bottom the custom's song id shows up
* Click "Update file" to export the list to "tracklisting.xml" 


## Setting up the Text folder

* Navigate to the Text folder
  * [Wii, PS3, X360]/Text/
* If you haven't done so already, set up djh_text_csv_convert
  * Save djh_text_csv_convert.exe to the Text folder
  * Run djh_text_csv_convert.exe, it should spit out several CSV files.
* Open TRAC.csv in Notepad++
  * **DO NOT OPEN THESE FILES IN MS EXCEL**, MS Excel can't save these files properly.
* Open the custom's "Info for TRAC.csv." in Notepad++, and copy the contents into the bottom of TRAC.csv
  * Adding newlines at the bottom of TRAC.csv is ok.
* Save TRAC.csv
* Drag-and-drop TRAC.csv onto djh_text_csv_convert.exe

# PS3-only: Rename all files to be upper-case

The PS3 console requires all game filenames to be upper-case or else the game/customs won’t work. Fortunately, this is easily done with a script.

**Warning: Do not run this script outside of the DJ Hero folder. It will rename everything in the folder containing the script.**

Note: Renaming only works properly on NTFS formatted drives. If the script isn’t renaming anything, you’ll need to move your game files to an NTFS drive like your internal hard drive.

* Download [TO_UPPER.BAT](https://drive.google.com/open?id=1ETZe4wT69L1scKskW-4KnLE7o0WycgLd) to PS3\_GAME\USRDIR\
  * [Source](https://stackoverflow.com/questions/43992595/recursively-rename-files-and-subfolders-in-a-folder-using-batch-script) 
* Run TO_UPPER.BAT
