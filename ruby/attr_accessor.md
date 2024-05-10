# What does the attr_accessor method do in Ruby, and how does it differ from attr_reader and attr_writer?

The `attr_accessor`, `attr_reader`, and `attr_writer` methods in Ruby are used to define attribute accessors for a class. Here's what each method does and how they differ:

1. **attr_accessor**:
   - `attr_accessor` is a Ruby method that automatically creates both råeader and writer methods for instance variables of a class.
   - It allows both reading and writing to the instance variable.
   - It is a shortcut for defining both `attr_reader` and `attr_writer` for the same variable.
   - Example:
     ```ruby
     class MyClass
       attr_accessor :name
     end

     obj = MyClass.new
     obj.name = "John"
     puts obj.name #=> "John"
     ```

2. **attr_reader**:
   - `attr_reader` creates a reader method for an instance variable, allowing you to access the variable's value from outside the class, but not modify it.
   - It provides only read access to the instance variable.
   - Example:
     ```ruby
     class MyClass
       attr_reader :name
       def initialize(name)
         @name = name
       end
     end

     obj = MyClass.new("Alice")
     puts obj.name #=> "Alice"
     ```

3. **attr_writer**:
   - `attr_writer` creates a writer method for an instance variable, allowing you to modify the variable's value from outside the class, but not read it directly.
   - It provides only write access to the instance variable.
   - Example:
     ```ruby
     class MyClass
       attr_writer :name
     end

     obj = MyClass.new
     obj.name = "Bob"
     ```

In summary:
- `attr_accessor` provides both read and write access to an instance variable.
- `attr_reader` provides read-only access to an instance variable.
- `attr_writer` provides write-only access to an instance variable.

Understanding these methods is crucial for managing the state of objects in Ruby classes efficiently.
