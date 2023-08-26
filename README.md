# WordPress Hook: Filter &Action
## Filter Hook
### How to work
When applying a filter, at first it finds a function registered with this hook. If it is, the argument is passed as parameter to that function, and after some operation, this function returns the parameter which is updated at apply_filter() function. If not default parameter remains same.
### Features
* always return something
* accept parameters
* priority
```php
/**
* apply filter
* argument is passed as parameter
* to the registered function associated with hook
*/

apply_filter('your_filter_name', 'argument');
// or
$filtered_value = apply_filter('your_filter_name', 'argument');

/**
* create filter
* $parameter comes from apply_filter()
*/

function function_to_be_excuted($parameter){
  // do something with $parameter
  return $parameter;
}
add_filters('your_filter_name', 'function_to_be_excuted');
```
