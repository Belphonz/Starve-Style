# Naming Conventions : Variables

Variables should be written in `camelCase`.  
In terms of length, they should be 1–2 words generally so they don't occupy too much space. They should be short, simple descriptions of what data is stored within.  
While this is said, I generally think that `ptr`suffixes/prefixes to Variables are unneeded as even though they are by definition descriptive, the variable in question tends to be used the same as any other variable.  
However, if any pointer variable when being used heavily deals with pointer arithmetic or any such pointer specific operations, than its name should reflect that.  
Example : 
``` cpp linenums="1"
int main()
{
	int addressStep{3};
	int* unparsedData{new int{10}};

	for (size_t i{0}; i < sizeof(int); ++i)
	{
		//code here
	}
}
```

