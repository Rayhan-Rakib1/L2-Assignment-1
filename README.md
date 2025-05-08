✅ 1. What are some differences between interfaces and types in TypeScript?
Both interfaces and types are used to describe the structure of data in TypeScript, but they have some key differences:

Interfaces are specifically designed to describe the shape of objects and are ideal for working with class-based code or object modeling.

Types are more flexible and can be used to describe not only objects but also primitives, unions, intersections, and more complex data structures.

Interfaces support declaration merging, meaning you can define the same interface multiple times and TypeScript will combine them — which is not possible with types.

While both are capable of extending other structures, interfaces are often preferred for building public APIs and libraries because they are more readable and semantically clear.

✅ 2. What is the use of the keyof keyword in TypeScript?
The keyof keyword is used to get a union of all property names (keys) of a given object type. It’s very useful when you want to restrict access to certain keys of an object dynamically, ensuring type safety.

For example, if you have an object with properties like name and age, keyof will allow you to create a variable or function that only accepts "name" or "age" as input — preventing errors like misspelled keys or accessing undefined properties. This helps create more robust and reusable code.

✅ 3. Explain the difference between any, unknown, and never types in TypeScript.
any: Disables type checking. You can assign anything to it and perform any operation — useful in quick prototypes, but dangerous in large projects due to lack of safety.

unknown: A safer version of any. You can assign any value to it, but you must perform type checks before using it — promoting safer coding practices.

never: Represents a value that will never occur. It's used for functions that never return (like functions that always throw errors or have infinite loops). It helps indicate unreachable or erroneous states in your program.

✅ 4. What is the use of enums in TypeScript? Provide an example of a numeric and string enum.
Enums (short for “enumerations”) allow you to define a set of named constants — a group of related values under one name. They make your code more readable and less error-prone when dealing with predefined options.

Numeric enums assign numbers (by default starting from 0) to each member.

String enums assign custom string values to each member, making the output more readable and useful in logs or UI.

Enums are especially helpful when you have a fixed set of possible values like days of the week, roles in a system, or status codes.

