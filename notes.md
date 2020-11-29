<b> A <i>namespace</i> is a space (understood in a non-physical context) in which some names exist and the names don't conflict 
with each other (i.e., there are not two different objects of the same name). We can say that each social group is a 
namespace - the group tends to name each of its members in a unique way (e.g., parents won't give their children the 
same first names). </b>
To enter the namespace of the module we must do the following:

```
import math
print(math.sin(math.pi/2))
```

```
import math

def sin(x):
    if 2 * x == pi:
        return 0.99999999
    else:
        return None

pi = 3.14
print(sin(pi/2))
print(math.sin(math.pi/2))
```
<b>or we can do the following:</b>
```
from math import sin, pi
print(sin(pi/2))
```

#### "from module import *": 
Is it unsafe? Yes, it is - unless you know all the names provided by the module, you may not be able to avoid name 
conflicts. Treat this as a temporary solution, and try not to use it in regular code.

<b>To see all the entities in a module after importing it you can use the "dir(module name)" and it gives the list of
all the entities.</b>

#### Random module:
```
from random import choice, sample

my_list = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

print(choice(my_list))
print(sample(my_list, 5))
print(sample(my_list, 10))
```
#### Platform and Machine and Processor and System:
```
from platform import platform

print(platform())
print(platform(1))
print(platform(0, 1))
```
And 
```
from platform import machine 

print(machine())
```
And
```
from platform import processor, system, version

# the os version
print(version())
print(system())
print(processor())
```
