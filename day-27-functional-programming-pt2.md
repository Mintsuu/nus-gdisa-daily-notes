## `.reduce`
- Can omit the accumulator parameter, this means that 2 arguments is necessary for the reducer function, but it'll work with 2 elements on each loop 
- Can only work with the same time (so e.g. when iterating through an object, you'd need to `.map` through the stream of objects and convert it into a stream of primitives, then use reduce to do the function that you're looking for)
- Benefit of using `.reduce` instead of `.filter` for iterating through reference types seems that you'd be able to convert the base type that you're looking for in `.reduce` since `.filter` will still retain the `stream` type, so accessing the value is tougher
