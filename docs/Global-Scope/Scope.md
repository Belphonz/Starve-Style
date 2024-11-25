Scope in C++ is marked by `{}`, the categories of this code guideline encapsulate the scopes which are relevant within the majority of Projects and Libraries.  
To properly delimitate different scopes within a given project,  
**All Scopes should occupy a new line without any other code on it.**
Example :
``` cpp linenums="1"
void foo()
{
	if (check)
	{
		std::cout << "Code Ran";
	}
}
```