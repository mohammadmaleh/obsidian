## New types added to JavaScript 
- `any` (allow anything)
-  [`unknown`](https://www.typescriptlang.org/play#example/unknown-and-never) (ensure someone using this type declares what the type is),
- [`never`](https://www.typescriptlang.org/play#example/unknown-and-never) (it’s not possible that this type could happen), and 
- `void` (a function which returns `undefined` or has no return value).

#
## Composing Types

With TypeScript, you can create complex types by combining simple ones. There are two popular ways to do so: unions and generics.

### Unions

With a union, you can declare that a type could be one of many types. For example, you can describe a `boolean` type as being either `true` or `false`:

`   type MyBool = true | false;   `

### Generics

Generics provide variables to types. A common example is an array. An array without generics could contain anything. An array with generics can describe the values that the array contains.

type StringArray = Array<string>;
type NumberArray = Array<number>;
type ObjectWithNameArray = Array<{ name: string }>;







