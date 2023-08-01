```python3

### another way to create a template
### the argument of t is written as a result of the template
### all but t(...) part is clasic python

t(<!DOCTYPE html>
<html>)
for item in itemlist:
    t(<li>{item}</li>)
t(</html>)

## I find it, a lot more pleasant to read than the same  jinja template

<!DOCTYPE html>
<html>
{% for item in items %}
  <li>{{item}}</li>
{% endfor %}

# it is more or less the reverse of classic template,
# the special syntax is for emmiting string and the code stay real python

# There is no attempt to add this syntax to cpython,
# but having separate file exactly like jinja template

# the exact syntax is left to bikeshedding

# any parenthesis inside t(...) don't need to be escaped, as long they are balanced

```
