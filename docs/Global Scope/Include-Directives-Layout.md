# Include Directives Layout

`Include directives` should be organised first by standard library headers, then by external library headers, then by headers found within the project then finally by the class definition headers if it applies.
Example :

``` cpp linenums="1"
#STD Library
#include <iostream>
#incldude <cmaths>
#EXTERNAL LIBRARY + PROJECT HEADERS
#include "Arson/Tensor2DArray.h"
#include "GeneralInterface.h"
#CLASS DEFINITION
#include "shapeBundle.h"
```

