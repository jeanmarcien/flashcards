# Flashcards: Parsing

## Flashcard 1  
**Q:**  
- What are the common data formats, and how are they used?  

**A:**  
- **Formats**: CSV, XML, JSON  
- **Usage**:  
  - CSV: Simple data exchange, often spreadsheets  
  - JSON: API communication  
  - XML: Document storage and structure  
- **Similarity**: All can represent structured data as plain text.  

---

## Flashcard 2  
**Q:**  
- What is a CSV file, and what are its key features?  

**A:**  
- **Definition**: Comma-Separated Values; text files with records on separate lines and fields separated by commas.  
- **Features**:  
  - Human-readable  
  - Optional header row  
  - Non-standardized delimiters/quotes  

---

## Flashcard 3  
**Q:**  
- How is JSON structured, and what are its key features?  

**A:**  
- **Definition**: JavaScript Object Notation; text-based, human-readable key-value pairs.  
- **Features**:  
  - Lightweight  
  - Derived from JavaScript, but independent  
  - Ruby Equivalent: Hash  

---

## Flashcard 4  
**Q:**  
- How does XML represent data, and what are its key features?  

**A:**  
- **Definition**: Extensible Markup Language; structured, nested data format.  
- **Features**:  
  - Tags and contents  
  - Human and machine-readable  
  - Ruby Equivalent: Nested Hash  

---

## Flashcard 5  
**Q:**  
- How do you parse a CSV file in Ruby?  

**A:**  
- **Library**: `require "csv"`  
- **Example (without headers)**:  
  ```ruby
  CSV.foreach("data.csv") do |row|
    puts row.inspect
  end
  ```  
- **Example (with headers)**:  
  ```ruby
  CSV.foreach("data.csv", headers: true) do |row|
    puts "#{row['Name']} works as a #{row['Job']}"
  end
  ```  

---

## Flashcard 6  
**Q:**  
- How do you write to a CSV file in Ruby?  

**A:**  
- **Example**:  
  ```ruby
  CSV.open("data.csv", "wb") do |csv|
    csv << ["Name", "Job"]
    csv << ["Alice", "Engineer"]
  end
  ```  

---

## Flashcard 7  
**Q:**  
- How do you parse and store JSON in Ruby?  

**A:**  
- **Parsing**:  
  ```ruby
  require "json"
  json_data = File.read("data.json")
  data = JSON.parse(json_data)
  ```  
- **Storing**:  
  ```ruby
  File.write("data.json", JSON.generate(data))
  ```  

---

## Flashcard 8  
**Q:**  
- How do you parse and store XML in Ruby?  

**A:**  
- **Parsing**:  
  ```ruby
  require "nokogiri"
  doc = Nokogiri::XML(File.open("data.xml"))
  doc.xpath("//tag").each do |node|
    puts node.text
  end
  ```  
- **Storing**:  
  ```ruby
  builder = Nokogiri::XML::Builder.new do |xml|
    xml.root { xml.example "data" }
  end
  File.write("data.xml", builder.to_xml)
  ```  

---

## Flashcard 9  
**Q:**  
- How can you use JSON APIs in Ruby?  

**A:**  
- **Example**:  
  ```ruby
  require "json"
  require "open-uri"
  url = "https://api.github.com/users/example"
  user = JSON.parse(URI.open(url).read)
  puts "#{user['name']} - #{user['bio']}"
  ```  

---

## Flashcard 10  
**Q:**  
- How do you scrape a website using Nokogiri in Ruby?  

**A:**  
- **Example**:  
  ```ruby
  require "nokogiri"
  require "open-uri"
  url = "https://example.com"
  doc = Nokogiri::HTML(URI.open(url))
  doc.css(".class").each { |node| puts node.text.strip }
  ```  
- **Tips**: Use a browser's "Inspect" feature to find CSS selectors.  
  
    <instrument>Guitar</instrument>  
  </beatle>  
  ```
---
