#TODO Explain why we need loop. + Real examples


Let's imagine we need to write a program which has only one goal - count to 100.
How we can achieve it?





### For loop (classic)

```js
for (let i = 0; i < 10; i++) {
	console.log(i)
}
```

First part `let i = 0`  - we define variable where our counter will be stored.
Second `i < 10` we set a condition until when our loop will be running (must be boolean expression)
Third - we say what would happen with our variable after one tick. Here we just saying 'increment i by 1'

Let's imagine you want to count by different increment

```js
for (let i = 0; i < 10; i+=2) {
	console.log(i)
}
```


## Task

Make a loop which goes from 0 to 10, but shows only even numbers (Even number - which remainder after division by two is zero)

---


### For-of

How we can go through values inside array? We can access value of the array by index.

```js
const array = ['John', 'Smith', 'Thomas']
const name = array[0] // 'John'
```

Array has length property

```js
const array = ['John', 'Smith', 'Thomas']
const length = array.length // 3
```

So if we combine all information, from above can we write for loop which displays all the values from array?

> [!info]
> Try to access values outside of the array boundary


### Better way

```js
for (const name of array) {
	console.log(name)
}
```


### Task

Create an array with 5 random numbers. Go through this array and display only odd numbers using for..of loop.


---

## While loop

```js
while (true) {
	// do something
}
```


Let's create another counter.

```js
let i = 0;

while (i <= 10) {
	console.log(i)
	i++
}

```

Early exit

```js
let i = 0;

while (i <= 10) {
	console.log(i);
	
	if (i === 5) {
	  break;
	}
	
	i++;
}

console.log('After loop', i)
```


Mostly while loop can be met during algorithmic tasks.