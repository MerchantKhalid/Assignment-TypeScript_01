
## 1. Use of Enums in TypeScript

Enums allow us to define a set of named constants, making code more readable and maintainable. They can be **numeric** or **string-based**.

### Numeric Enum Example
```ts
enum Direction {
    East = 1,
    West,
    North,
    South
}

let move: Direction = Direction.East;
console.log(move);


### String Enum Example: User Roles

enum UserRole {
    Admin = "ADMIN",
    Moderator = "MOD",
    Subscriber = "SUB"
}

let currentUserRole: UserRole = UserRole.Moderator;
console.log(currentUserRole);



### Union and Intersection Types in TypeScript



### Union Types

### A union type allows a variable to hold more than one type.

let value: string | number;
value = "Hello"; // its valid
value = 42;      // its also valid


### Intersection Types

## An intersection type combines multiple types into one, so the variable must satisfy all types.

type Author = {
    fullName: string;
    booksWritten: number;
};

type Contact = {
    email: string;
    phone: string;
};

type AuthorContactInfo = Author & Contact;

const author: AuthorContactInfo = {
    fullName: "khalid hasan",
    booksWritten: 5,
    email: "khalidhasan@gmail.com",
    phone: "920102458"
};



