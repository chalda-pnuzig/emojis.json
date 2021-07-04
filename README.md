# Emojis.json

List of all emojis in json format.

The list of emoji was retrieved from [Full Emoji Data](http://www.unicode.org/emoji/charts/full-emoji-list.html), v13.1

There are different files:

### Array of all available emojis

|File                                        | Standard | Modifiers | Images | Size       
|--------------------------------------------|----------|-----------|--------|------------
| **array.json**                             | ✔        | ❌        | ❌     | 16 KB      |
| array.only.modifiers.json                  | ❌        | ✔        | ❌     | 32 KB      |modifiers only
| array.with.modifiers.json                  | ✔        | ✔        | ❌     | 47 KB      |

### Array of emoji objects 
|File                                        | Standard | Modifiers | Images | Size       
|--------------------------------------------|----------|-----------|--------|------------
| **list.json**                              | ✔        | ❌        | ❌     | 514 KB     |
| list.only.modifiers.json                   | ❌        | ✔        | ❌     | 554 KB     |
| list.with.modifiers.json                   | ✔        | ✔        | ❌     | 1068 KB    |
| list.with.images.json                      | ✔        | ❌        | ✔     | 33268 KB  |
| list.only.modifiers.with.images.json       | ❌        | ✔        | ✔     | 32859 KB   |
| list.with.images.with.modifiers.json       | ✔        | ✔        | ✔     | 66127 KB   |

### Array of emoji objects enclosed in their respective categories and sub-categories
|File                                        | Standard | Modifiers | Images | Size       
|--------------------------------------------|----------|-----------|--------|------------
| **categories.json**                        | ✔        | ❌        | ❌     | 423 KB    | 
| categories.only.modifiers.json             | ❌        | ✔        | ❌     | 463 KB    | 
| categories.with.modifiers.json             | ✔        | ✔        | ❌     | 884 KB    | 
| categories.with.images.json                | ✔        | ❌        | ✔     | 33177 KB  | 
| categories.only.modifiers.with.images.json | ❌        | ✔        | ✔     | 32768 KB  | 
| categories.with.images.with.modifiers      | ✔        | ✔        | ✔     | 65944 KB  |



### Emoji Object:

- `code` <_array_> : the code point(s) for the emoji characters and sequences
- `emoji` <_string_> : The emoji character
- `name` <_string_> :  The CLDR short name for the character or sequence in American English
- `category` <_string_> : The main category
- `subcategory` <_string_>: The minor category
- `support` <_array_> : array containing whether the emoji is supported by the respective resource
    - `apple` <_bool_>
    - `google` <_bool_>
    - `facebook` <_bool_>
    - `windows` <_bool_>
    - `twitter` <_bool_>
    - `joypixels` <_bool_>
    - `samsung` <_bool_>
    - `gmail` <_bool_>
    - `softbank` <_bool_>
    - `docomo` <_bool_>
    - `kddi` <_bool_>
- `images` <_array_> :array containing the png emoji in base64 by the respective resource, false if not present (only in the file `.with.images`)
    - `apple` <_base64|false_>
    - `google` <_base64|false_>
    - `facebook` <_base64|false_>
    - `windows` <_base64|false_>
    - `twitter` <_base64|false_>
    - `joypixels` <_base64|false_>
    - `samsung` <_base64|false_>
    - `gmail` <_base64|false_>
    - `softbank` <_base64|false_>
    - `docomo` <_base64|false_>
    - `kddi` <_base64|false_>
