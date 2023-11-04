# This file to used to demonstrate the usage of some common bash commands.

## Table of Contents:

1. [Listing Commands](#listing-commands)
    - [ls](#ls)
    - [lspci](#lspci)
    - [lscpu](#lscpu)
    - [lsblk](#lsblk)
    - [lshw](#lshw)
    - [lsof](#lsof)
2. [Output Commands](#output-commands)
    - [cat](#cat)
    - [less](#less)
    - [more](#more)
    - [wc](#wc)
    - [tee](#tee)

### Listing commands.

- ## ls{#ls}
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

- ## lspci{#lspci}
    - List all PCI devices.
    - #### Options and their description
        - -v --> verbose.
        - -vv --> very verbose.
        - -vvv --> very very verbose.
        - -k --> show kernel drivers.

- ## lscpu{#lscpu}
    - Display information about the CPU architecture
    - #### Options and their description
        - a --> all
        --help
        --version

- ## lsblk{#lsblk}
    - List block devices
    - #### Options and their description
        - -a , --all
        - -l , --list
        - -V , --version

- ## lshw{#lshw}
    - List hardware
    - #### Options and their description
        - -version
        - -help
        - -X --> launch the X11 GUI if available

- ## lsof{#lsof}
    - List open files
    - #### Options and their description
        - An open file may be a regular file, a directory, a block special file, a charac‐
       ter special file, an executing text reference, a library, a stream or a  network
       file  (Internet socket, NFS file or UNIX domain socket.)  A specific file or all
       the files in a file system may be selected by path.
       - In the absence of any options, lsof lists all open files belonging to all active
       processes.

### Output Commands

- ## cat{#cat}
    - Concatenate files and print on the standard output.
    - #### Options and their description
        - --help
        - --version
        - -A --> Show all
        - -E Show $ at end of each line.
        - -T Display tab character as ^I.

- ## more{#more}
    - ==file perusal filter for crt viewing==
    - more is a filter for paging through text one screenful at a time.
    - #### Options and their description
        - -V , --version
        - --help
        - -n --> Specify the number of lines per screenfull.
        - -number --> same as -n
        - +number --> start displaying each file at line `number`.
        - +/string --> string to be searched before displaying.

- ## less{#less}
    - ==Opposite of more.==
    - Less  is a program similar to more(1), but it has many more features.  Less does
       not have to read the entire input file before  starting,  so  with  large  input
       files  it  starts up faster than text editors

- ## wc{#wc}

- ## tee{#tee}

