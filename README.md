# stringAndArrayMethods

charAt -- returns a new string that contains a character at a specific index. Time complexity O(1)
  ie let sring - "i love pie" 
        sring.charAt(1) =     (space)
        sring.charAt(4) = v
        sring.charAt(2) = l
        
charCodeAt -- returns an integer between 0 and 65535 (code that handles unicode characters-- based on the ASCII) at that specific index. Time complexity O(1) 
 ie let string - "This is string"
        string.charCodeAt(0) = 84
        string.charCodeAt(1) = 104
        string.charCodeAt(2) = 105
        
concat -- method to join two or more string, does not change existing strings but returns a new string containing the text of a joined string. Time complexity of O(n)
  ie let str1 = 'hello'
     let str2 = 'world'
     let result = str1.concat(str2) = 'helloworld'
     let result = str2.concat(str1) = 'worldhello'
     
     let str3 = 'hello '
     let str4 = 'world'
     let result = str1.concat(str2) = 'hello world'
     let result = str2.concat(str1) = 'worldhello '
     
includes -- case sensitive method that determines whether it contains specified string/character by returning t or f. Time complexity of O(1)
  ie let cost = $50.90
  console.log(cost.includes($)) = true
  console.log(cost.includes(.)) = true
  console.log(cost.includes(%)) = false 
  
  let string3= "Just a string"
  console.log(string3.includes('Script', 5)) = false
  
indexOf -- method that returns the index of the element that exists in the array or the first occurance of where it is. Time complexity of O(n)
  ie let str1 = 'finding substring in string'
  let example2= str1.indexOf('str')
  console.log(example) = 11
  
match -- method that searches a string for a match and returns the match as an array object. Time complexity is O(n) **matches against regular expression, if not 'match()' will convert it to a regular expression **. 
  ie let str2 = 'Price: $5 - $15'
  let result = str2.match(/\$\d+/g)
  console.log(result) = [ '$5', '$15']
  
repeat -- method that returns a string containing a specified number of copies of string. Time complexity is O(1)
  ie let str3= 'hello world'
  console.log(str3.repeat(2)) = 'hello worldhello world'
  
replace -- method that searches a string for a specified value or regex and returns ndw string where that specified value is/are replaced. Time complexity is O(n)
  ie let str= 'hello world'
  let result = str.replace('world', 'mom') = 'hello mom'

search: case sensitive method that searches a string for a specified value and returns the position of the match. Time complexity is O(1).
  ie let re = /[A-Z]/
  let str = 'hi There! How are you?'
  let index = str.search(re)
  console.log(index) = 3 --> count by the index after the first cap letter, if doesnt exist it will return (-1)
  
slice -- method that returns a copy of a sub array between two index, start and end. Time complexity is O(n)
  ie const users = [ {name:'Luis', age:15}, {name:'Jose', age:18}, {name:'Aaron', age:40} ];
  const adults = users.slice(1, users.length) 
  console.log(adults) = (2) [{name: "Jose", age: 18}, {name: "Aaron", age: 40}]

split -- method that splits a string into an array of substrings. Time complexity is O(n)
  ie let str = 'i like pie'
  console.log(str.split('') = [ 'i', 'like', 'pie']
  
substr -- method that extract part of a string, it begins at the character at the specified position and returns specifed number of characters. Time complexity is O(n)

toLowerCase -- method that converts a string to lowercase letters. Time complexity is O(n)
  ie let str = 'HelLO WoRLd' 
  console.log(str.toLowerCase) = 'hello world'

toUpperCase -- method that converts a string to uppercase letters. Time complexity is O(n)
  ie let str = 'HelLO WoRLd' 
  console.log(str.toUpperCase) = 'HELLO WORLD'

trim - method that removes whitespace string. Time complexity is O(n)
ie let str = 'HelLO WoRLd' 
  console.log(str.trim) = 'HelLOWoRLd'
