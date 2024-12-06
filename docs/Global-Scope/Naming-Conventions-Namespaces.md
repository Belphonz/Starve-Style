# Naming Conventions : Namespaces

If creating a C++ library, a `namespace` should encapsulate each element.  
As for how to go about naming them, for the outer `namespace` they should be the name of the library shortened into a 3-5 characters sequence.
Example :
``` cpp linenums="1"
//Library Arson
namespace Arn
{
	
}
```

If a library is big enough to warrant having several `namespaces` than the `namespace` should be the subject also shortened into a 3-5 characters sequence.
Example :
``` cpp linenums="1"
//Coalescence Engine
namespace COSCE
{
	namespace GFX
	{
	}
}
```