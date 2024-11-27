The Header Guard is a directive used to ensure that header files are only copied once into any single file. While `#pragma once` can be used, `#ifndef` will be preferred for a multitude of reasons :

First off, and while it is a small reason it must be stated, some compilers do not support `#pragma once`. 