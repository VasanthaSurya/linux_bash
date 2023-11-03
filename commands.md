# This file to used to demonstrate the usage of some common bash commands.

### Listing commands.

- ## ls
    - List direcotory content.
    - #### Options and their description
        - -a --> display all files that including starting with '.'.
        - -A --> same as -a but exclude . and .. directory.
        - -B --> Ignore backups.
        - -c --> sort by last modified time.
        - -C --> list entries by column.
        - -d --> list dictionaries.
        - -f --> do not sort.
        - -h --> with -l and -s print size in human redable format.
        - -i --> print index number of each file(inode).
        - -l --> long listing format.
        - -r --> reverse order while sorting.
        - -R --> list subdirectories recursively.
        - -s --> size of each file.
        - -S --> sort by file size (descending).
        - -t --> sort by time(newest first).
        --help
        --version

- ## lspci
    - List all PCI devices.
    - #### Options and their description
        - -v --> verbose.
        - -vv --> very verbose.
        - -vvv --> very very verbose.
        - -k --> show kernel drivers.

- ## lscpu
    - Display information about the CPU architecture
    - #### Options and their description
        - a --> all
        --help
        --version

- ## lsblk
    - List block devices
    - -a , --all
    - -l , --list
    - -V , --version

- ## lshw
    - List hardware
    - #### Options and their description
        - -version
        - -help
        - -X --> launch the X11 GUI if available

- ## lsof
    - List open files
    - #### Options and their description
        - An open file may be a regular file, a directory, a block special file, a charac‐
       ter special file, an executing text reference, a library, a stream or a  network
       file  (Internet socket, NFS file or UNIX domain socket.)  A specific file or all
       the files in a file system may be selected by path.
       - In the absence of any options, lsof lists all open files belonging to all active
       processes.

### Output Commands

- ## cat
    - Concatenate files and print on the standard output.
    - #### Options and their description
        - --help
        - --version
        - -A --> Show all
        - -E Show $ at end of each line.
        - -T Display tab character as ^I.