# Why not `scriptname`? 

Why not simply invoke the script with scriptname? If the directory you are in ($PWD) is where scriptname is located, why doesn't this work? This fails because, for security reasons, the current directory (./) is not by default included in a user's $PATH. It is therefore necessary to explicitly invoke the script in the current directory with a ./scriptname.
