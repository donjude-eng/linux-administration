# Customizing the shell prompt
* use an environment variable to customize
* Bash , ksh, and sh use $PS1.
* Csh, tcsh and zsh use $prompt.

# Customizing the Prompt with PS.
* \d : Date in
* \h : hostname up to the first period
* \H : Hostname
* \n :Newline
* \t : Current time in 24-hour HH:MM:SS format
* \T : Current time in 12 hours/

# IP Check - ifconfig
# Shutdown - sudo shutdown -h now

* vi .bash profile (to get the the bash)
# My custom prompt - PS1="[persist \u@\h\w]\$"

# Summary
* An environment variable customizes the prompt.
* To persist changes, set the environment varaible in your dot files.



