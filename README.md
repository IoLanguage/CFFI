# CFFI 
A C function interface for Io.

# Installation
`libffi` should be installed and foundable in your system. Then:

```
eerie install https://github.com/IoLanguage/CFFI.git
```

If you have problems on macOS try to install `libffi` with brew and forcefully link it:
```
brew install libffi
brew ln --force libffi
```

## TODO

- Bitfields
- Endianness
- Variable length arrays
- Stronger type/error checking
- Variadic functions
- stdcalls
- struct/union member alignment option (pack)
- 64 bit types
- More and more unit tests
- ...
