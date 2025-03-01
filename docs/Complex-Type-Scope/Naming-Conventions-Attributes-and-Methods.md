# Naming Conventions : Attributes and Methods
### <u>Private</u>

To differentiate between different `Access specifier scopes`, and code within a function, `Attributes within the Private class Scope`, should be `_camelCase`, `methods` should be `_PascalCase`.
Example :  
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

If there is a `protected specifier`, then `attributes under the protected class scope` should be `_camelCase` and the `private attributes` should be `__camelCase`, methods should be `_pascalCase` and `private methods` should be `__PascalCase`.
Example :  
``` cpp linenums="1"
class GenericInterface 
{
private:
	size_t __id{};
	
	void __Init();
protected:

	int _common{};
	float _deltaCommon{};

	virtual void _CustomInit();
};
```

### <u>Public</u>

Within the `Public class scope`, `attributes` should be `PascalCase` and `methods` should be the same.
Example :  
``` cpp linenums="1"
struct genBundle 
{
	float FloatArray[3];
	int IntArray[3];
	size_t AddressArray[3];

	void Sort();
}
```