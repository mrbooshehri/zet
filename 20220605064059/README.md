# Bash parameter Substitution and Expansion

|Expression |	Meaning |
|:--------- | :------ |
|${var} |	Value of var (same as $var) |
|||
|${var-$DEFAULT} |	If var not set, evaluate expression as $DEFAULT *|
|${var:-$DEFAULT}|	If var not set or is empty, evaluate expression as $DEFAULT *|  
|||
|${var=$DEFAULT} |	If var not set, evaluate expression as $DEFAULT * |
|${var:=$DEFAULT}	| If var not set or is empty, evaluate expression as $DEFAULT * |  
|||
|${var+$OTHER} |	If var set, evaluate expression as $OTHER, otherwise as null string |
|${var:+$OTHER} |	If var set, evaluate expression as $OTHER, otherwise as null string |
|||
|${var?$ERR_MSG} |	If var not set, print $ERR_MSG and abort script with an exit status of 1.*|
|${var:?$ERR_MSG}	If var | not set, print $ERR_MSG and abort script with an exit status of 1.*|
|||
|${!varprefix}	Matches | all previously declared variables beginning with varprefix |
|${!varprefix@} |	Matches all previously declared variables beginning with varprefix |

\* If var is set, evaluate the expression as $var with no side-effects.
# Note that some of the above behavior of operators has changed from earlier versions of Bash.

Tags:
```
#Linux #bash #scripts #shell #shell_paramter
```

Related
```
* https://tldp.org/LDP/abs/html/refcards.html#AEN22728
```
