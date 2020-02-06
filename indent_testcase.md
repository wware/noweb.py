# Test Case for Python indentation

I'm curious to see if this tool supports indentation, and if it doesn't, how hard it
would be to add that.

```
<<Puppy class definition>>=
class Puppy(object):
    <<Speak method for puppy>>
@
```

and here is a method file for our class.

```
<<Speak method for puppy>>=
def speak(self):
    print "Woof woof"
@
```

and let's make sure to

```
<<Exercise the puppy>>=
p = Puppy()
p.speak()
@
```

Here's how the pieces we have discussed fit together:

```
<<indent_testcase.py>>=
#! /usr/bin/env python

<<Puppy class definition>>
<<Exercise the puppy>>
@
```
