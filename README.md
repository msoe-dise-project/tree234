# tree234
Standalone version of the [counted 2-3-4 tree](https://www.chiark.greenend.org.uk/~sgtatham/algorithms/cbtree.html) from PuTTY, written in C.

This is a B-tree that only supports between 2 and 4 values per node.
It has some advanced functionality including:

* tracking the number of elements in each subtree, allowing items to by accessed by index
* user-supplied comparator functions so that the tree can be used with any type of object
* finding the next largest element for a missing key

The implementation provides a number of test cases as well as some logging.

I made some small changes to enable it to compile on my MacOS system.  You can compile the code with:

``` bash
$ ./build.sh
```

You can see that the script simply invokes the C compiler.

The executable runs a bunch of tests when invoked:

``` bash
$ ./tree234
```

