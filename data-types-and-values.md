## Introduction

The ECMAScript language is popularly know as JavaScript. The current latest version is ECMAScript 2020 (ES2020). From here on I will refer to it as ES2020 or JavaScript.

## Basics

### Data Types and Values

JavaScript has the following eight primitive data types.

- Undefined
- Null
- Boolean
- String
- Symbol
- Number
- BigInt
- Object

> Note: The statement that says JavaScript has no type is incorrect. JavaScript has types, but there is no type notation for a variable, because it is a dynamically typed language, which means a variable can hold any type of value and the type of value it holds can be changed at runtime. That is a variable which initially had string value can end up being a function.

1. The **Undefined** type has exactly one value, called `undefined`.

2. The **Null** type has exactly one value, called `null`.

3. The **Boolean** type has exactly two values, called `true` and `false`.

4. The **String** type is the set of all ordered sequences of zero or more 16-bit (UTF-16) unsigned integer values (“elements”) up to a
   maximum length of 2^53 - 1 elements.

5. The **Symbol** type is the set of all non-String values that may be used as the key of an **Object** property. Each Symbol value **immutably** holds an associated value called [[Description]] that is either **undefined** or a **String**
   value.

   > There are some well-known symbols which are built-in to the language, like `Symbol.iterator`.

6. The **Number** type has exactly 18437736874454810627 (that is, 2^64 - 2^53 + 3 R ) values, representing the double-precision 64-bit format.
   > There are three special values to **Number** type,
   >
   > 1. **NaN** (Note: `NaN` != `NaN`, `-NaN` => `NaN`)
   > 2. **+Infinity**
   > 3. **-Infinity**

> Note that there is both a **positive zero** **+0** and a **negative zero** **-0**.

7. The **BigInt** type represents a mathematical integer value. The value may be any size and is not limited to a particular bit-width. The unit value is represented as `1n`.

8. The **Object** type represents a collection properties. Each property is either a data property or an accessor property.

- **Data property** -> associates a key with an ECMAScript language value, and a set of Boolean attributes.
- **Accessor property** -> associates a key with accessor functions, and a set of Boolean attributes. The accessor functions are `get` and `set` corresponding to value retrieval and assignment. These properties include both own properties and inherited properties.
- **Property Key** -> is either string or symbol -**Property Attributes**

  > For Data Properties

  | Attributes       | Value Domain   |
  | ---------------- | -------------- |
  | [[Value]]        | Any value type |
  | [[Writable]]     | Boolean        |
  | [[Enumerable]]   | Boolean        |
  | [[Configurable]] | Boolean        |


    > For Accessor properties

    | Attributes       | Value Domain   |
    | ---------------- | -------------- |
    | [[Get]] | Function object |
    | [[Set]] | Function object |
    | [[Enumerable]] | Boolean |
    | [[Configurable]] | Boolean |
