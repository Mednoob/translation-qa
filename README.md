# My Translation QA
Lists of things to check when I'm creating a Kata translation

- Make sure there are random tests, of course
- If you're dealing with array inputs, don't forget to make a copy of the array (shallow or deep, depends on case).
- Make sure everything goes within the boundary / specs of kata
- If you're dealing with codes in preload, make sure that functions and objects from the preload cannot be modified by user.
- Assertions must be inside of `it`. Never put it inside `describe` or outside of them.
- Use `assert.strictEqual` for equality of primal types, and `assert.deepEqual` for equality of objects and arrays
- Add edge cases if it's possible to do so.
- Fixed tests must be available in both actual and sample tests
- When dealing with PRNG, make sure whether the PRNG is end-exclusive or end-inclusive.
- For tests that will be done on multiple times / patterns but only differs in numbers, they should be converted to a function.
- Reference solution must be put inside the `describe` / `it` block of the random tests. Never outside.
- If you're dealing with array inputs, make sure that the reference solution doesn't mutate / modify the input array. You can make a copy if it does mutate them.
- Make sure that the description will be language agnostic when the language has been added.
- If you're dealing with code challenges that needs restrictions, make sure **every single restriction** is implemented.
- Make sure that random tests can cover as much cases as possible.

Last update: 23 / 05 / 2024
