# Principles of Writing Idiomatic JavaScript 
## Basic
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
### String UpperCase/Lowercase

Syntax **toUpperCase()**;
**toLowerCase();**

Spec: Change first character of name to upper case rest to lower case

``` Javascript
var name= prompt("Enter your name:");
//full name to lower case
name=name.toLowerCase();

//first character to upper case
var firstChar=name.slice(0,1);
firstChar=firstChar.toUpperCase();

// Seperating rest of the name
var restName= name.slice(1,name.length);

//alert output
alert("Hello "+ firstChar+restName+"!");
```
Output: Hello Inian!

## Basic Arthmetic operations

### Modulo

4 % 6 = 2 (Remainder)

evenly divisible is even ( Remainder is 0)

not evenly divisible is odd (Remainder is not 0)

### Dog Age to Human age

**Order of Precedence**

Formula = ((dogAge-2) * 4)+21

```Javascript
var dogAge= prompt("Enter your dog Age:");
var humanAge=((dogAge-2)*4)+21;
alert("Your dog is "+ humanAge+ " Years old in Human Age!");
```
Output: Your dog is 33 Years old in Human Age!

### Increment and Decrement Operators

x= x+1 | x++

x= x-1 | x--

x= x+2 | x+=2

x= x+y | x+= y

y=x++ // Postfix increment, The value of x is assigned, then incremented

y=++x// Prefix increment, The value is incremented before, then assigned

``` Javascript
var x = 3;
var y = x++;
y += 1;
```
Output: X=4, y=4;

## Functions

### Constructing function

function getMilk(){
}


### Calling function

getMilk();

### Types of function
### Input type: Parameters and arguments

function getMilk(5);// 5 is number of bottles

### Round Values

Math.floor rounds the value to the nearest integer

var numbottles=Math.floor(money/1.5);


