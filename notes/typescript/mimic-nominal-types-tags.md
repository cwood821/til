# Mimic nominal typing with tags in TypeScript

TypeScript is structurally typed, which means roughly that two types that share a similar shape will be treated as the same type.

This may not be what you want when domain modeling with types. For example, this works: 
```ts

type Address = string;
type Email = string;

let email = "test@example.com" as Email;

function makeAddress(address: Address): Address {
  return address;
}

let value = makeAddress(email);
```

To make two types which share the same underlying basic data type different, we can tag types in TypeScript with a string literal. This example will be show an error:

```ts
class Tagged<T> { private _tag: T };
type Nominal<Type, Tag> = Type & Tagged<Tag>;

type Email = Nominal<string, 'Email'>;
type Address = Nominal<string, 'Address'>;

function makeAddress(add: Address): string {
  return add;
}

let email = "test@example.com" as Email;

let add = makeAddress(email);
```

Hat tip to [this post](https://betterprogramming.pub/nominal-typescript-eee36e9432d2).