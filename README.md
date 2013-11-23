chats
=====

Python program to archive and analyze google chat logs.

This is a work in progress. I'm interested in taking a look at how IMs affect my work day since our company uses it a lot for communication. There's not much there yet in terms of actual analysis, but the code to pull down your chat, archive them, and make them available to things with is there.

Archiving your chats
====================

Import chat logs using the import_gchats script.

    usage: ./import_gchats [-h] USERNAME [GCHAT\_LOG\_DIR]
     
    Download gchat logs from specified account.
     
    positional arguments:
      USERNAME       Google chat ID of user to fetch the logs of. Typically gmail
                     email address.
      GCHAT\_LOG\_DIR  Directory to save chat logs into. Default: "gchat_logs"
     
    optional arguments:
      -h, --help     show this help message and exit

Gmail configuration
===================

To archive your chats the gmail needs chat logs to be available via IMAP.

1. Under 'Forwarding and POP/IMAP' select the 'Enable IMAP' option.
1. Under 'Labels' check the 'Show in IMAP' box next to 'Chats'.
