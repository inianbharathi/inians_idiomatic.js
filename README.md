# Principles of Writing Idiomatic JavaScript 
## Comment
### Single line comment
```Javascript
//  This is a single line comment
```
### Multy line comment
``` Javascript
/* This is a multy line comment
This has more lines*/
```

## Alert 
### Alert Syntax
```window.alert("Hello World");```
### Alert Usage
``` alert("Hello World");```

## DataTypes
### Main types of datatypes 
Strings = "Hello"

Numbers=123

Boolean=true or False

### Find datatype

```typeof(23);```

## Variables
``` var yourName=prompt("Enter your name:");```

Prompt is used to get input from the user

### Variables naming conventions

Can't use

1. Keyword - var, function, alert (myvar-valid)
2. Start with number - 123 (my123-valid)
3. Spaces - my Name (myName - Valid)

Can use - my123$_ (my_name- Valid)

**Camel Casing** - myVar
## Strings
### String Concatenation
```javascript
    var message="Hello";
    var name=prompt("Enter your name: ");
    alert(message +" + name);
```
**Output:** Hello Inian

### String Length

```Javascript
var tweet=prompt("Enter Tweet: ");
var tweetLength=tweet.length;
alert("You have entered "+tweetLength+" Characters, " + "You have "+(140-tweetLength)+ " Characters remaining");
```
**Output:** You have entered 283 Characters, You have -143 Characters remaining

### String Slicing

1. String are always counted from 0.

2. Element in last value of slice parameter doesn't come in output

3. Second slice value - first slice value will give length of slice, which you will get as output

4. To slice last character alone (if length of string is 5, string.slice(5,6))

```Javascript 
alert(prompt("Enter your tweet:").slice(0,140));
```
