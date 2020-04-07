## Data Types and Values

The ECMAScript language has following primitive data types.

- Undefined
- Null
- Boolean
- String
- Symbol
- Number
- BigInt
- Object

1. The **Undefined** type has exactly one value, called `undefined`
2. The **Null** type has exactly one value, called `null`.
3. The **Boolean** type has exactly two values, called `true` and `false`.
4. The **String** type is the set of all ordered sequences of zero or more 16-bit (UTF-16) unsigned integer values (“elements”) up to a
maximum length of 2^53 - 1 elements.
5. The **Symbol** type is the set of all non-String values that may be used as the key of an **Object** property. Each Symbol value **immutably** holds an associated value called [[Description]] that is either **undefined** or a **String**
value.
> There are some well-known symbols which are built-in to the language, like `Symbol.iterator`.
6. The **Number** type has exactly 18437736874454810627 (that is, 2^64 - 2^53 + 3 R ) values, representing the double-precision 64-bit format.
> There are three special values to **Number** type,
> 1. **NaN** (Note: `NaN` != `NaN`, `-NaN` => `NaN`)
> 2. **+Infinity**
> 3. **-Infinity**

> Note that there is both a **positive zero** and a **negative zero**.
7. The **BigInt** type represents a mathematical integer value. The value may be any size and is not limited to a particular bit-width. The unit value is represented as `1n`.
8. 
