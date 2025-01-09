# Ruby Flashcards


markdown
Copy code
## Flashcard 1  
**Question:**  
- How do you launch the Ruby interactive shell and run a Ruby file?

**Answer:**  
- Launch IRB: `irb`  
- Run a file: `ruby path/to/your/file.rb`  

---

## Flashcard 2  
**Question:**  
- What are some common Ruby object classes?

**Answer:**  
- `"Hello".class` → `String`  
- `12.class` → `Integer`  
- `3.14.class` → `Float`  
- `[1, 2, 3].class` → `Array`  

---

## Flashcard 3  
**Question:**  
- How does string interpolation work in Ruby?

**Answer:**  
- Use double quotes: `"two: #{1 + 1}"` → `"two: 2"`

---

## Flashcard 4  
**Question:**  
- How do you define and call a method in Ruby?

**Answer:**  
```ruby
def method_name(parameters)  
  # code  
end  

method_name(arguments)

---

## Flashcard 5  
**Question:**  
- What’s the difference between a method ending in `?` and one ending in `!`?

**Answer:**  
- `?` → Returns true or false.  
- `!` → Destructive or dangerous operation.  

---

## Flashcard 6  
**Question:**  
- How do you convert between types in Ruby?

**Answer:**  
- To Integer: `'1984'.to_i` → `1984`  
- To String: `1984.to_s` → `"1984"`  

---

## Flashcard 7  
**Question:**  
- What is the purpose of variables in Ruby?

**Answer:**  
- To store values for reuse:  

```ruby
age = 17  
puts "You are #{age} years old"  

