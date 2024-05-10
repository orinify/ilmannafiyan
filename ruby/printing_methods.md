# What is the difference between puts, print, and p in Ruby, and when would you use each one?


Here's the difference between `puts`, `print`, and `p` in Ruby:

1. **puts**:
   - `puts` stands for "put string" and is a method in Ruby used to output a string to the console followed by a newline character (`\n`).
   - It automatically adds a newline character at the end of the output, which means each call to `puts` starts a new line.
   - It's commonly used for displaying messages or data in a user-friendly format.
   - Example:
     ```ruby
     puts "Hello"
     puts "World"
     # Output:
     # Hello
     # World
     ```

2. **print**:
   - `print` is a method in Ruby used to output a string to the console without adding a newline character.
   - It prints the string as it is, without adding any extra formatting.
   - It's useful when you want to output multiple strings on the same line.
   - Example:
     ```ruby
     print "Hello "
     print "World"
     # Output: Hello World
     ```

3. **p**:
   - `p` is a method in Ruby used to output the result of an expression to the console in a more "inspectable" format.
   - It's commonly used for debugging or inspecting the value of variables.
   - Unlike `puts` and `print`, `p` doesn't convert the value to a string; it uses `inspect` method to represent the object, making it useful for debugging complex data structures.
   - Example:
     ```ruby
     p "Hello"
     # Output: "Hello"
     ```

When to use each one:
- Use `puts` when you want to output a string followed by a newline character, typically for user-facing messages or data.
- Use `print` when you want to output a string without adding a newline character, useful for printing multiple strings on the same line.
- Use `p` when you want to output the result of an expression in a format that's easier to inspect, commonly used for debugging or understanding the value of variables.
