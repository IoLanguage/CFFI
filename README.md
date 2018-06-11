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

# ChangeLog:

04/20/2010
----------
- Added CString size: gets the size of the underlying Sequence.
- Added LongLong/ULongLong types
- Modified Array size to return the array size in bytes (nitems*itemsize)
- Fix in Pointer cast: don't keepref when casting to CString

04/10/2010
----------
- More unit tests
- Better type casting (Pointer proto)
- Some improvements

03/10/2010
----------

- Added basic Byte types (like Char types) that accept numbers instead of 1-char-strings
- Added Structure and Union complex types allowing "Forward referencing"
- Added Array complex type. Allows flattening inside a Structure. Only fixed length at the moment
- Added ramdom access (read/write) to memory pointed by pointer types
- Modified Function and Library types to allow getting functions directly from a Library
- Added callback (closures) support via Function type
- Added "anonymous functions" to the Function type (that is, calling a c-function knowing its pointer and signature)
- Fixed a GC problem: types that get c-pointers from values, keep an Io reference to the value
- Pointer type casting (very basic)
- Some unit tests for Structure and Union.

TODO:

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
