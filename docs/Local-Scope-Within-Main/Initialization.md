# Initialization

There are several ways to go about `Initialization` within C++.
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

`List Initialization` is preferred between all the above methods.  
There are several reasons for this.  
The Primary reason is for consistency, `Class`, `Aggregate`, etc `Initialization` all use `{}`, having Initialization specifically always be associated with it is useful for legibility. 
In addition `List Initialization`, allows for `Zero-Initialization`.   
This reduces bugs so that variables `Initialized` with no values won't cause bugs as they'll be set to a valid value.