Attention: PrinterWebUI has been renamed to OctoPrint
=====================================================

On January 19th 2013 PrinterWebUI was renamed to OctoPrint, with the repository location change following on January 27th. OctoPrint (formerly known as Printer WebUI) is now located at https://github.com/foosel/OctoPrint. The repository can be found at https://github.com/foosel/OctoPrint.git.

If you did checkout OctoPrint from its previous location at https://github.com/foosel/PrinterWebUI.git, you'll have to
update your so-called remote references in git in order to make 'git pull' use the new repository location as origin.

To do so you'll only need to execute the following command in your OctoPrint/PrinterWebUI folder:

    git remote set-url origin https://github.com/foosel/OctoPrint.git

After that you might also want to rename your base directory (which probably still is called 'PrinterWebUI') to 'OctoPrint'
and delete the folder 'printer_webui' in your base folder (which stays there thanks to Python's compiled bytecode files
even after a rename of the Python package to 'octoprint').

After that you are set, the configuration files are migrated automatically :)