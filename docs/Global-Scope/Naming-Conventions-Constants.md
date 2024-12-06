# Naming Conventions : Constants

Global Constant variables should be written with `SCREAMING_SNAKE_CASE`, and should always be within a namespace.  
They should clearly describe what they are, so they should be as long as they need to be.  
Example : 

``` cpp linenums="1"
namespace MAT
{
	constexpr float PI{ 3.14159 };
}
```