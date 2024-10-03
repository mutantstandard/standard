# Color Modifiers (CMs)

These are the only CMs available in the **Mutant Core** bundle. These are the standard Unicode skin tones introduced in 2015 with some differences in shortcode notation and descriptions to provide seamless integration with **Mutant Form**.

The original descriptions of these skin tones was based on the Fitzpatrick scale, which is biased and flawed. As a result, Mutant describes them in more generic terms.

Note that because of the way Mutant notes the lightness of a colour, the shortcodes run in the opposite order to the codepoints. **When implementing these in an interface, follow the shortcode order (h1-h5).**

| Unicode codepoint (U+) | Mutant shortcode | Mutant name |
| ---- | ---- | ---- |
| 1f3fb | h5 | light skin tone |
| 1f3fc | h4 | medium-light skin tone |
| 1f3fd | h3 | medium skin tone |
| 1f3fe | h2 | medium-dark skin tone |
| 1f3ff | h1 | dark skin tone |


## Default colour
In most other emoji sets, the default colour of unmodified emoji is yellow, however, because of the white-coded nature of yellow, Mutant opts for a medium grey, [the same shade as K2 in Mutant Form](../form/cm.md).

