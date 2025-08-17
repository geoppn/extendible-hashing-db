# Extendible Hashing DBMS

Georgios Papaioannou
Michail Aretakis

A C project implementing a block-based extendible hashing database with primary and secondary hash tables.

## Structure

- `src/`: Core source files ([hash_file.c](src/hash_file.c), [sht_file.c](src/sht_file.c))
- `include/`: Headers ([bf.h](include/bf.h), [hash_file.h](include/hash_file.h), [sht_file.h](include/sht_file.h))
- `lib/`: Block file library ([libbf.so](lib/libbf.so))
- `examples/`: Test programs ([ht_main.c](examples/ht_main.c), [sht_main.c](examples/sht_main.c), [bf_main.c](examples/bf_main.c))
- `Makefile`: Build and clean commands
- `README.md`: Project overview
- `LICENSE`: MIT License

## Features

- **Primary Hash Table**: Extendible hashing for fast record insertion and lookup.
- **Secondary Hash Table**: Indexes on record attributes (e.g., city, surname) for efficient secondary queries.
- **Inner Join**: Fast join operations between secondary indexes.
- **Block File Layer**: Efficient disk/memory management via [libbf.so](lib/libbf.so).
- **Unit Tests**: Comprehensive tests in [examples/sht_main.c](examples/sht_main.c).


