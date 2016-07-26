PyProg
=========

PyProg is a simple, aesthetically-pleasing command line progress bar written in Python 3 which uses Unicode blocks for the smoothest progression possible.

## Use

Print progress in terms of `1.0`:
``` python
print_progress(0.5)
▏███████████████████████████████████                                   ▕ 50.0%
```

Print progress in terms of any number:
``` python
print_progress(27, 54)
▏███████████████████████████████████                                   ▕ 50.0%
```

Print progress with a different size progress bar
``` python
print_progress(10, 20, length=30)
▏███████████████               ▕ 50.0%
```

Print progress without percent:
``` python
print_progress(10, 16, percent=False)
▏███████████████████████████████████████████▋                          ▕
```

PyProg inserts a carriage return at the end of each line so that `print_progress()` can be called repeatedly to update the same line; this can be disabled by passing the argument `reset=False`.
