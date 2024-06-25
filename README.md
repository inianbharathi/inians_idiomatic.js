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
### Normal type
```Javascript
function example(){
console.log("This is a example");
}
example()
```
### Input type: Parameters and arguments

function getMilk(5);// 5 is number of bottles

**Round Values**

Math.floor rounds the value to the nearest integer

var numbottles=Math.floor(money/1.5);

### Life in weeks

``` Javascript
function lifeInWeeks(age) {
 
    var numMonths= (90*12)-(age*12);
    var numWeeks=(90*52)-(age*52);
    var numDays=(90*365)-(age*365);
    console.log("You have "+ numDays + " days, "+ numWeeks+" weeks, "+ "and "+numMonths+ " months left.");
}
lifeInWeeks(56);
```
### Return type: function that return vaues

```Javascript
  function getMilk(money,costPerBottle){
  return money % costPerBottle;
}
var change = getMilk(8,3);
console.log(change);
```

**Output:** change:2

### BMI Calculator

```Javascript
var weight="102";
var height="1.83";
function bmiCalculator(weight,height){
    var bmi = weight/ Math.pow(height, 2);
    return bmi;
    
}
```
### Conditional Statements

**Random Number Generator**

``` Javascript
Math.random();
```
// generates values between 0 to 0.99999..

**Random Dice** 

``` Javascript
var n = (Math.random()*6);
```

**Random Range between 1 - 6**

``` Javascript
n= (n*6)+1;
```
// range between 1 to 6

## Love Calculator
``` Javascript
prompt("Enter your name:");
prompt("Enter your Dollies name:");
var n = Math.random();
n= Math.floor((n*100)+1);
if (n>70){
    alert("Your love score "+n+"% , your love is true!");
}

else{
    alert("Your love score "+n+"% !");    
}
```
**D1 - till fibonacci solutions**

##  Comparators and Equality

=== : Check if equal to

!== : Check if not equal to

==: Check equal to, but not the data type


## Combining Comparators

&& : And

|| : Or

!: Not Equal

**Love Calculator using Comparators**
``` Javascript

prompt("Enter your name:");
prompt("Enter your Dollies name:");
var n = Math.random();
n= Math.floor((n*100)+1);
if (n>70){
    alert("Your love score "+n+"% , your love each other like kanye loves kanye!");
}
else if (n>=30 && n<=70)
{
    alert(" Your love score is "+n+"%, you guys are okie!")
}
else {
    alert("Your love score "+n+"% !"+ " you love each other like oil and water");    
}
```
## BMI Calculator Advance if/ else

``` Javascript
function bmiCalculator (weight, height) {
    var interpretation;
    var bmi = Math.round(weight/ Math.pow(height, 2));

if (bmi <18.5){
    interpretation = "Your BMI is "+ bmi+ ", so you are underweight."
    return interpretation
}
else if (bmi>=18.5 && bmi<=24.9){
    interpretation = "Your BMI is "+ bmi+ ", so you have a normal weight."
    return interpretation;
}
else{
    interpretation = "Your BMI is "+ bmi+ ", so you are overweight."
    return interpretation;
}
}
bmiCalculator(80,1.83);
```




