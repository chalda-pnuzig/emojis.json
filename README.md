# Emojis.json

List of all emojis in json format.

The list of emoji was retrieved from [Full Emoji Data](http://www.unicode.org/emoji/charts/full-emoji-list.html), v13.1

There are 4 different files:

- [**array.json**](#array.json)
- [**list.json**](#list.json)
- [**list.images.json**](#list.images.json)
- [**categories.json**](#categories.json)
- [**categories.images.json**](#categories.images.json)

-------------------------------------------------------------------------------

### `array.json`

[`https://unpkg.com/@chalda/emojis.json/dist/array.json`](https://unpkg.com/@chalda/emojis.json/dist/array.json)

Only an array of all available emojis.

-------------------------------------------------------------------------------

### `list.json`

[`https://unpkg.com/@chalda/emojis.json/dist/list.json`](https://unpkg.com/@chalda/emojis.json/dist/list.json)

An array of emojis with some properties:

- `n` <_int_> :  a line count, for reference
- `code` <_array_> : the code point(s) for the emoji characters and sequences
- `emoji` <_string_> : The character
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

-------------------------------------------------------------------------------

### `list.images.json`

[`https://unpkg.com/@chalda/emojis.json/dist/list.images.json`](https://unpkg.com/@chalda/emojis.json/dist/list.images.json)

Same as `list.json` but with the `images` property containing a png representation of the emoji by the respective resource

- `images` <_array_> : array containing the png emoji in base64 by the respective resource, false if not present
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

-------------------------------------------------------------------------------

### `categories.json`

[`https://unpkg.com/@chalda/emojis.json/dist/categories.json`](https://unpkg.com/@chalda/emojis.json/dist/categories.json)

Same as `list.json` but emojis are enclosed in their respective categories and sub-categories

-------------------------------------------------------------------------------

### `categories.images.json`

[`https://unpkg.com/@chalda/emojis.json/dist/categories.images.json`](`https://unpkg.com/@chalda/emojis.json/dist/categories.images.json`)

Same as `list.images.json` but emojis are enclosed in their respective categories and sub-categories
 