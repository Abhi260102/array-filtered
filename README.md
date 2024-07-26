# Array Filter Package

## Install with npm

npm install array-filter2

## Overview

The `array-filter2` package provides a simple and effective way to filter array in your JavaScript/TypeScript projects. This package allows you to  filter array on condition basis various formats with ease.

## Installation

To install the `npm install array-filter2` package, use the following npm command:

```bash
npm install array-filter2



Importing the Package

import { useFilterArray } from 'array-filter2';


Uses

#Filtering an array of numbers
const numbers = [1, 2, 3, 4, 5, 6];
const isEven = num => num % 2 === 0;
useFilterArray(numbers, isEven) ;  Output: [2, 4, 6]


#Filtering an array of strings
const strings = ['apple', 'banana', 'cherry', 'date'];
const containsA = str => str.includes('a');
useFilterArray(strings, containsA); // Output: ['apple', 'banana', 'date']



#Filtering an array of objects
const people = [
  { name: 'John', age: 25 },
  { name: 'Jane', age: 30 },
  { name: 'Jim', age: 35 },
];
const isOver30 = person => person.age > 30;
useFilterArray(people, isOver30); // Output: [{ name: 'Jim', age: 35 }]





# Filtering an array of mixed types
const mixedArray = [1, 'apple', { name: 'John' }, 2, 'banana', { age: 30 }];
const isString = item => typeof item === 'string';
useFilterArray(mixedArray, isString); // Output: ['apple', 'banana']
