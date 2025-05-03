# Scope

Scope in C++ is marked by `{}`, the categories of this code guideline encapsulate the scopes which are relevant within the majority of Projects and Libraries.  
To properly delimitate different scopes within a given project,  
**All Curly Brackets delimitating Scopes should occupy a new line by itself.**  
Example :
``` cpp linenums="1"
void foo()
{	
	if (check)
	{
		std::cout << "Check One";
		std::cout << "Finshed Checks!";
	}
	
	if (check) 
	{ 
		std::cout << "Code Ran"; 
	}
}
```