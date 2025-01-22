# Flashcards: Iterators & Blocks

## Flashcard 1  
**Q:**  
- How do you interact with arrays in Ruby?

**A:**  
- Create: `musicians = ['David Gilmour', 'Roger Waters', 'Richard Wright', 'Nick Mason']`
- Size: `musicians.size` → `4`
- Access: `musicians[1]` → "Roger Waters"
- Add: `musicians << 'Syd Barrett'`
---

## Flashcard 2  
**Q:**  
- What are ranges in Ruby and how do they differ?

**A:**  
- Inclusive: `0..10` includes 10.
- Exclusive: `0...10` excludes 10.
- Convert to array: `(0..10).to_a` → `[0, 1, ..., 10]`
---

## Flashcard 3  
**Q:**  
- How do you loop through arrays in Ruby?

**A:**  
- By index:
  ```ruby
  for index in 0...(musicians.size)
    puts "#{index + 1} - #{musicians[index]}"
  end
  ```
- By element:
  ```ruby
  for musician in musicians
    puts "Listen to #{musician}"
  end
  ```
---

## Flashcard 4  
**Q:**  
- How does the `each` iterator work in Ruby?

**A:**  
```ruby
musicians.each do |musician|
  puts "Hello #{musician}!"
end
```
---

## Flashcard 5  
**Q:**  
- How does `each_with_index` work in Ruby?

**A:**  
  ```ruby
  musicians.each_with_index do |musician, index|
    puts "#{index + 1} - #{musician}"
  end
  ```
---

## Flashcard 6  
**Q:**  
- What does the `map` method do in Ruby?

**A:**  
- Uppercase names:
  ```ruby
  musicians.map { |musician| musician.upcase }
  ```
- First names:
  ```ruby
  musicians.map { |musician| musician.split.first }
  ```
---

## Flashcard 7  
**Q:**  
- How do `select` and `count` work in Ruby?

**A:**
- Filter (`select`):
  ```ruby
  musicians.select { |musician| musician.start_with?('R') }
  ```
  →` ['Roger Waters', 'Richard Wright']`
- Count (count):
  ```ruby
  musicians.count { |musician| musician.start_with?('R') }
  ```
  →`2`
---

## Flashcard 8  
**Q:**  
- What are blocks in Ruby and how are they used?

**A:**
- Syntax:
  ```ruby
  do |num| num * 2 end  
  { |num| num * 2 }
  ```
- Multi-line returns last statement. Example:
  ```ruby
  musicians.map do |musician|
    musician.upcase
  end
  ```
---

## Flashcard 9  
**Q:**  
- How does `yield` work in Ruby? Example:

**A:**  
```ruby
def timer
  start = Time.now
  yield
  puts "Elapsed time: #{Time.now - start}s"
end
timer { sleep(2) }
```
---

## Flashcard 10  
**Q:**  
- How can you define custom iterators in Ruby?

**A:**  
- Recreate `.times`:
  ```ruby
  def repeat(number_of_times)
    (1..number_of_times).each { |i| yield(i) }
  end
  repeat(3) { |i| puts "Iteration #{i}" }
  ```
  →` Iteration 1, Iteration 2, Iteration 3`
