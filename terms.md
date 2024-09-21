# Terms

## codepoint
A number (represented in hexadecimal) that represents a single block of data in Unicode text encoding. As long as it's not in the Private Use Area, codepoints are generally 1:1 consistent across platforms and systems (as long as it has the software updates and/or fonts to display the characters that are being encoded).

Traditional notation for Unicode codepoints is to add "U+" and then the hexadecimal number (eg. 'U+2764`). To save space and make documentation to read, all Mutant documentation foregoes this prefix ('2764').

Sometimes an emoji is just defined by one codepoint, but many are defined by a *sequence* of codepoints (eg. `2764 fe0f`.)


## shortcode 
A string that represents an approachable and linguistic shorthand for people to input emoji in various platforms and software. Shortcodes are not universal across all emoji sets and/or platforms.

If you see a shortcode in Mutant documentation, the only guarantee that you have is that it works in Mutant. (Though I often make shortcodes similar to other systems.)


## ZWJ
**Zero-width joiner**. It is an invisible character that contextually joins the characters on either side.

This was originally developed for scripts such as Arabic or Indic scripts, but this has also been used in emoji. In emoji it generally means 'take these two symbols and combine them into a single new symbol'. They are often used to make certain symbols look a bit more backwards compatible to devices that don't support the emoji in question.

In Unicode, the codepoint for a ZWJ is `200d`. To make ZWJs semantically obvious, documentation in Mutant often uses `\[ZWJ]` in place of `200d` when outlining codepoint sequences.

[More information on ZWJs from Wikipedia](https://en.wikipedia.org/wiki/Zero-width_joiner)


## VS16
**Variation Selector 16**.

In Unicode, a Variation Selector indicates how a character should be depicted. There are 16 different Variation Selectors. Number 16 indicates that the character before is supposed to be an emoji.

VS16 is generally used to convert symbols that existed before emoji into emoji. A popular example is `U+2764` *Heavy Black Heart* (❤). This released in Version 1 of Unicode in 1993. When it came time to encode a heart as an emoji, Unicode did not assign a new codepoint, they simply added VS16 to Heavy Black Heart.

| symbol | codepoint(s) (U+) | As it appears on your computer right now |
| ---- | ---- | ---- |
| Heavy Black Heart | `2764` | ❤ |
| Heavy Black Heart (as emoji) | `2764 fe0f` | ❤ |

Variation Selectors are contentious in Emoji, with various systems stripping or disregarding this codepoint wherever present. Depending on how GitHub works and how your computer works, you may see the two symbols above in the same way or in different ways. Mutant's current position is that VS16 should be used wherever specified in the Unicode standard.

The codepoint for VS16 is `fe0f`. To make VS16 semantically obvious, documentation in Mutant often uses `\[VS16]` in place of `fe0f` when outlining codepoint sequences.

[More information on Variation Selectors from Wikipedia](https://en.wikipedia.org/wiki/Variation_Selectors_(Unicode_block))
