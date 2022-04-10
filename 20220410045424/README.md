# Check API response in python

1. Test if response body contains sth.
```python
if response.text:
    # ...
```

2. Handle error if deserialization fails (because of no text or bad format)
```python
try:
    responses = response.json()
    # ...
except ValueError:
    # no JSON returned
```

3. check that .json() did NOT return an empty dict
```python
if responses:
    # ...
```

4. safeguard against malformed data
```python
try:
    data = responses[some_key][some_index][...][...]
except (IndexError, KeyError, TypeError):
    # data does not have the inner structure you expect
```

5. check if data is actually something useful (truthy in this example)
```python
if data:
    # ...
else:
    # data is falsy ([], {}, None, 0, '', ...)
```

Related:
```
* <https://stackoverflow.com/questions/37605278/how-to-determine-if-my-python-requests-call-to-api-returns-no-data>
```

Tags:
```
#Python #API
```
