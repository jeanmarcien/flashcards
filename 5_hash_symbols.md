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
  Easier to access: ***students_age["Peter"]*** → 24
---

## Flashcard 3  
**Q:**  
- How do you read values from a hash in Ruby?

**A:**  
```ruby
paris = { "country" => "France", "population" => 2211000 }
paris["country"]  # → "France"
paris["population"]  # → 2211000
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
- When should you use symbols instead of strings in Ruby?

**A:**  
- Use strings for data: ***"Sebastien Saunier"***, ***"ruby on Rails".***
- Use symbols for identifiers: ***:fullname***, ***:email***.
- Symbols are more memory-efficient for keys in hashes:
  ```ruby
    paris = { country: "France", population: 2211000 }
    paris[:population]  # => 2211000
  ```
---

## Flashcard 8  
**Q:**  
- How do hashes differ from arrays in Ruby?

**A:**  
- Arrays are indexed by integers: ***cities[0] → "London"***.
- Hashes are indexed by keys: ***city["name"] → "Paris"***.
- Example for readability:
  ```ruby
    cities = { "Paris" => { "country" => "France", "monument" => "Tour Eiffel" } }
    cities["Paris"]["monument"]  # → "Tour Eiffel"
  ```
---

## Flashcard 9  
**Q:**  
- What is special about using a hash as the last method argument in Ruby?

**A:**  
- Omit curly braces:
  ```ruby
    tag("a", "Le Wagon", href: "http://lewagon.org", class: "btn")
  ```
- Equivalent to:
  ```ruby
    tag("a", "Le Wagon", { href: "http://lewagon.org", class: "btn" })
  ```
---

## Flashcard 10  
**Q:**  
- How can you use hashes for dynamic HTML generation in Ruby?

**A:**
- Example method:
  ```ruby
  def tag(name, content, attrs = {})
    flat_attrs = attrs.map { |key, val| " #{key}=\"#{val}\"" }.join
    "<#{name}#{flat_attrs}>#{content}</#{name}>"
  end
  ```
- Call:
  ```ruby
  tag("h1", "Hello", class: "bold")
  ```
