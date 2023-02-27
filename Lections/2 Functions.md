### What is function

> [!defintion]
> Function - in mathematics, an expression, rule, or law that defines a relationship between one variable (the independent variable) and another variable (the dependent variable)

This is very academic definition. But let's think about some examples from real world. What function has juice maker.
Make a juice!
There you have it!
Function:
- must do one thing
- In ideal world do not modify input (show example)

Let's see how we can define function is JS

```js
function makeJuice(ingridients) {
	// make me a juice
}
```

Here we have an argument - ingredients - in our case. Body function - everything between curly braces. You can have any number of arguments.

Calling functions in sequence we can write small programs.

Let's create sum function, which sums two number values together

```js
function sum(a, b) {
	// wait how we get result out of the function
}
```


`return` - keyword that signals our program to exit function with some values

### Arrow function

There is another way to define function so called arrow function. Differences are again lies in the scope.

```js

const makeJuice = (ingridients) => // make me a juice
```

> [! mental note]
> Function body in arrow functions and return values

Let's rewrite our sum function to arrow function.


### Callbacks and function composition

Function can take another function as argument and invoke from inside.

Let's imagine we have robot bartender which mix or stir cocktails

```js

function stir(ingredients) {
	// stir a drink
}

function shake(ingredients) {
	// mix a drink
}
```

But also robot has a function to make a drink

```js
function makeADrink(cocktailName, action) {
	// fetch ingridients
	// do the action = action()
	// pour into glass
}
```

In the end we will have full example like that

```js
const myDrink = makeADrink('James Bond Martini', shake)
```


#TODO *make it more appealing*

Another example of callbacks is subscription model.

I'm subscribing to the result of the some action - new show release.

```js
function notifyMe(showName) {
	// here I can decide what to do with incoming information
}

function subscribe(notifierFuction) {
	// if there is a new specific show, call me
	notifierFuction('Stranger things')
}
```


Real time application, so called webhooks etc.



### Real life task

Using function combination, write a small program. Which takes 3 arguments.
- a - number
- b - number
- c - function which sums two variables

Algorithm of the main function
1. Multiply numbers
2. Result of the multiplication divide by the result of the *action*

I'm intentionally not saying result of the sum, because we can pass any function that takes two arguments.

---



