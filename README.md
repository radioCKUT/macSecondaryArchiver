# macSecondaryArchiver
scripts to control mac
Archiver CKUT Mac mini Folder Action "Delete 7 day old BUTT.workflow" is a folder action .workflow document created in Automator.  It is stored in Users/ckutsys/Library/Workflows/Applications/Folder Actions.  The .workflow file is best accessed by right clicking any folder and selecting  "Folder Actions Setup…" at the bottom of the menu. This will launch the Folder Action Setup application, which manages folder actions and their associated folders.  one can then select the  "Delete 7 day old BUTT.workflow" and click [Edit Workflow] to edit the workflow in Automator.  

The  "Delete 7 day old BUTT.workflow" is launched when files or folders are modified in /Users/ckutsys/Music/BUTT Archives, and runs an applescript (within Automator).  The applescript deletes all files whose modification date is greater than modDate (7) days before the current date and time.

An applescript file that contains the same script as the .workflow file has been included in the contents of this folder as a reference for future changes to the .workflow file.

in order to run applescript from automator one must include the additional lines of code 
{
on run {input, parameters}
	--Applescript goes here
	return input
end run
}

please note that applescript directory structure conventions use : rather than / to separate file and folder hierarchies (e.g. Macintosh HD/Users/ckutsys/Library becomes Macintosh HD:Users:ckutsys:Library)
