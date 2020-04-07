## Concepts of Functional Programming in Javascript:

### What is functional programming?
**Functional programming** is a programming paradigm a style of building the structure and elements of computer programs, that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

### What is  pure functions?:
We called  a function a function pure when:
- It returns the same result if given the same arguments ``(it is also referred as deterministic)``
- It does not cause any observable side effects

#### Pure functions benefits:
 The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:
- Given a parameter A → expect the function to return value B
- Given a parameter C → expect the function to return value D

### Immutability:
When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

>>
pure functions + immutable data = referential transparency
>>

### Functions as first-class entities:
The idea of functions as first-class entities is that functions are also treated as values and used as data.
Functions as first-class entities can:
- refer to it from constants and variables
- pass it as a parameter to other functions
- return it as result from other functions

###  Higher-order functions:
When we talk about higher-order functions, we mean a function that either:
takes one or more functions as arguments, or
returns a function as its result

### Filter
Given a collection, we want to filter by an attribute. The filter function expects a ``true`` or ``false`` value to determine if the element should or should not be included in the result collection

### Map:
The idea of map is to transform a collection.
The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.

###  Reduce
The idea of reduce is to receive a function and a collection, and return a value created by combining the items.

## Refactoring JavaScript for Performance and Readability:
#### Scenario 1
We're an URL-shortening website, like TinyURL. We accept a long URL and return a short URL that forwards visitors to the long URL. We have two functions.

###  Scenario 2
We're a social media website where user URLs are generated randomly. Instead of random gibberish, we're going to use the friendly-words package that the Glitch team works on. They use this to generate the random names for your recently created projects!

### stratigies:
1. Return early from functions.
2. Cache variables so functions can be read like sentences.
3. Check for Web APIs before implementing your own functionality.
4. 

