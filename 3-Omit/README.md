## Challenge 3 - Omit

- **Difficulty**: Medium

### Comments

This one took me some time, but I achieved a rather uncommon result to pass on all tests, but the more simple solution is the one most probably go.

```ts
type MyOmit<T, K> = { 
    [P in keyof T as P extends K ? never : P]: T[P] 
};
```

My solution used a generic auxiliar to acheive the same result in the tests, but it's a more risk solution and more easy to exploit, so I don't recommend it.