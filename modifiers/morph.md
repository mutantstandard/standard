# Morph Modifiers (MMs)
**Morph Modifiers change the shape/presentation of an expression without changing the
fundamental expression itself. These are primarily designed for hand emoji.**

Morph Modifiers work just like skin tone modifiers - they are combined with a base expression
to create a modified version of that expression.

Morph Modifiers are exclusive to Mutant Standard. Unlike CMs, there is no analogous type of
encoding in the Unicode Standard.


| codepoint (U+) | Mutant shortcode | Name/Description |
| ---- | ---- | ---- |
| (nothing) | hmn | humanoid hand |
| 101650 | paw | paw hand |
| 101651 | clw | clawed hand |
| 101652 | hoof | hoof hand |

## Humanoid hands (unmodified)
Mutant Standard uses MMs to encode different types of hands (ie. paw hands and claw hands)
with the same expression. As with Unicode Standard emoji, the ‘base expression’ (thumbs up,
V, fist, etc.) is assumed to be a humanoid hand by default, so in this way, MMs are a
backwards-compatible extension to Unicode emoji.

Unicode doesn’t specify what type of hand should be this expression, but in Mutant
Standard, un-modified hands are expected to be humanoid in order to formalise assumptions
made by other emoji vendors and ensure the best possible cross-vendor compatibility.
In shortcodes however, there is no default - the indicator ‘hmn’ is always used to indicate/
disambiguate humanoid emoji from other versions.

## Other hands
Each different hand morph is anthropomorphised to the extent that it is generally capable of
creating the same expressions as a humanoid hand (so that it may mirror the expression of
the original emoji).
