# Pointer and Reference Notation

There's a small bit of contention about how to go about syntax for `pointer` and `reference` type variable initialization.  
The 2 main ways of Initialization are the following :
``` cpp linenums="1"
int main()
{
	int* ptr{};
	int *ptr{};
}
```

The Notation that the Starve Style Guideline will be adopting is the former : `int* ptr{};`.
The reasons for this is simply that I consider that pointer and reference type variables as their own type, distinct from their original variants.  

`pointer` variables hold an (ARCHITECTURE DEPENDANT) 8 byte long string of numbers.  
If the pointer points to an integer as an example, their sizes, data and usage will vary.  
`reference` variables are aliases for already existing variables and as such occupy no space on the RAM. In terms of the various factors they match that of their counterparts, however for consistency reasons they should be put on the left.