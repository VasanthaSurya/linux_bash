# Introduction to bash.

- Sha bang or hash bang is the first line of the bash script.

- It determines which shell should be used to execute it.

- If it is not mentioned , some bash functions may not work properly.

- It is usually "/bin/bash" or "/usr/bin/bash"

---
### Some keywords in bash script are:

---

1. If
2. then
3. else
4. elif
5. fi
6. for 
7. do    
8. done
9. while
10. case
11. esac
12. declare
13. until
14. select
15. time
16. coproc

---- 

### Some looping statements are as follows:

---

```
    for [[ Expression ]];do
      #For loop statements
    done
      (or)
    for name [ in [words ...]]; do commands ; done
      (or)
    for (( expr1;expr2;expr3 )); do commands ; done
```

```
    while [[ Expression ]]
    do
        #while loop statements
    done
```

```
    until [[ Expression ]]
    do
        #while loop statements
    done
```

---

### The conditional statements are as follows.

---

```
    if (( Expression ))
    then
        #consequence commands
    fi
```

```
    if (( Expression ))
    then
        #consequence commands
    else
        #consequence commands
    fi
```

```
    if (( Expression ))
    then
        #consequence commands
    elif (( Expression))
        #consequence commands
    else
        #consequence commands
    fi

```

```
    case word in 
        pattern1 ) command list ;;
        pattern2 ) command list ;;
        * ) #for all other cases (derfault case) command list ;;
    esac
```

```
    select name [in words ...];do commands break ;done
```

---

### Grouping commands in bash:

> Bash provides two ways to group list of commands.

```    
    1. ( list )
        Placing a list of commands between parentheses forces the shell to create a subshell .
        And each of the commands in list is executed in that subshell environment. 
        Since the list is executed in a subshell, variable assignments do not remain in effect after the subshell completes.
```

```
    2. { list; }
        Placing a list of commands between curly braces causes the list to be executed in the current shell context. 
        No subshell is created. 
```

--- 

### Some definitions you should know.

> ### metacharacter
>> - A character that, when unquoted, separates words. A metacharacter is a space,tab, newline, or one of the following characters: ‘|’, ‘&’, ‘;’, ‘(’, ‘)’, ‘<’, or ‘>’.
> ### signal
>> - A mechanism by which a process may be notified by the kernel of an event occurring in the system.
> ### job
>> - A set of processes comprising a pipeline, and any processes descended from it,that are all in the same process group.
> ### field
>> - A unit of text that is the result of one of the shell expansions. After expansion,when executing a command, the resulting fields are used as the command name and arguments.
> ### builtin
>> - A command that is implemented internally by the shell itself, rather than by an executable program somewhere in the file system.
> ### exit status
>> - The value returned by a command to its caller. The value is restricted to eight bits, so the maximum value is 255.

---

### Points to remember.

> #### asynchronous commands:
> - If a command is terminated by the control operator ==‘&’==, the shell executes the command asynchronously in a subshell.
> - This is known as executing the command in the background,and these are referred to as asynchronous commands.
> - The shell does not wait for the command to finish, and the return status is 0.

> #### AND and OR
> 1. **command1 && command2**
> - command2 is executed if, and only if, command1 returns an exit status of zero.
> 2. **command1 || command2**
> - command2 is executed if, and only if, command1 returns a non-zero exit status.

> #### Shell Functions
> :arrow_right: Shell functions are a way to group commands for later execution using a single name for the group.
> :arrow_right: Shell functions are executed in the current shell context; no new process is created to interpret them.
> ``` 
>    Functions are declared using the syntax:
>        fname () compound-command [ redirections ]
>                            (or)
>        function fname [()] compound-command [ redirections ]
>```
> :arrow_right: will be continued .... 

> #### Process
> - A process is simply an instance of one or more related tasks (threads) executing on your computer. 
> - If we are running a process in background, it means it become detached from the shell.
---
| **Process Type** | **Description** | **Example** |
| ---- | -------- | ---- |
| Interactive Process | Need to be started by user, either by command line or gui. | firefox, bash, top |
| Batch Process | Automatic processes which are scheduled and then detached from the terminal. | updatedb, idconfig |
| Deamons | Server processes that run continuously.Many lauch during system startup. | httpd, sshd |
| Threads | Light weight process . | firefox, gnome-terminal-server |
| Kernel Threads| Kernel tasks that users neither start nor terminate and have little control over. | kthreadd, migration, ksoftirqd |
---
> - At any given time, there are always multiple processes being executed.
> - The OS keeps track of them by assigning a unique id called PID.
> - It is used to track process state, CPU usage, memory and where it is located in memory.
---
| ID Type | Description |
| ---- | -------- |
| Process ID(PID) | Unique process ID number. |
| Parent Process ID(PPID) | Parent that started the process. If parent , it refers to the adoptive process. |
| Thread ID(TID) | Thread ID number. This is the same as the PID for single-threaded processes. For a multi-threaded process, each thread shares the same PID, but has a unique TID.|
---
>