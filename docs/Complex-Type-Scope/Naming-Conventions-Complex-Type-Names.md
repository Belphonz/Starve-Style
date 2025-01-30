# Naming Conventions : Complex Type Names
### <u>Classes </u>

`C++ Classes` should be named using `PascalCase`, this is to differentiate them from `structs and user defined aliases` :
``` cpp linenums="1"
class GenericInterface 
{

}; 
```

In addition, due to the fact that the Instantiation of Classes shouldn't happen too often, the upmost clarity can be pursued with the **names of Classes being several whole words such as** : `MemoryMatrix`.   
However, if very well known shorthands can be used instead, then they should be.

### <u>Structs </u>

`C++ Structs` should be named using `camelCase` :
``` cpp linenums="1"
struct shapeBundle 
{

}; 
```

`structs` within C++ are functionally the same as `Classes`, however in practice I will be using `structs` as **bundles of data** while I'll be using `Classes` as **interfaces**. 
Since `structs` will be treated close to primitive types, their naming convention should mirror/be close to it hence `camelCase`.  

Since `structs` on average are instantiated more often than `Classes` and due to the fact they're simpler in function than a `Class`, their names should be one word or several shorthands. Except for exceptional cases where alternatives cannot be found, `structs` **should be 2 short words maximum in length.**

`unions` should also be `camelCase` since they possess a similar role as `structs` within a program in most use cases. They should also use the same rules in terms of length as `structs`.