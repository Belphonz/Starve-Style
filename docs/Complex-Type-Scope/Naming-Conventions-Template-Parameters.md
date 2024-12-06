# Naming Conventions : Template Parameters

Within C++, `Templates` should generally only be restricted to `Classes` and their respective `methods`.   
`Template Parameters` should be written in `SCREAMING_SNAKE_CASE`.  
The main reason for this is that I believe that they should be easy to differentiate from variables initialized within function scope.   

`typename` should be preferred over `class` for `template parameters`, for the simple reason that I find them easier to understand.
If the `template parameter`