# Dropbox Printer

Usage: dropbox-printer [options] basepath

*dropbox-printer* monitors the folder defined in 'basepath' parameter and prints any pdf file added to this path

IMPORTANT: the subfolders' name under 'basepath' will be used as printers' names when the jobs are sent to the printing server

Options:

    -u <user>  Print using the specified username
    -1         One sided printing (default: 2 sided)
    -c         Print in color (default: grayscale)
    -s         Staple
    -h         Show help
    -v         Verbose mode	

Example:
    $APP_NAME /Users/yourusername/Dropbox/PrinterQueue
	
## Suggested usage

Open a terminal and start a screen session:

    $ screen
    
Then run the script

    $ ./dropboxPrinter -s /home/user/Dropbox/PrintQueue/
    
Finally, leave the screen session by pressing "CTRL + A", then "D". To return to the screen session just type "screen -r"