# Ruby Flashcards

## Flashcard 1  
**Q:**  
- How do you launch the Ruby interactive shell and run a Ruby file?

**A:**  
- Launch IRB: `irb`  
- Run a file: `ruby path/to/your/file.rb`  

---

## Flashcard 2  
**Q:**  
- What are some common Ruby object classes?

**A:**  
- `"Hello".class` → `String`  
- `12.class` → `Integer`  
- `3.14.class` → `Float`  
- `[1, 2, 3].class` → `Array`  

---

## Flashcard 3  
**Q:**  
- How does string interpolation work in Ruby?

**A:**  
- Use double quotes: `"two: #{1 + 1}"` → `"two: 2"`

---

## Flashcard 4  
**Q:**  
- How do you define and call a method in Ruby?

**A:**  
```ruby
def method_name(parameters)  
  # code  
end  

method_name(arguments)
```
---

## Flashcard 5  
**Q:**  
- What’s the difference between a method ending in `?` and one ending in `!`?

**A:**  
- `?` → Returns true or false.  
- `!` → Destructive or dangerous operation.  

---

## Flashcard 6  
**Q:**  
- How do you convert between types in Ruby?

**A:**  
- To Integer: `'1984'.to_i` → `1984`  
- To String: `1984.to_s` → `"1984"`  

---

## Flashcard 7  
**Q:**  
- What is the purpose of variables in Ruby?

**A:**  
- To store values for reuse:  

```ruby
age = 17  
puts "You are #{age} years old"  
```
---

## Flashcard 8  
**Q:**  
- How do you create and manipulate arrays?

**A:**  
- Create: `%w[Huey Dewey Louie]` → `["Huey", "Dewey", "Louie"]`  
- Sort: `[3, 1, 2].sort` → `[1, 2, 3]`  
- Size: `['a', 'b'].size` → `2`  

---

## Flashcard 9  
**Q:**  
- How do ranges work in Ruby?

**A:**  
- Inclusive: `(1..5).to_a` → `[1, 2, 3, 4, 5]`  
- Exclusive: `(1...5).to_a` → `[1, 2, 3, 4]`  

---

## Flashcard 10  
**Q:**  
- What’s the return convention in Ruby methods?

**A:**  
- A method returns the last statement executed:  

```ruby
def add(x, y)  
  x + y  
end  
```
