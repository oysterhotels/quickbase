quickbase
=========

Simple Python interface to the [Intuit QuickBase API](http://www.quickbase.com/api-guide/index.html), as used by [Oyster.com](http://www.oyster.com/).

Simple example:

```python
>>> import quickbase
>>> client = quickbase.Client(username, password, database='abcd1234')
>>> client.do_query("{'6'.EX.'Foo'}", columns='a')
[{'record_id': 1234, ...}]
>>> client.edit_record(1234, {6: 'Bar'}, named=False)
1
```

See the docstring comments in the code for more details and the [QuickBase API docs](http://www.quickbase.com/api-guide/index.html) for more details.
