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

## Flashcard 3
**Q:**
- How is a class different from an instance in Ruby?
  
**A:**
- A class is a blueprint (e.g., Car), while an instance is an object created from the class (e.g., Car.new).

## Flashcard 4
**Q:**
- How do you create a class in Ruby, and what is the naming convention?

**A:**
- Files: Use lower_snake_case (e.g., car.rb).
- Classes: Use UpperCamelCase (e.g., class Car).
```ruby
class Car  
end
```

## Flashcard 5
**Q:**
- What is the initialize method in Ruby, and when is it called?

**A:**
- It is called automatically when creating a new instance using ClassName.new.
```ruby
class Car  
  def initialize(color)  
    @color = color  
  end  
end
```

## Flashcard 6
**Q:**
- How do you define and access instance variables in Ruby?

**A:**
- Use @ to define instance variables, and methods to access them:
```ruby
class Car  
  def initialize(color)  
    @color = color  
  end  

  def color  
    @color  
  end  
end
```

## Flashcard 7
**Q:**
- What are attr_reader, attr_writer, and attr_accessor in Ruby?

**A:**
attr_reader: Creates a getter.
attr_writer: Creates a setter.
attr_accessor: Creates both getter and setter.
```ruby
class Car  
  attr_accessor :color  
end
```

## Flashcard 8
**Q:**
- What is the difference between public and private methods in Ruby?

**A:**
- Public: Accessible from outside the class.
- Private: Only accessible within the class.
```ruby
class Car  
  def start_engine  
    ignite_spark  
  end  

  private  

  def ignite_spark  
    puts "Spark ignited!"  
  end  
end
```

## Flashcard 9
**Q:**
- How do you instantiate objects from a class in Ruby?

**A:**
- Use the .new method:
```ruby
my_car = Car.new("red")  
puts my_car.color #=> "red"
```
 
## Flashcard 10
**Q:**
- What is OOP in Ruby summarized in key points?

**A:**
- Everything in Ruby is an object.
- Objects are instances of classes.
- Instance variables store state.
- Instance methods define behavior.
