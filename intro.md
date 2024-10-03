# What is Mutant?

Mutant is an emoji set and a new emoji encoding standard (the latter of which this document describes).

While it is compatible with certain Unicode emoji and characters, both in intent and structure, it is not necessarily an extension of Unicode Standard emoji. Various Unicode emoji characters are altered or ignored entirely.

## Why a different standard?
- Unicode and big tech companies should not have a monopoly on digital graphical communication.
- Unicode’s encoding decisions are largely driven by popularity.
- There are needs from various people, such as minority groups, who are unlikely to get emoji they would like into the Unicode Standard, precisely because Unicode is largely a popularity-based standard.
- Unicode has made (in the eyes of this project) various missteps in how to technically structure codepoints, leading to some serious cultural pitfalls (ie. gendered emoji).
- Unicode’s emoji system represents a cultural, political and economic status quo.
- Unicode emoji encoding is poorly described, and many design decisions are either compensating for those failings, or compensating for how big tech companies (especially Apple) choose to represent emoji in the wake of those failings.

## Why a technical standard?
- It enables as many people to benefit from Mutant emoji as much as possible.

## Key points about Mutant Standard encodings
- All people-based glyphs are gender-neutral.
- All gendered Unicode emoji are not used.
- Family and couple ZWJs (in planning - these emoji are not yet implemented) are not used in favour of letting people place different people together in any configuration they want.
