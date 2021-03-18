﻿`other` reports an agentset which is the same as the input agentset but omits the asking agent. In other words, it excludes itself from the resulting agentset. For example:



```
show count turtles-here
=> 10
show count other turtles-here
=> 9  
```


shows how one agent, the original turtle who called the command, is excluded from the agentset, resulting in the final count of "9". `other` is often useful when we want our agents to interact with other agents. For example,  



```ask turtles [ if any? turtles-here [```

```								set color red ] ]```



 would make all the turtles red because `turtles-here` reports the original turtle as well. There is always at least 1 turtle when we use `turtles-here`. However, if we write 



```ask turtles [if any? other turtles-here [```

```								set color red ] ]```



 only the turtles who have another turtle on the same patch would turn red. 
