# ps Options
* -e : Everything, all processes.
* -f : Full format listing
* -u username : Display username's processes
* -p pid : Display information for PHD.

# Common ps Commands
* ps -e : Display all processes
* ps -ef : Display all processes, full
* ps -eH : Display a processes tree
* ps -e --forest : Display a processes tree.
* ps -u username : Display user's processes.
* pstree : Will show the processes in atree
* top command : Will get the cpu resorces at the top of the list.

# htop -> is also given the cpu resorces in detail.

# Background and Foreground Processes
* bg [ %num] : Background a suspended process.
* fg [ %num] : Foreground a background process.
* kill : Kill a process by job number or PID
* jobs [ %num] : List jobs

# Killing Processes
* ctrl c : Kill the foreground prod.
* kill [ -sig] Pid : Send a signal to a process
* kill -l : Display a list of signals.
* kill 123
* kill -15 123
* kill -TERM 123 , kill -9 123



