# What is the difference between a symbol and a string in Ruby, and when would you use each one?

In Ruby, both symbols and strings are used to represent data, but they have some key differences:

1. **Strings**: 
   - Strings are mutable, meaning they can be changed after they are created.
   - Strings are sequences of characters enclosed within single quotes ('') or double quotes ("").
   - They are often used to represent textual data like names, messages, or any arbitrary sequence of characters.
   - Example: `"Hello, World!"`

2. **Symbols**:
   - Symbols are immutable, meaning they cannot be changed once they are created. They are unique and immutable string literals.
   - Symbols are preceded by a colon (:).
   - They are often used as identifiers or labels within a Ruby program, such as keys in hash tables or method names.
   - Symbols are more memory efficient than strings because they are stored as a single, internalized value, whereas each occurrence of a string literal creates a new object.
   - Example: `:hello_world`

When to use each one:
- Use strings when you need mutable text data or when you need to interpolate variables within the text.
- Use symbols when you need a constant and immutable identifier, such as keys in hashes, method names, or enum values. Symbols are also commonly used in metaprogramming and to represent identifiers in Ruby code.
