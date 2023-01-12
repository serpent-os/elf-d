elf-d
------------

Reads 32-bit and 64-bit elf binary files.

Features
------------

- Read general elf file properties like file class, abi version, machine isa, ...
- Parse elf sections.
- Read elf symbol tables and string tables.
- Read DWARF line program tables and produce address info (.debug_line section).

How to run example
------------

Run `dub run elf-d:example` in the parent directory. (Note: running the example produces a lot of output to stdout)


How to run scanelf
------------

Run `dub build elf-d:scanelf` in the clone root directory.

After building it, run scanelf with:

    bin/scanelf <path to shared-elf-library.so> |less


TODOs
------------

- Fix endianness issue (currently only native endianness is supported).
- Add interpretation for more sections.

License
------------

Licensed under Boost. Check accompanying file LICENSE_1_0.txt or copy at
http://www.boost.org/LICENSE_1_0.txt

