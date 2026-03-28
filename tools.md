# TOOLS
How computers work; Using common tools and writing custom ones in multiple languages

## Table of Contents
| Module | Sub-module |
| :---- | :---- |
| [Prep]() |  |
| [Sprint 1]() | Prep |
|  | Backlog |
|  | Day Plan |
|  | End of Sprint Review |
| [Sprint 2]() | Prep |
|  | Backlog |
|  | Day Plan |
|  | End of Sprint Review |
  [Sprint 3]() | Prep |
|  | Backlog |
|  | Day Plan |
|  | End of Sprint Review |
  [Sprint 4]() | Prep |
|  | Backlog |
|  | Day Plan |
|  | End of Sprint Review |
  [Sprint 5]() | Prep |
|  | Backlog |
|  | Day Plan |
|  | End of Sprint Review |



## Prep
- [x] Install a UNIX-based operating system (Mac and Linux already have a UNIX-based operating system)
- [x] Check Git- to double check if you have git installed, run this command ```git --version```
- [x] Install VS Code-if you are on github press on "." while on any github repo to open github.dev
- [x] Make a folder called Migracode and store all your work for the course
- [x] Create a planner repo (reuse the previous planner)
      

## Sprint 1
  ### Prep
  Learning objectives
  - [x] Convert signed and unsigned numbers between any two of: binary, decimal, hexadecimal
  - [x] Identify whether a binary number is a power of two
  - [x] Explain the similarities and differences between binary, decimal, and hexadecimal numbers
  - [x] Explain why we use binary numbers
  - [x] Explain why we use hexadecimal numbers
  - [x] Describe how different programs can interpret the same bytes as different data
  - [x] Identify how many bits are needed to store integers up to some limit
  - [x] Identify the maximum integer that can be stored in a number of bits
  - [x] Add together two binary numbers without converting to decimal
  - [x] Identify which of two binary numbers is larger without converting to decimal



  
  ### Backlog
  ### Day Plan
  `git log` - shows all the logs, author, and date when the log happens\
  `grep '^Author:'` - Filters the output, keeping only lines that start with Author:. You end up with lines\
  `git log | grep '^Author:' | sed 's/^Author: //' | sed 's/ <.*$//' | sort | uniq | wc -l` - this counts all the Author

  `nano myscript-june.sh`-saving script templates
  
  
  ### End of Sprint Review


## Sprint 2
  ### Prep
  Learning objectives
  - [x] Define the term variable
        A variable is a named storage location in memory
        Variables allow programmers to give a name to a memory address
           
  - [ ] Describe how a variable relates to a memory location
        
  - [ ] Give 3 examples of common operators
  - [ ] Define && (and), || (or), and !(not) operators
  - [ ] Explain what happens when you call a function
  
  ### Backlog
  ### Day Plan
  Review about Variables, Classes, and Objects\
  jq '.' file.json - pretty prints the JSON\
  jq '.key' file.json - extracts value of "key"\
  jq '.key.subkey' file.json - extracts nested value\
  jq '.[0]' file.json - gets first element of array\
  jq '.[1:3]' file.json - slices array elements 1 to 2\
  jq '.[]' file.json - iterates over all array elements\
  
  jq '.users[].name' file.json - prints all names from users array\
  jq '.[] | select(.age > 18)' file.json - filters objects where age > 18\
  jq '.users[] | select(.name=="John")' file.json - filters by name\
  
  jq '.[] | .name' file.json - extracts name field from each element\
  jq '.[] | {name: .name, age: .age}' file.json - creates new objects with selected fields\
  jq '{name: .name, age: .age}' file.json - constructs a new object\
  
  jq 'map(.age)' file.json - extracts age field from all elements into array\
  jq 'map(select(.age > 18))' file.json - filters array elements by condition\
  
  jq 'length' file.json - returns length of array or object\
  jq 'add' file.json - sums array values\
  jq 'max' file.json - returns max value in array\
  jq 'min' file.json - returns min value in array\
  jq 'group_by(.age)' file.json - groups array elements by age\
  
  jq '.price * 2' file.json - multiplies numeric field\
  jq '.count + 10' file.json - adds to numeric field\
  
  jq '.name | ascii_upcase' file.json - converts string to uppercase\
  jq '.name | ascii_downcase' file.json - converts string to lowercase\
  jq '.name | length' file.json - gets string length
  
  jq 'keys' file.json - returns object keys\
  jq 'values' file.json - returns object values\
  jq 'to_entries' file.json - converts object to key-value pairs\
  jq 'from_entries' file.json - converts key-value pairs back to object\
  
  jq 'if .age > 18 then "adult" else "minor" end' file.json - conditional logic\
  
  jq '.users[] | .name' file.json - pipes output to extract names
  jq '. as $data | $[data.name](http://data.name/)' file.json - stores input in variable\
  
  jq -R '.' file.txt - reads raw input as strings\
  jq -s '.' file.json - slurps multiple inputs into array\
  
  jq 'type' file.json - returns JSON type\
  jq 'sort' file.json - sorts array\
  jq 'sort_by(.age)' file.json - sorts array by age field\
  jq 'unique' file.json - removes duplicate elements\
  jq 'reverse' file.json - reverses array\
  
  jq '.. | .name?' file.json - recursively finds all "name" fields\
  jq 'flatten' file.json - flattens nested arrays\
  jq 'walk(if type=="string" then ascii_upcase else . end)' file.json - transforms all strings\
  
  jq -c '.' file.json - outputs compact JSON\
  jq -r '.name' file.json - outputs raw string without quotes\
  
  jq '.users | length' file.json - counts users
  jq '.users[] | {name, age}' file.json - extracts selected fields shorthand\
  jq '.users[] | select(.age > 18) | .name' file.json - filters and extracts names\

  ### End of Sprint Review


## Sprint 3
  ### Prep
  ### Backlog
  ### Day Plan
  ### End of Sprint Review

## Sprint 4
  ### Prep
  ### Backlog
  ### Day Plan
  ### End of Sprint Review
  
## Sprint 5
  ### Prep
  ### Backlog
  ### Day Plan
  ### End of Sprint Review
