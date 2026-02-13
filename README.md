# Ziglings

My solutions to the Ziglings exercises in an attempt to learn the Zig programming language!

## Advanced Usage

To check just a single exercise:

```
zig build -Dn=19
```

Or run all exercises, starting from a specific one:

```
zig build -Ds=27
```

Or let Ziglings pick an exercise for you:

```
zig build -Drandom
```

You can also run without checking for correctness:

```
zig build -Dn=19 test
```

Or skip the build system entirely and interact directly with the
compiler if you're into that sort of thing:

```
zig run exercises/001_hello.zig
```

Calling all wizards: To prepare an executable for debugging,
install it to zig-cache/bin with:

```
zig build -Dn=19 install
```

To get a list of all possible options, run:

```
zig build -Dn=19 -l

  install          Install 019_functions2.zig to prefix path
  uninstall        Uninstall 019_functions2.zig from prefix path
  test             Run 019_functions2.zig without checking output
  ...
```

To reset the progress (have it run all the exercises that have already been completed):

```
zig build -Dreset
```
