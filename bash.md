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
