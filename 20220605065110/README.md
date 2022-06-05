# Bash string Operations

|Expression |	Meaning |
|${#string}|	Length of $string|
|${string:position}|	Extract substring from $string at $position|
|${string:position:length}|	Extract $length characters substring from
$string at $position [zero-indexed, first character is at position 0]|
|${string#substring}|	Strip shortest match of $substring from front of $string|
|${string##substring}|	Strip longest match of $substring from front of $string|
|${string%substring}|	Strip shortest match of $substring from back of $string|
|${string%%substring}|	Strip longest match of $substring from back of $string|
|${string/substring/replacement}|	Replace first match of $substring with $replacement|
|${string//substring/replacement}|	Replace all matches of $substring with $replacement|
|${string/#substring/replacement}|	If $substring matches front end of $string, substitute $replacement for $substring|
|${string/%substring/replacement}|	If $substring matches back end of $string, substitute $replacement for $substring|
|expr match "$string" '$substring'	Length of matching $substring* at beginning of $string|
|expr "$string" : '$substring'	Length of matching $substring* at beginning of $string|
|expr index "$string" $substring	Numerical position in $string of first character in $substring* that matches [0 if no match, first character counts as position 1]| 
|expr substr $string $position $length|Extract $length characters from $string starting at $position [0 if no match, first character counts as position 1]|
|expr match "$string" '\($substring\)'|Extract $substring*, searching from beginning of $string|
|expr "$string" : '\($substring\)'|Extract $substring* , searching from beginning of $string|
|expr match "$string" '.*\($substring\)'|Extract $substring*, searching from end of $string|
|expr "$string" : '.*\($substring\)'|Extract $substring*, searching from end of $string|

Tags:
```
#Linux #shell #bash #script #string #string_proccess
```

Related:
```
* https://tldp.org/LDP/abs/html/refcards.html#AEN22728j
```
