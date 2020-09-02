# Cron
* cron - A time based job scheduling service.
* crontab - A Program to create, read,update, and delete your job schedules.
* Use cron to schedule and automate tasks.

# Crontab Format
 ![linux_intermediate](cronjob.PNG?raw=true "Title")

# using the crontab command
* crontab file : Install a new crontab from file
* crontab -l : List your cron jobs
* crontab -e : Edit your cron jobs.
* crontab -r : Remove all of your cron jobs.

```
[adminuser@localhost ~]$ crontab -l
no crontab for adminuser
[adminuser@localhost ~]$
[adminuser@localhost ~]$ vi my-cron
[adminuser@localhost ~]$ cat my-cron
# Run every Monday at 07:00
0 7 * * 1 /opt/sales/bin/weekly-report
[adminuser@localhost ~]$
[adminuser@localhost ~]$
[adminuser@localhost ~]$ crontab my-cron
[adminuser@localhost ~]$ crontab -l
# Run every Monday at 07:00
0 7 * * 1 /opt/sales/bin/weekly-report
[adminuser@localhost ~]$ echo $EDITOR

[adminuser@localhost ~]$ EDITOR=vi
[adminuser@localhost ~]$ crontab -e
crontab: installing new crontab
[adminuser@localhost ~]$
```
