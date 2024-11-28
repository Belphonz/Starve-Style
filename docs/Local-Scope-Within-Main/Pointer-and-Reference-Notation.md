# Pointer and Reference Notation
There's a small bit of contention about how to go about the syntax that should be followed for `pointer` and `reference` type variables Initialization.  
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
`Pointer` variables hold an (RAM DEPENDANT) 8 byte long string of numbers.  
If the pointer points to an integer as an example, their sizes and the data and usage is different. 
`Reference` variables are aliases for already existing variables and as such occupy no space on the RAM. In terms of use they match that of their counterparts, however due to consistency they should be put on the left.