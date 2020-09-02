# Viewing Environment variables.
* $ printenv
* $ printenv home

* Environmental variables are case sensitive.

# Creating environmental variables
* Syntax
  1. export VAR = "value"

 ```
 Examples:
  1. export EDITOR="vi"
  2. export TZ="US/Pacific"
  ```

# Removing environmeental variables
* Syntax
  1. unset VAR

```
Example :
unset TZ
```

# Persisting Environment varables
* $cat ~/.bash_profile
* export TZ="US/Central"

# Environment Variables Demo
* printenv
* printenv PATH
* printenv MAIL

# Conclusion
* Environment variables are name/value pairs
* Can change how an application behaves
* View with printenv and echo
* export VAR="value"
* unset VAr
* Persistance via personal initialization files.
* Refer to the man page.





