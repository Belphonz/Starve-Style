## <u>Loop Index</u>
#### <u>General Cases :</u>
Within a `for loop`, the variable used as an index should follow the following naming convention within general cases : 

``` cpp linenums="1"
for (size_t i{0}; i < size; ++i)
{
	for (size_t j{0};j < size; ++j)
	{
		for (size_t k{0}; k < size; ++k)
		{
			++arr[i][j][k];
		}
	}
}
```

`i,j,k` is used as it is generally the most universally understood variable names for index's for `for loops` across software engineering.   
Using `index, deltaIndex,..` was entertained however has been dropped due to the overall lack of clarity it possessed compared to the unofficial standard. 

#### <u>Other Cases :</u>

Within cases where a more apt name can be chosen for the index, they should be preferred over `i,j,k`.   
An Example being `x,y,z` when the loop is iterating over something that can be called spatial dimensions.  

It is to be stated that generally there will be moments where words can be a more apt variable name for an index within a loop as they're more immediately understood, such as `position`.   
Within such cases attempts should be done to shorten them into globally understood shorthands, such as for the above example `pos`.  
If a nice shorthand cannot be chosen for the situation at hand and `i,j,k` will lead to more confusion than clarity, than the index variable name can be chosen as a whole word.

It must be said that while this section mentions

## <u>Variables Instantiated within the </u>