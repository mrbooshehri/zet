# re module vs re object

There are two ways to use regular expressions in python

1. re module
```python
imprt re
re.findall(REGEX_PATTERN, STRING)
```
1. re Object
```python
reg_obj = re.compile(REGEX_PATTERN)
reg_obj.findall(STRING)
```
