# Ruby Flashcards

## Flashcard 1  
**Q:**  
- What is the purpose of the `pry-byebug` gem, and how is it used?  

**A:**  
- It allows you to debug by inserting breakpoints using `binding.pry`.  
```ruby
require "pry-byebug"  
binding.pry # Pauses the program for debugging
```

## Flashcard 2 
**Q:**  
- What is Object-Oriented Programming (OOP) in Ruby?

**A:**  
- A paradigm that organizes code into objects combining data (state) and methods (behavior).
- Example: String.new("Hello") creates an object with state "Hello" and methods like .upcase.
