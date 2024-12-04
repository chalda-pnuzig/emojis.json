# Emojis.json

This repository contains a comprehensive list of emojis in JSON format, **version 16.0.1**

The data was sourced from the [Full Emoji Data](https://www.unicode.org/emoji/charts/full-emoji-list.html),
**version 16.0**

## Available Files

### Array of all available Emojis

| File                      | Standard | Modifiers | Images |  Size |
|---------------------------|:--------:|:---------:|:------:|------:|
| **array.json**            |    ✔     |     ❌     |   ❌    | 17 KB |
| array.only.modifiers.json |    ✔     |     ✔     |   ❌    | 34 KB |
| array.with.modifiers.json |    ✔     |     ✔     |   ❌    | 51 KB |

### Array of Emoji Objects

| File                                 | Standard | Modifiers | Images |   Size |     
|--------------------------------------|:--------:|:---------:|:------:|-------:|
| **list.json**                        |    ✔     |     ❌     |   ❌    | 216 KB |
| list.only.modifiers.json             |    ❌     |     ✔     |   ❌    | 320 KB |
| list.with.modifiers.json             |    ✔     |     ✔     |   ❌    | 535 KB |
| list.with.images.json                |    ✔     |     ❌     |   ✔    |   7 MB |
| list.only.modifiers.with.images.json |    ❌     |     ✔     |   ✔    |   8 MB |
| list.with.images.with.modifiers.json |    ✔     |     ✔     |   ✔    |  15 MB |
| list.new.json                        |    ❌     |     ❌     |   ❌    |   1 KB |

### Array of Emoji Objects organized by Categories and Subcategories

| File                                       | Standard | Modifiers | Images |   Size |     
|--------------------------------------------|:--------:|:---------:|:------:|-------:|
| **categories.json**                        |    ✔     |     ❌     |   ❌    | 119 KB | 
| categories.only.modifiers.json             |    ❌     |     ✔     |   ❌    | 218 KB | 
| categories.with.modifiers.json             |    ✔     |     ✔     |   ❌    | 337 KB | 
| categories.with.images.json                |    ✔     |     ❌     |   ✔    |   6 MB | 
| categories.only.modifiers.with.images.json |    ❌     |     ✔     |   ✔    |   8 MB | 
| categories.with.images.with.modifiers      |    ✔     |     ✔     |   ✔    |  15 MB |

### Emoji Object Structure:

Each emoji object includes the following properties:

- `code` <_array_> : the code point(s) for the emoji characters and sequences.
- `emoji` <_string_> : The visual representation of the emoji.
- `name` <_string_> :  The CLDR short name for the character or sequence in American English.
- `category` <_string_> : The primary category of the emoji.
- `subcategory` <_string_>: The subcategory under which the emoji falls.
- `image` <_base64|false_> : The emoji image in base64 format, available only in `.with.images` files. False if not present.
