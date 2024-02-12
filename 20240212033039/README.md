# Special shell variables

|Special | Variable	 Variable Details |
| ----- | ----- |
|$1 to $n |	$1 is the first arguments, $2 is second argument till $n n’th arguments. From 10’th argument, you must need to inclose them in braces like ${10}, ${11} and so on |
|$0 |	The name of script itself|
|$$ |	Process id of current shell|
|$* |	Values of all the arguments. All agruments are double quoted|
|$# |	Total number of arguments passed to script|
|$@ |	Values of all the arguments|
|$? |	Exit status id of last command|
|$! |	Process id of last command|


Tags:
```
#Linux #shell #variable #shell_variable
```

Related:
```
* https://tecadmin.net/tutorial/bash-scripting/bash-command-arguments/#:~:text=Here%20ARG1%2C%20ARG2%20to%20ARG10,Variable%20Details
```
