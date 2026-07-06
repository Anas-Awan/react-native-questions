# Typescript Interview Questions & Answers


### 1. Type vs Interface
**Question:** What’s the difference between type and interface?
**Answer:**
**Interface:** Best for object contracts, supports declaration merging.
**Type:** More flexible, can represent unions, intersections, primitives, tuples.

### 2. Union vs Intersection
**Question:** Explain union and intersection types.
**Answer:**
**Union (|):** Value can be one of several types.
**Intersection (&):** Value must satisfy all combined types.

### 3. Generics
**Question:** Why are generics important?
**Answer:** They allow reusable, type-safe components.

### 4. Utility Types
**Question:** What are utility types like Partial, Pick, Omit?
**Answer:** Built-in helpers to transform types.

### 5. Unknown vs Any
**Question:** What's the difference between unknown and any?
**Answer:**
**Any:** Disables type checking & completely bypasses compile-time type checking
**Unknown:** Enforces strict type safety by forcing you to verify the type before performing operations

### 6. Discriminated Unions
**Question:** How do discriminated unions help?
**Answer:** They enable exhaustive type checking in switch statements.

### 7. Strict Mode
**Question:** Why enable strict mode?
**Answer:** It enforces null safety, type inference accuracy, and better maintainability.

### 8. Runtime Validation
**Question:** Does TypeScript guarantee runtime safety?
**Answer:** No. It only enforces types at compile-time. For runtime validation, libraries like Zod or io-ts are used.
