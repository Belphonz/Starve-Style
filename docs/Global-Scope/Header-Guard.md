#  Header Guard

The Header Guard is a directive used to ensure that header files are only copied once into any single file. While `#pragma once` can be used, `#ifndef` will be preferred for a multitude of reasons :  

First off, and while it is a small reason it must be stated, some compilers do not support `#pragma once`.   
In Addition, `#ifndef` allows for more on hands control of what is included for example including in a mock header who uses the same `#ifndef` as another more complex class.  
Personally I find it increases makes headers easier to navigate as the guard describes the file name generally.  
Finally, `#ifndef` is still the standard while `#prgama once` isn't.

As for naming convention, the defined variable should be in `SCREAMING_SNAKE_CASE`, in the format `LIBRARY/PROJECTNAME_FILENAME_H`.
Example :
``` cpp linenums="1"
#ifndef ARSON_TENSOR2DARRAY_H
#define ARSON_TENSOR2DARRAY_H

//file here

#endif
```