﻿`of` is a primitive that allows you to reach into an agent and pull out the value of some variable it owns. Normally, agent variables (such as `color`, `size`, `shape`, as well as variables defined with `<agent>-own` commands) are accessed within an agent context, i.e., within an `ask turtles [...]` or `ask patches [...]` block. `of` will allow you to get to those variables outside of such a block, or to get all the values for each agent in an agentset all at once. 



 `of` is used with a reporter inside a `[]` block, like : 



```[reporter] of agent` or `[reporter] of agentset ```



 For example, if we wanted to get the `pcolor` of the patch at the center of the world, we would say `[pcolor] of patch 0 0`, because `pcolor` is the name of the variable we want to get  and `patch 0 0` is the agent we want to get the variable from. If we wanted to get the `size` values for every turtle, we would write `[size] of turtles` and would get back a list of the size of each turtle. 



Note:  your reporters can be more elaborate than just getting the value of a variable. You can treat the code inside the reporter block as you would any other code in Netlogo and write full expressions within it. For instance, say each turtle had a diameter stored in a `diameter` variable and you wanted to get a list of every turtle's radius. A simple way to do so would be to write `[diameter / 2] of turtles`.