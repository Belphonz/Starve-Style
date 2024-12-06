# Initialization

### <u>Initialization Type</u>

There are several ways to go about `initialization` within C++.
``` cpp linenums="1"
int main()
{
	//Copy Initialization
	int a = 5;
	//Direct Initialization
	int b(5);
	//Direct List Initialization
	int c{5};
}
```

`Direct List Initialization` is preferred between all of the above methods.  
There are several reasons for this.  
The Primary reason is for consistency. `Class` and `Aggregate` `initialization` all use `{}`, having `initialization` specifically always be associated with it is useful for legibility. 
In addition `List Initialization`, allows for `Zero-Initialization`.   
This reduces bugs as variables `Initialized` with no values may keep garbage data.

### <u>Multiple Initializations</u>

Within C++ it is possible for you to `Initialise` several variables of the same type within a singular statement.
Example :
``` cpp linenums="1"
int main()
{
	int x{}, y{};
}
```
For legibility’s sake this practice will be strictly banned within this coding guideline.
While I find it reasonable to use this syntax for variables such as `x,y,z` like the above example, it gets quickly out of hand the moment you use variables whose names exceed a singular character in length.   
Due to the aforementioned reason and for the sake of consistency, each  `Initialised` variable should occupy a new line.