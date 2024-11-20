# Complex Type Layout

### <u>Classes</u>

`C++ Classes` should follow the following layout :
``` cpp linenums="1"
class GenericInterface 
{
private:
	int _common{};
	float _deltaCommon{};

	void _Init();
protected:
/*NOTHING IS IN THIS AND IS ONLY FOR THE EXAMPLE*/
public:
	//Constructor
	GenericInterface();
	//Destructor
	~GenericInterface();
	//Change the values within the Interface
	void Modify();
}
```

The `Private Access specifier` should be the 1st declared within a Class.   
While there is a lot of debate on whether the `private` or `public` specifier should come first, it is my belief that if users of my libraries or code are investigating the internals it is from an **inquisitive standpoint to see how things are working internally** rather than to check all the methods they can interact with the interface as documentation should suffice in said cases.  
In addition, for a Class where the internals should be assumed unread by the users, I prefer to facilitate the lives of the programmer/s who worked on the project.   
**Seeing the internal variables first allows readers to get into the headspace of who wrote it when it was written,** which is important for those modifying the project after a long absence and those wishing to learn from it.  
Due to all these reasons the `private` access specifier should be the 1st one within the `Class` layout.

`protected` should be just after because generally they function as the `Private` specifier within a base class.  

`Class attributes` should be at first within the `private class scope`, `private class methods` coming after. Same layout for anything within `protected`.   
Within the `public class scope`, `constructors`, `destructors`and `operator overloads`, should be written first, followed by methods unique to that class, then lastly getters and setters.  

### <u>Structs</u>

`C++ Structs` should follow the following layout :

``` cpp linenums="1"
struct genBundle 
{
	float FloatArray[3];
	int IntArray[3];
	size_t AddressArray[3];
}
```

Due to the fact that generally `Structs` will only possess `attributes` and no `methods` the layout is simple, a list of the `attributes.`
For specific cases where there are `methods`, they should be under the `attributes.`