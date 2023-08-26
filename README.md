# WordPress Hook: Filter &Action
## Filter Hook
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

function($parameter){
  // do something with $parameter
  return $parameter;
}
add_filters('your_filter_name', 'function_to_be_excuted');
```
