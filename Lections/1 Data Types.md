
## Where we start?

We need a place to store data. We start from variables, how to define variables?
There are specific keywords we can use to define variables: `let`  and  `const`
Historically there is another way `var` - but it's not used. You can find it in old code bases. Main difference is visibility scope.

We are not gonna talk about scope. Only small thing you can think about scope is curly braces. Everything inside curly braces is thought as one scope.

### let vs const

From naming, you already can guess what's the difference. What `const` does?

We use *=* to assign values to variables. Here we have simple string values.
String values -  text. Between double or single quotes. Backticks???

```js
let name = 'John'

const name = 'John'
```
 
 What error we see? Blocked-scoped variable.

> [!Mental note]
> Give an example of scoped variables later on in if-else
> 

```js
let personOne = 'John'

const personTwo = 'John'

// re-assign values


personOne = 'Smith'
personTwo = 'Smith'
```

What kind of error we have here?


## Different data types

### Number

```js
let age = 33;

age = 35;

age = 'Thirty five'

```

Here we see that JS is dynamically typed language, which in big projects can lead to problems. That's why we have TS, to help big team to maintain bigger code bases.

> [!note]
> BigInt, couple of words about 


### Null, undefined

Null - when we want intentionally say there is no value

```js
const noCar = null
```

Undefined - usually appears in cases when what to access some value, but is not there.

> [!info]
> Show, undefined later on arrays or in objects


### Boolean

Boolean - has one of two possible values, it's either `true` or `false`

```js
const hasCar = false
```

Word `has`  (`is`) in the variable naming is intentional, try to keep this rule especially for boolean variables. Because later on if somebody will read code after you, it will show to a reader that a variable stores boolean value

Examples

```js
const hasCar = false;

const isAlive = true
```


## Objects

Tricky area, because how objects stored in memory.

### Arrays

List of the values.

```js

const people = ['John', 'Smith', 'Anderson']

// we can access value by index

console.log(people[0])

// indexing starts from zero.


const peopleCopy = people

peopleCopy[1] = 'Neo'

console.log(people)
```

Why it's like that?
This applies for all objects
[[Drawing 2023-02-20 15.57.15.excalidraw]]


### Objects

It helps to store, complex data type about real "objects".

```js
const person = {
	name: 'John',
	age: 33,
	possesions: ['Car', 'House']
}
```

As you can see we can, combine different data types


```js
const person = {
	name: 'John',
	age: 33,
	possesions: ['Car', 'House']
}

const copyPerson = person;

copyPerson.name = 'Smith'

console.log(person)
```

What is the result we will see? Think about previous image


### How to make a copy which won't change content

Spread operator

---







