```python3

# I was always in pain, when it occurs 
# that templating languages eventually recreate 
# their own loop, if/else, functions

# so I propose to use the structures of the host languages

#for example in python 

t(<!DOCTYPE html>
<html>)
for item in itemlist:
    t(<li>{item}</li>)
t(</html>)

### the argument of t is written as a result of the template
### all but t(...) part is clasic python

# it is more or less the reverse of usuals template,
# the special syntax is for emmiting string and the code stay real python

# any parenthesis inside t(...) don't need to be escaped, as long they are balanced

```
