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
