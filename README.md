# Ruby Koans

This is my attempt to solve the [Ruby Koans](https://www.rubykoans.com/)

Ruby version: 3.0.0

## What I've Learned

- Basic TDD  
\- Red, Green, Refactor  
\- `asert`, `asert_equal` methods *(File: `about_asserts.rb` line 19-34)*  

- Boolean:  
\- `false` and `nil` is treated as `false`  
\- Everything esle is treated as `true`. Example: `0`, `""`, `[]`, `{}`  

- String:  
\- Create string using single quotes, double quotes, flexible quotes, HERE docs.  
\- Using backslash (`\`) for special characters  *(escape character)*  
\- Difference bettween flexible quotes and HERE docs *(File: `about_strings.rb` line 38-56)*  
\- Prefer the shovel operator (`>>`) to the plus equal operator (`+=`) when concatenate strings *(File `about_strings.rb` line 71-105)*  
\- String interpolation: `"After 2 is #{2+1}"`  
\- Double quotes strings support string interpolation and all escape characters *(ie: `\n`)*, single quotes strings don't  
\- How to `split` and `join` strings  
\- Strings are unique objects *(2 variables with the same string value have different object id)*   

- Symbol:  
\- Symbols can be compared  
\- Identical symbols are the same object  
\- String to Symbol: `"cat".to_sym`  
\- Symbol to String: `:cat.to_s`  
\- Symbol can have space between: `:"cats and dogs"`  
\- Symbol interpolation is supported: `:"cats #{value} dogs`  
\- Symbol doesn't have String methods  
\- It's not a good idea to dynamically create a lot of symbols  

- Array:  
\- Interesting read about [splat operator](https://thoughtbot.com/blog/ruby-splat-operator)  

- Object:  
\- Everything is object  
\- Every object have an unique object ID  

- Hash:  
\- `hash[:doesnt_exist_key]` return `nil`  
`hash.fetch(:doesnt_exist_key)` throw `KeyError` exception  
\- Hash is unordered  
\- Hash default value is the same object `h = Hash.new([])`. To prevent this, use:  
\- Hash default value with block: `h = Hash.new {|hash, key| hash[key] = []}`  

- Method:  
\- Method with default value for arguments: `method_with_defaults(a, b=:default_value)`  
\- Method with variable arguments: `method_with_var_args(*args)`  
\- Can't call private methods with an explicit receiver: `self.private_method` will raise `NoMethodError` exception  



