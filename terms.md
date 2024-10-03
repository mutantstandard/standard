# Terms

## name
Every standard unicode codepoint has an assigned name. This is a line of text in English describing what this codepoint is. This name is essentially a very brief description of how to design your own version of that character for your own fonts.

### Unicode name
The name of a codepoint as it appears in the Unicode Standard.

### Mutant name
The name of a codepoint as it appears in Mutant's Standard. Mutant's use of codepoints and names follows Unicode's with some explicit deviations. When there is an explicit deviation, a non-standard sequence or involves Mutant's PUA, it has a **Mutant name**.

## codepoint
A number (represented in hexadecimal) that represents a single block of data in Unicode text encoding. As long as it's not in the Private Use Area, codepoints are generally 1:1 consistent across platforms and systems (as long as it has the software updates and/or fonts to display the characters that are being encoded).

Traditional notation for Unicode codepoints is to add "U+" and then the hexadecimal number (eg. 'U+2764`). To save space and make documentation to read, all Mutant documentation skips this prefix ('2764').

Sometimes an emoji is just defined by one codepoint, but many are defined by a *sequence* of codepoints (eg. `2764` `fe0f`.)

### Unicode codepoint
The codepoint sequence as it appears in the Unicode Standard.

### Mutant codepoint
A *Private Use Area* or otherwise non-standard codepoint sequence made for Mutant's own standard.

### Private Use Area (PUA)
Unicode outlines sections of codepoints that are designated as 'private use' - this means anyone can claim them for their own non-standard encodings. Some of the largest historical use of PUAs has been used for scripts for constructed languages.

Some of Mutant's unique emoji symbols and modifiers have been encoded in the SPUA plane, in block `1016xx`. This repository outlines what encodings have been made by the project in this area (and potentially subsequent blocks if `1016xx` is filled).

PUA encodings in Unicode are inherently non-standard, there may be collisions that exist. There are also accessibility concerns too, such as operating systems not being able to describe codepoints in PUA areas to those who use screenreaders. Please take things like this into consideration when using any PUA encoding.


## shortcode 
A string that represents an approachable and linguistic shorthand for people to input emoji in various platforms and software. Shortcodes are not universal across all emoji sets and/or platforms.

If you see a shortcode in Mutant documentation, the only guarantee that you have is that it works in Mutant. (Though, shortcodes are often made similar to other systems in practice, notably Discord.)


## modifier

In character encoding, a modifier changes the shape/presentation of an expression without changing the fundamental expression itself.

In typical emoji encoding, modifiers perform these functions:

- Skin tones in symbols where human forms are present.
- Combining symbols into new ones via a Zero-Width Joiner (ZWJ - `U+200d`).
- Marking legacy symbols to display like emoji instead of grayscale characters (VS16 - `fe0f`).

One of Mutant's design goals is for people who use nonhuman characters/personas/representations to have symbols that represent them better, so in **Mutant Form**, the idea of using skin tones has been greatly extended beyond what Unicode has created.


## ZWJ
**Zero-width joiner**. It is a modifier that contextually joins the characters on either side.

This was originally developed for scripts such as Arabic or Indic scripts, but this has also been used in emoji. In emoji it generally means 'take these two symbols and combine them into a single new symbol'. They are often used to make certain symbols look a bit more backwards compatible to devices that don't support the emoji in question.

In Unicode, the codepoint for a ZWJ is `200d`. To make ZWJs semantically obvious, documentation in Mutant often uses `[ZWJ]` in place of `200d` when outlining codepoint sequences.

[More information on ZWJs from Wikipedia](https://en.wikipedia.org/wiki/Zero-width_joiner)


## VS16
**Variation Selector 16**.

In Unicode, a Variation Selector is a modifier indicating how the previous character should be depicted. There are 16 different Variation Selectors. Number 16 indicates that the character before is supposed to be an emoji.

VS16 is generally used to convert symbols that existed before emoji into emoji. A popular example is `U+2764` *Heavy Black Heart* (❤). This released in Version 1 of Unicode in 1993. When it came time to encode a heart as an emoji, Unicode did not assign a new codepoint, they simply added VS16 to Heavy Black Heart.

| symbol | codepoint(s) (U+) | As it appears on your computer right now |
| ---- | ---- | ---- |
| Heavy Black Heart | `2764` | ❤ |
| Heavy Black Heart (as emoji) | `2764` `fe0f` | ❤ |

Variation Selectors are contentious in Emoji, with various systems stripping or disregarding this codepoint wherever present. Depending on how GitHub works and how your computer works, you may see the two symbols above in the same way or in different ways. Mutant's current position is that VS16 should be used wherever specified in the Unicode standard, and standard VS16 use is present in all Mutant releases.

The codepoint for VS16 is `fe0f`. To make VS16 semantically obvious, documentation in Mutant often uses `[VS16]` in place of `fe0f` when outlining codepoint sequences.

[More information on Variation Selectors from Wikipedia](https://en.wikipedia.org/wiki/Variation_Selectors_(Unicode_block))
