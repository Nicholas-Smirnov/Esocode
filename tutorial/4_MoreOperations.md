# Esocode Tutorial; Part 4

### The Swap Operation

The `SWAP` operation, does exactly what is sounds like. It swaps the values of 2 storage nodes. 
Here is an example on how to use this operation.

```
[0]
    EQUAL 10
[1]
    EQUAL 39
    SWAP [0] [1]
    OUTPUT
```
And the output will turn out to be:
```
10
```
Quick Thing: The `SWAP` operation doesn't target the referenced storage node. It just takes 2 arguments.

### The Compare Operation

The `COMPARE` operation only works with integers. This operation will take two arguments likewise, and will then
compare which value is larger. It will return `1` if the first value given is greater, `0` if they are equal, and
`-1` if the second argument is greater. Here are 2 example of how to use the `COMPARE` operation.
```
[0]
    EQUAL 100
[1]
    COMPARE [0] 10
```
and
```
[0]
    EQUAL 100
[1]
    EQUAL 150
[2]
    COMPARE [0] [1]
```
Now this is important! Other argument positioning will be invalid. So these 2 examples will be invalid:
```
[0]
    EQUAL 100
[1]
    COMPARE 10 [0]
```
and
```
[0]
    COMPARE 10 105
```
So basically in other words, the first argument of the operation has to be a storage node. The second argument can either be a storage node or a constant.
