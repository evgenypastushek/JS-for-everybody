# How we can drive our program in different directions?

## If - else - else if

```js
const hasCar = true;

if (hasCar) {
	// drive like a crazy
} else {
	// take public transport
}

// if - else if
if (hasCar) {
	// drive like a crazy
} else if (hasPrivateJet) {
	// dont worry at all
} else {
	// take public transport
}


```

Important note what's considered as truthy-falsy values

### Truthy

```js
' ' // true
'anything' // true
1+ // true
[] // true
{} // true
```


### Falsy

```js
'' // false
0 // false
undefined // false
null // false
```

You can negate expression by adding `!` in front of the values or even double negate it. Let's see why we call Truthy values as true


```js
console.log(!!' ')
console.log(!!1)
console.log(!![])
console.log(!!{})
```


### Operators ( === , !== , ? , % )


You can assign values to the variable by checking the condition

```js
const person = { age: 33, name: 'Jesus' }

const isLegalAge = person.age > 18

const whereWillEndUp = person.name === 'Jesus' ? 'Heaven' : 'Hell'
```

=== -  equal to
!== -  not equal to
? - ternary operator
% - remainder operator

Now we can combine if - else statement with functions

```js
const person = { age: 33, name: 'Jesus' }

if (person.name === 'Jesus') {
	goToHeaven()
} else {
	payForYourSins()
}

// OR

if (person.name !== 'Jesus') {
	payForYourSins()
} else {
	goToHeaven()
}

```


### Remainder

```js

const remainder = 5 % 2 // 1

```

### Task

Write a function which takes two arguments and check if the remainder of the division of the first argument by 2 is zero, than sum those arguments otherwise subtract first argument from the second one.

As outcome you will have three functions: main function which will use either sum or subtract, sum function and subtract function.

---


### Switch statement

Sometimes we face such issues where we need to check one variable against different cases and do different actions.

E.g

```js
if (person.profession === 'pilot') {
	// fly
} else if (person.profession === 'manager') {
	// manage
} else if (person.profession === 'dev') {
	// code code code
} else {
	// do something with your life
}
```

This can become quite cumbersome and hard to read. To help us to solve such a problem we have `switch` statement

```js
switch(person.profession) {
	case 'pilot':
		// fly
		break; // or return
	case 'manager':
		// manage
		break; // or return
	case 'dev':
		// code code code
		break; // or return
	default:
		// do something with your life
	break; // or return
}

```


### Task (Switch statement)

Create a function which takes name of the fruit and write a message to console about price of the fruit. For now assume we have only 3 (apple, orange, banana) fruits as a default result, print to console message "Unknown price"

Hint: to print message use `console.log('Your message here')`

```js
function getFruitPrice(fruitPrice) {
	// do the magic here
}
```


---