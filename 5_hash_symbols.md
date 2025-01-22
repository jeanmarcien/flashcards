# Ruby Flashcards

## Flashcard 1  
**Q:**  
- What are the primary data types in Ruby?

**A:**  
- ***42*** → Integer
- ***1.25*** → Float
- ***true*** → Boolean
- ***"hello world"*** → String
- ***[ "a", "e", "i", "o", "u" ]*** → Array
---

## Flashcard 2  
**Q:**  
- How does a Hash improve maintainability compared to arrays for key-value data?

**A:**
- Array example:
  ```ruby
    students = ["Peter", "Mary"]
    student_ages = [24, 25]
  ```
  Hard to maintain large datasets.
- Hash example:
  ```ruby
    students_age = { "Peter" => 24, "Mary" => 25 }
  ```
  Easier to access: ***students_age["Peter"] => 24
---

## Flashcard 3  
**Q:**  
- How do you read values from a hash in Ruby?

**A:**  
```ruby
paris = { "country" => "France", "population" => 2211000 }
paris["country"]  # => "France"
paris["population"]  # => 2211000
```
---

## Flashcard 4  
**Q:**  
- How do you add, update, and delete key-value pairs in a hash?

**A:**  
- Add: ***paris["star_monument"] = "Tour Eiffel"***
- Update: ***paris["population"] = 2211001***
- Delete: ***paris.delete("star_monument")***
---

## Flashcard 5  
**Q:**  
- How do you iterate through a hash in Ruby?

**A:**  
  ```ruby
  paris.each do |key, value|
    puts "Paris #{key} is #{value}"
  end
  ```
  Outputs:
  ***Paris country is France***
  ***Paris population is 2211000***
---

## Flashcard 6  
**Q:**  
- What are some useful methods for hashes in Ruby?

**A:**  
- Check key: ***paris.key?("country")*** → ***true***
- List keys: ***paris.keys*** → ***["country", "population"]***
- List values: ***paris.values*** → ***["France", 2211000]***

---

## Flashcard 7  
**Q:**  
- How do you iterate over an array using ***each***?

**A:**  
```ruby
array.each do |element|
  # code for each element
end
```

---

## Flashcard 8  
**Q:**  
- How do you iterate over an array using each?

**A:**  
- Append: ***array << "element"***
- Delete by value: ***array.delete("value")***
- Delete by index: ***array.delete_at(index)***
- Query size: ***array.size*** or ***array.count***

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
- Access: ***array[index]***
- Modify: ***array[index] = new_value***
