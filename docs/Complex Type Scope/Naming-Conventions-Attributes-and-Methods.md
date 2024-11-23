# Naming Conventions : Attributes and Methods
### <u>Private</u>

To differentiate between different `Access specifier scopes`, and code within a function, `Attributes within the Private Scope`, should be `_lowerCamelCase`, `methods` should be `_UpperCamelCase` like the following :  
``` cpp linenums="1"
class GenericInterface 
{
private:

	int _common{};
	float _deltaCommon{};

	void _Init();
}; 
```

### <u>Protected</u>

If there is a `protected specifier`, than `attributes under the protected scope` should