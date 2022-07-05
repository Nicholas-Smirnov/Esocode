### The `EQUAL` Operation

The first basic operation is the `EQUAL` operation, which just sets the referenced storage node with the value given after. 
```
[0] EQUAL 10
```
Here, the storage node referenced at pointer 0, is set to integer 10. However, the interesting thing about this language is that an typing is done automatic. For example, `15256` is an integer. `151h` is a string. No quotations are necessary. Here is an example of this automatic typing.
```
[0] EQUAL 145
[1] EQUAL Hello
```
Quick Thing: Strings cannot have spaces!!!

### Other Basic Operations

There are other basic operations that exist in Esocode. Here they are below.

1. The `PLUS` operation: Can be used with both strings and integers. Combines integers and concatenates strings.
2. The `MINUS`, `MULTIPLY`, `DIVIDE`, `POWER` operations: Only work with integers.

Here is just a quick example on how to use these operations. Quick Tip: Once you reference a storage node, you do not have to rereference it for the next operations if you want these operations to target this specific storage node.
```
[0] EQUAL 10
    PLUS 13
    DIVIDE 15
    MULTIPLY 13
    OUTPUT
```
