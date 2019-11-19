### Lab: Functions

Create a file named `functions.js`.

1.  Define a `youRock` function that accepts a string argument of a name and returns a string using that name.
```js
youRock = (str) => {
  console.log("You rock " + str + "!")
}
youRock('Samar') // 'You rock Samar!'
youRock('Sara') //'You rock Sara!'
```

2.  Define a `square` function that accepts a number argument and returns that number multipled by itself.
```js
square = (n) => {
  return n**2
}
square(2) // 4
square(3) // 9
```

3.  Define a `cube` function that accepts a number argument and returns that number raised to the third power.
```js
cube = (n) => {
  return n**3
}
cube(2) // 8
cube(3) // 27
```

4.  Define a `toTheFourth` function that accepts a number argument and returns that number raised to the fourth power.
```js
toTheFourth = (n) => {
  return n**4
}
toTheFourth(2) // 16
toTheFourth(3) // 81
```

#### Extra Practice

If you finish the Lab, try this challenge.

Write a function that will add, subtract, multiply or divide two numbers and return the answer 
```js
calculator = (n1, n2, command) => {
  if(command == "add") return n1+n2
  else if (command == "subtract") return n1-n2
  else if(command == "multiply") return n1*n2
  else if(command == "divide") return n1/n2
  else return "calculator can only add, subtract, divide, or multiply"
}
calculator(1, 2, "add") // should return 3 
calculator(1, 2, "subtract") // should return -1
calculator(1, 2, "divide") // should return .5
calculator(1, 2, "multiply") // should return 2
calculator(1, 2, "something else") // should return "calculator can only add, subtract, divide, or multiply
calculator("cat", 2, "add") // should return "calculator only accepts numbers"
```

### Lab: FizzBuzz Function

Write a function that accepts an argument of a number

If it is a multiple of 3, return “Fizz” instead of the number.

If it is a multiple of 5, return “Buzz” instead of the number.

If it is a multiple of both 3 and 5, return “FizzBuzz” instead of the number.

Otherwise, return the number

```js
fizzBuzz = (n) => {
  let result = ""
  if(n % 3 == 0) result += "Fizz"
  if(n % 5 == 0) result += "Buzz"
  return result
}
fizzBuzz(3) // Fizz
fizzBuzz(15) // FizzBuzz
fizzBuzz(7) // 7
```

### Lab: RainDrop Function

Write a function that accepts an argument of a number

If the number contains 3 as a factor, output 'Pling'.

If the number contains 5 as a factor, output 'Plang'.

If the number contains 7 as a factor, output 'Plong'.

If the number does not contain 3, 5, or 7 as a factor, output the number as a string.

```js
rainDrop = (n) => {
  result = ""
  if(n % 3 == 0) result += "Pling"
  if(n % 5 == 0) result += "Plang"
  if(n % 7 == 0) result += "Plong"
  if(result === "") result += n
  return result
}
rainDrop(28) // Plong
rainDrop(1755) // PlingPlang
rainDrop(34) // 34
```
