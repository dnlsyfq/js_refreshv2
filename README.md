### Rules
'' js
"" html

### Array

a = ['x','b','c']

a = Array()

a.push('first')

a[1] = 'second'

### Associative Array @ Objects

b = {
    'name':'chunk',
    'class':'json'
}

### for loops 

balls = {'golf':'Golf balls','tennis':'Tennis balls','ping':'Ping Pong balls'};

for(ball in balls){
    console.log(ball + ' = ' + balls[ball])
}

### Variables

* var 
var yourName = 'Dan'

### Switch

```
let groceryItem = 'papaya';

switch(groceryItem){
    case 'tomato':
        console.log('Tomatoes are $0.49');
        break;
    case 'lime':
        console.log('Limes are $1.49');
        break;
    default:
        console.log('Invalid item');
        break;
}
```

### JS Function

* prompt(string)
* alert(string)
* typeof varname

```
<script>
    function product(a,b){
        value = a + b;
        return value;
    }

    console.log("Prod = " + product(4,5));
</script>
```

### JS String Properties 
* Property : characteristics
* Method : function

* .length
```
    varString.length
```

* .startsWith('')
* .toUpperCase()
* .toLowerCase()
* .trim()
* .concat()
```
    varString.concat(varSting)
```
*  .slice(start,end)
* .includes("<character or string to find",<optional: specific index>) // true or false
* .search() // search the string starting index
```
    varString.search(varString)
```
* .indexOf() // search string starting
```
    varString.indexOf(<string>,<index>)
```
* .lastIndexOf() // search string from last
* .replace(<oldString>,<newString>)

* interpolation
```
var yourName;
document.write(`${yourName} <br>`);
```
  
### JS DOM

* documen.write
```
    <div class="results">
        <script>
            document.write ("Hello " + yourName + ", <br>");
        </script>
    </div>
```

* document.getElementById()

example 1
```
<p> Hello <b><span id="person">Chuck</span></b> there. </p>

<script>
    st = document.getElementById('person').innerHTML;
    console.log("ST = " + st);
    console.dir(document.getElementById('person'));
    alert('Hi there ' + st);
    document.getElementById('person').innerHTML = 'Joseph';
</script>
```

example 2
```
<a href="#" onclick="document.getElementById('stuff').innerHTML ='BACK'; return false;">
    Back
</a>

<a href="#" onclick="document.getElementById('stuff').innerHTML = 'FORTH'; return false;">
    Forth
</a>

<p>Hello <b><span id="stuff">Stuff</span></b> there.</p>
```

example 3
```
<p>
    <a href="#" onclick="add(); return false;">More</a>
</p>

<ul id="the-list">
    <li>First Item</li>
</ul>

<script>
    let counter = 1;
    function add(){
        var x = document.createElement('li');
        x.innerHTML = 'The counter is " + counter;
        document.getElementById('the-list').appendChild(x);
        counter ++;
}
</script>

```

### HTML + JS 

* onclick
```
<p><a href="https:www.google.com" onclick="alert('Hi'); return false;">Click Me</a></p>
```

### Debugger with / without console

window.console && console.log()

console.dir()

### Math & Number method

* Prints a random number between 0 and 1
Math.random() 

```
Math.random() * 50;
```

* Math.floor() takes a decimal number, and rounds down to the nearest whole number. 

```
Math.floor(Math.random() * 50);
```

* Math.ceil()
returns the smallest integer greater than or equal to a decimal number.

* Number.isInteger()
isInteger() method from the Number object to check if 2017 is an integer.



* string to number

```
var salary;
salary = 129000;
raise = prompt("Like raise ?");
salary += Number(raise);
```

* number to string


```
            var cust1;
            var cust2;
            var cust3;

            cust1 = 12345;
            cust2 = 98765;
            cust3 = 11550;

            document.write(cust1.toString() + cust2.toString() + cust3.toString());
```

```
            var acctBal;
            acctBal = 85699.64;
            document.write(Number(acctBal).toLocaleString());
```

* isNan() method

isNan(variable);

* Number.MAX_VALUE;

### Array 
 elements in an array declared with const remain mutable. Meaning that we can change the contents of a const array, but cannot reassign a new array or a different value.
 
```
const arr = []

let arr = []
```

* .length
array.length

* .push
to add items to the end of an array.
take a single argument or multiple arguments separated by commas
```
array.push(value1,value2)
```

* .pop
removes the last item of an array.
returns the value of the last element
```
array.pop()
```

* .shift()
 to remove the first item from the array
```
array.shift()

```

* .unshift()
method to add element to the beginning of array
```
array.unshift(element)
```

* .slice()
```
array.slice(start,stop);
```

* .indexOf()
```
array.indexOf('element')
```

