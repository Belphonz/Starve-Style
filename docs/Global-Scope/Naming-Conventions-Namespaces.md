# Naming Conventions : Namespaces

If creating a `C++ library`, a `NameSpace` should encapsulate each element.  
As for how to go about naming them, for the outer `NameSpace` they should be name of the library crushed into a 3-5 characters sequence.
Example :
``` cpp linenums="1"
//Library Arson
namespace Arn
{
	
}
```

If a library is big enough to warrant having several `NameSpaces` than they should be the subject then a 3-5 characters sequence.
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