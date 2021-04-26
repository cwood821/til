# Nominal vs Structural Types

Type systems may use either nominal or structural subtypes schemes.

Nominal subtypes are explicitly defined. Consider `Manager extends Employee` where Manager is a subtype of Empmloyee.

Structural subtypes have all the members of the supertype, and, optiontally others. Consider `Animal` and `Human` types which both have `age` properties -- any case where a type with `age` is required, both are treated as subtypes. This is how TypeScript works.



