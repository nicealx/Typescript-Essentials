# nicealx-JSFE2023Q4
___

# My TypeScript Exploration: Earned Badges 🎯

## Badges Overview
____

#### [Link to my Bages Overview](./TypeScript-Badges-Compilation.md)
### Here's a collection of badges I got from taking the TypeScript modules in Microsoft Learn:

1. **Getting Started with TypeScript**: [Badge](https://learn.microsoft.com/api/achievements/share/ru-ru/nicealx-6938/4S29NDWK?sharingId=495664853F7558C8)
2. **Declare Variable Types in TypeScript**: [Badge](https://learn.microsoft.com/api/achievements/share/ru-ru/nicealx-6938/3XLMGP9H?sharingId=495664853F7558C8)
3. **Implement Interfaces in TypeScript**: [Badge](https://learn.microsoft.com/api/achievements/share/ru-ru/nicealx-6938/UF5MHMC3?sharingId=495664853F7558C8)
4. **Develop Typed Functions in TypeScript**: [Badge](https://learn.microsoft.com/api/achievements/share/ru-ru/nicealx-6938/PTZ3JNV4?sharingId=495664853F7558C8)
5. **Declare and Instantiate Classes in TypeScript**: [Badge](https://learn.microsoft.com/api/achievements/share/ru-ru/nicealx-6938/3XLQLUMH?sharingId=495664853F7558C8)
6. **Generics in TypeScript**: [Badge](https://learn.microsoft.com/api/achievements/share/ru-ru/nicealx-6938/ZPFC6Y42?sharingId=495664853F7558C8)
7. **Work with External Libraries in TypeScript**: [Badge](https://learn.microsoft.com/api/achievements/share/ru-ru/nicealx-6938/FZUTLT2X?sharingId=495664853F7558C8)
8. **Organize Code with Namespaces in TypeScript**: [Badge](https://learn.microsoft.com/api/achievements/share/ru-ru/nicealx-6938/HYGTMLZ8?sharingId=495664853F7558C8)

## Reflections
____

#### [Link to my Reflections](./TypeScript-Modules-Reflections.md)

#### These are my reflections after going through eight modules on TypeScript from Microsoft Learning.

##### 1. Getting Started with TypeScript. 🚀
___
I got to know TypeScript and learnt that it is an extended version of JavaScript. The main feature of TypeScript is its static typing. Thanks to TypeScript's static typing, we can see errors in the code before it is executed. TypeScript is easy to maintain, it is easy to understand how the code works. Assigning a type is not always necessary, if a variable is assigned a value during initialisation, TypeScript automatically determines the type of the variable. Learned how to set up a workspace to work with TypeScript. Installed the compiler. Practiced writing code in TypeScript. Compiled the first code written in TypeScript and ran it in a browser. All code written using TypeScript runs in `"use strict"` mode after compilation


##### 2. Declare Variable Types in TypeScript. 🔠
____
In TypeScript as well as in JavaScript, the `let` and `const` keywords are used when declaring variables.

Types in TypeScript
Main type `any`
Subtypes of type `any`:
1. Primitive:
- boolean
- number
- string
- enum
- void
- null
- undefined

2. Object types:
- class
- interface
- array
- literals

3. Parameters of types.

TypeScript gives you the ability to assign an explicit type to variables. Learned what `enum` is. Learned that all types are subtypes of the `any` type. That using the `any` type is undesirable because of unpredictable code behaviour, TypeScript will not be able to track this. That the assignment of types is optional, but that by specifying them you are making it clear exactly how they can be interacted with in the code, which will allow TypeScript to detect errors in the code before it is executed. The `unknow` type is almost the same as `any`, but it does not allow you to access the methods of a variable, nor can you call them and assign values to them. You can assign a type using `as` or `<type>`. The Union type allows you to assign a variable a list of types that it can use. Type Intersection allows you to combine multiple types into one generic type. Literal types are a specific subtype of a generic type. This means that `"Hello World"` is a `string`, but a `string` is not `"Hello World"` in the type system. A literal type definition is a type definition creates a literal type that can contain one of several values of type `string` or `number`. Collection types. Arrays can be written in one of two ways. We can use an element type followed by the square brackets `type[ ]` to denote an array of that element type or `Array<type>`. There is no difference in them, whichever variant you like better, you can use it. Tuples are a list of certain sequences of types in an array of a certain length. For example `[string, number]` can have only 2 elements and only types `string` and `number` and only in the sequence as they are specified in the declaration. You cannot add elements to a tuple, but you can replace them, but only with values of the same types as specified in the declaration.

##### 3. Implement Interfaces in TypeScript. 🧩
____
Interfaces are a way of describing a set of variables and their types, a kind of instruction that an object or function should contain. This ensures that no other data will get into the object or function, and will be of a certain type. Interfaces are very useful when working with third-party libraries. It gives more control over the values passed/received. An interface can be extended by another interface, but if both interfaces contain the same variable names, then these names must contain the same type, otherwise there will be an error. Interfaces can have the same name, then they are automatically expanded into one interface.

##### 4. Develop Typed Functions in TypeScript. ♾️
____
Function declarations in TypeScript are the same as in JavaScript, declaration, expression and arrow. But when declaring a function, if arguments are passed to it, then the parameters must be assigned types. You also need to indicate what type is expected when executing the function.
If the function does not return anything, you can not specify a return type, or you can specify a `void` type. Parameters may be optional; for this purpose, after the parameter, before the type, the symbol `?` is indicated. Parameters can be assigned default values by using the `=` symbol. If the number of parameters is unknown, then you can use the rest operator `...` indicating the types, for example `number[ ]`. You can create an interface or type with parameter types and use it when declaring a function. When typing a function, it is easier to understand what data the function can receive and what is expected when it is executed.

##### 5. Declare and Instantiate Classes in TypeScript. 🧑🏻‍🦱
____
Classes in TypeScript are created and behave exactly the same as in JavaScript. When declaring class parameters, a `_` character is added before the parameter name to distinguish it from constructor parameters. The main difference between classes in TypeScript and JavaScript is the presence of access modifiers: `public` (by default, all members of the class have this type, you don’t have to specify it), `private` (if you specify this type, it will not be possible to access it outside the class containing it class), `protected` (almost the same as `private`, except that class members will be available in derived classes), `readonly` (read-only properties), `static` (properties and methods are common to all instances of the class), modifier type `static` can be used with other types of modifiers.
When calling a static method, we use the class name, not `this`.
When creating an interface for a class, we specify only the public parameters of the constructor; the interface can only describe the public part of the class.
The use of an interface in a class is implemented using the `implements` keyword between the class name and the interface name.

##### 6. Generics in TypeScript. 🎲
____
Generics in TypeScript are a flexible template for creating objects. We can write a function that creates an array by specifying a key value of the form `<T>` - where `T` is any letter or set of letters, this allows us to specify what type of elements in the array should be when calling the function. Which saves us from writing monotonous code.

Example:
`function getArray<T>(items : T[]) : T[] {
     return new Array<T>().concat(items);
}`

So when declaring a type in `<...>` we can use Union Types to restrict the allowed types.

Example:
`type ValidTypes = string | number;`

`function identity<T extends ValidTypes, U> (value: T, message: U) : T {
     let result: T = value + value; // Error
     console.log(message);
     return result
}`


Despite this method of protecting against getting values in the form in which we wanted, for this we can use `if` with a type check, for primitive types it is `typeof`, for a class type it is `instanceof`.
Generics can use a class as a type.

##### 7. Work with External Libraries in TypeScript. 📚
____
With the advent of version EC6, support for modules appeared in JavaScript, and TypeScript fully supports this modularity system. Thanks to the compiler, we can choose for which boot system we need a module. Supported loading systems: **Node.js (CommonJS), require.js (AMD), UMD, SystemJS or native ECMAScript 2015 (ES6) modules**
To indicate which system we need a module for, we specify a command like this for compilation:
`tsc --module modulename main.ts`
where modulename is one of the boot systems listed above.
To run a module from a web page, we need to set the `module` value to `type`.
`<script type="module" src=".\main.js"></script>`

##### 8. Organize Code with Namespaces in TypeScript. 🗃
____
A namespace is the old version of creating a local scope for variables, functions, classes, etc., which can only be accessed by using the `export` keyword from `namespace`.
Example:
`namespace Greetings {
     export function returnGreeting(greeting: string) {
         console.log(`The message from namespace Greetings is ${greeting}.`);
     }
}`
We can only access the function using the namespace name.
`Greetings.returnGreeting('Hello')`
If we have `namespace` written in one file, but we want to use it in another, like a modular system, then in the file we use we must write:
`/// <reference path="filename.ts" />`.

This is now deprecated and a modular approach is best.

Using TypeScript for development at first seems like an unnecessary set of additional code, but if you think about it, strong typing is very convenient for clearly understanding what you expect from the program, what types accept or return functions, etc. This code is easier to work with and debug.
