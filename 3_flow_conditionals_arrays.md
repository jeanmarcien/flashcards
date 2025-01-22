# Flashcards: Flow, Conditionals & Arrays

## Flashcard 1
**Q:**
- How do you structure a basic `if` statement in Ruby?
  
**A:**  
```ruby
if condition
  # code when condition is truthy
end
```  
**Truthy** means anything except `false` or `nil`.

---

## Flashcard 2  
**Q:**
- What is the Ruby ternary operator?
  
**A:**  
```ruby
condition ? code_when_truthy : code_when_falsey
```

---

## Flashcard 3  
**Q:**
- How do `if/elsif/else` statements work?
  
**A:**  
```ruby
if condition
  # executed if condition is truthy
elsif another_condition
  # executed if first condition is false and this is truthy
else
  # executed if all conditions are false
end
```  

---

## Flashcard 4
**Q:**
- How do `case/when` statements work in Ruby?
  
**A:**  
```ruby
case variable
when value1
  # code for value1
when value2
  # code for value2
else
  # code for other values
end
```

---

## Flashcard 5
**Q:**
- How do you loop with `while` and `until` in Ruby?
  
**A:**  
- `while condition`: Loops while the condition is truthy.  
- `until condition`: Loops until the condition becomes truthy.  

---

## Flashcard 6
**Q:**
- How do logical operators `&&` and `||` work?
  
**A:**  
- `&&` (AND): Both conditions must be true.  
- `||` (OR): At least one condition must be true.  

---

## Flashcard 7
**Q:**
- How do you iterate over an array using `each`?  

**A:**  
```ruby
array.each do |element|
  # code for each element
end
```

---

## Flashcard 8
**Q:**
- How do you modify and query arrays in Ruby?
  
**A:**  
- Append: `array << "element"`  
- Delete by value: `array.delete("value")`  
- Delete by index: `array.delete_at(index)`  
- Query size: `array.size` or `array.count`

---

## Flashcard 9
**Q:**
- What is an inline condition?
  
**A:**  
```ruby
do_something if condition  
do_something unless condition  
```

---

## Flashcard 10
**Q:**
- How do you access and modify elements in an array?
  
**A:**  
- Access: `array[index]`  
- Modify: `array[index] = new_value`  
