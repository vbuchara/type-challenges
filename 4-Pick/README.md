## Challenge 4 - Pick

- **Difficulty**: Easy

### Comments

This one was rather easy to solve. Only problem I had was with extending the **`K`** type, which doing so it extends **`PropertyKey`** doesn't throw an Error that **`@ts-expect-error`** is excepting. The solution is simple, as you should make **`K`** extends the keys of **`T`** with **`keyof T`**.

