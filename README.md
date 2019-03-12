## RISC-V suppliers

This repository keeps a list of entities supplying RISC-V devices or boards.

The IDs are used in the xPack metadata files.

Submit pull request in order, if you need your own ID.

## Fields

### ID

This monotonically increasing numeric field is unique and the only imutable field.

It is intended to be used when stored on persistent storages.

### `name`

This single word short string is unique, and can be used to internally represent 
the supplier during temporary sessions, as key in maps, etc.

It should not be used alone on persistent storages,
since it is not imutable, **if the supplier name changes, it can be updated**, 
as long as uniqueness is preserved.

It may include only lower case ASCII letters.

### `displayName`

A single word short string that can be used to represent the supplier in external
circumstances, like displaying labels in a GUI tree representation.

Normally it should be unique. It may include any UTF-8 characters. 
Unless special cases, the first letter is expected to be capitalised.

### `fullName`

A multi word, resonably long, string that describes the supplier, like an 
official company name, organization name, person name, etc.

Unless special cases, each word is expected to be capitalised.

### `contact`

A generic email address where the supplier can be contacted.

### `url`

The full URL of the supplier web site.

