## Processes

A process represents an instance of a program running. You can run multiple instances of   
a single program by creating multiple processes. Anything that is running has a process,   
and understanding how to manage your processes will keep you in control of your computer.   

`top` show all active processes in an interactive interface   
`ps` show processes' with statuses(not interactive, only prints)   

  * `ps aux` show all processes with statuses   

`Ctrl + Z` stop(pause) the active process by sending STOP signal   

  * `fg` bring a job to the foreground (fg: foreground)   
    * `fg` (switch latest paused job)   
    * `fg #P_ID` (switch numbered jobs, we can see job's number using jobs commmand)   
  * `jobs` list jobs   

`Ctrl + C` terminate(exit) active process by sending TERM signal   

* `kill` send a signal to a process   
  * Example: `kill <signal> P_ID` (default signal: TERM)   

__Signals__   

* `STOP` stop(pause) a process   
* `TERM` request a process terminate normally   
* `KILL` or `9` force a process to exit   

_Examples_:   

```terminal
  >> kill -SIGKILL #P_ID   
  >> kill -KILL #P_ID   
  >> kill -9 #P_ID   

  >> kill -SIGSTOP #P_ID   
  >> kill -STOP #P_ID   

  >> kill -SIGTERM #P_ID   
  >> kill -TERM #P_ID   
```
