
#inotifylog  

A Simple inotify event logger. So single-use it's bordering on proof-of-concept

Uses,`Linux::Inotify2`  which is `liblinux-inotify2-perl` in Debian.

#USAGE:

    inotifylog [options] [file1 file2 file3 ...]

Will set up an inotify2 watcher on each of the listed files/dirs, logging
received events.

Options:

  --exclude [file]
      Exclude files whose names match pattern [file] from the output. 

  --help
      Display this help and exit

  --mask-help
     Display a reference to the meanings of the masks in the logs, and exit.

  --syslog
     Log to syslog rather than STDOUT

