# extvar
External Variables for Python
# example
```
#in this example I will use extvar to store settings for a gibberish generator
import extvar
from random import randint

letters = [ 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z' ]
word = ""

for i in range(int(extvar.getv("length"))): # this "length" variable is stored as (Script's Folder)/ExtVars/length.var
    word += letters[randint(0, 25)]

print(word)
```
# extvar.mkpth():
creates the directory where the extvariables are stored
# extvar.getv(varname):
gets an extvariable
# extvar.setv(varname, txt):
sets an extvariable
# extvar.addv(varname, txt):
adds text to an extvariable
