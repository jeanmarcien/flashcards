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
```
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
```
---

## Flashcard 8  
**Question:**  
- How do you create and manipulate arrays?

**Answer:**  
- Create: `%w[Huey Dewey Louie]` → `["Huey", "Dewey", "Louie"]`  
- Sort: `[3, 1, 2].sort` → `[1, 2, 3]`  
- Size: `['a', 'b'].size` → `2`  

---

## Flashcard 9  
**Question:**  
- How do ranges work in Ruby?

**Answer:**  
- Inclusive: `(1..5).to_a` → `[1, 2, 3, 4, 5]`  
- Exclusive: `(1...5).to_a` → `[1, 2, 3, 4]`  

---

## Flashcard 10  
**Question:**  
- What’s the return convention in Ruby methods?

**Answer:**  
- A method returns the last statement executed:  

```ruby
def add(x, y)  
  x + y  
end  
```
