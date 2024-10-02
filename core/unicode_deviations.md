# Unicode deviations

Mutant Core mostly follows Unicode standard emoji, but there are cases when it doesn’t:

- Some emoji designs are changed but maintain the same codepoint as the original symbol concept. Sometimes this is done in a way that still matches the Unicode Standard, sometimes it doesn’t.
- Some emoji are Unicode symbols, but they are not Recommended for General Interchange (RGI) as emoji.
- Some emoji use non-standard ZWJs (Zero-Width Joiners) of Unicode Emoji.
- Some emoji in the Unicode Standard are not used in Mutant at all.
- Some emoji and modifiers are non-standard and encoded in the PUA (Private Use Area).

This document will go into each of the ways that Mutant doesn’t follow either Unicode standards, or common expectations of Unicode standards, one by one.

----

## Implicitly deviated semantics
These are emoji that have specific changes in design from what is traditionally used, but it’s actual intended meaning is no different from the Unicode Standard.

| codepoint(s) (U+) | Unicode name | Notes |
| ---- | ---- | ---- |
| `1f6bb` | Restroom | Practically all other emoji sets depict this as an abstract male and female figure next to each other. In Mutant, it should be a gender-neutral toiler sign. (Though not WC, which is its own emoji in Unicode.) |
| `1f4fd` | Film Projector | Instead of a cinema celluloid projector that is traditionally used, a home/consumer digital projector is used instead.

-----

## Explicitly eviated semantics
These are emoji that have explicit shifts in intended communication from the Unicode Standard, but share the same codepoints as the originals.

### Currency emoji
Instead of representing banknotes for the specific 4 top world reserve currencies, they represent generic bank notes with generic designs intended to be somewhat evocative of the originals, but more open-ended towards any currency/locale.

| codepoint(s) (U+) | Unicode name | Mutant name |
| ---- | ---- | ---- |
| `1f4b4` | Banknote With Yen Sign | Yellow banknote |
| `1f4b5` | Banknote With Dollar Sign | Green banknote |
| `1f4b6` | Banknote With Euro Sign | Pink banknote |
| `1f4b7` | Banknote With Pound Sign | Purple banknote |

----

## Non-RGI (Recommended for General Interchange) symbols
These are symbols in the Unicode Standard that are not *Recommended for General Interchange as emoji*, but Mutant uses them as emoji nonetheless. These are combined with VS16 to ensure they display as emoji (because they normally display as text).

| codepoint(s) | Unicode name |
| ---- | ---- |
| `2640` `[VS16]` | Female Sign (♀) |
| `2642` `[VS16]` | Male Sign (♂ ) |
| `26a2` `[VS16]` | Doubled Female Sign (⚢) |
| `26a3` `[VS16]` | Doubled Male Sign (⚣) |
| `26a4` `[VS16]` | Interlocked Female and Male Sign (⚤) |
| `26a5` `[VS16]` | Male and Female Sign (⚥) |
| `26a6` `[VS16]` | Male with Stroke Sign (⚦) |
| `26a7` `[VS16]` | Male with Stroke and Male and Female Sign (⚧) |
| `26a8` `[VS16]` | Vertical Male with Stroke Sign (⚨) |
| `26b2` `[VS16]` | Neuter (⚲) |
| `007e` `[VS16]` | Tilde (~) |

----

## Emoji that are standard Unicode symbol but are intentionally not used
These are symbols in the Unicode standard that are RGI emoji, but the Mutant set explicitly has no current intention of using.

### Male/Female gendered sequences
Any encoding that results in a gendered person emoji (ie. a ZWJ featuring `2640` (female
symbol) or `2642` (male symbol)) do not exist in Mutant.

Instead, Mutant has only gender-neutral variants and has encoded male and female symbols as
independent symbols, which is not RGI (see earlier in this document). 

### Family sequences
Family ZWJs are also not being made in Mutant. Instead, users will be encouraged to simply put whatever emoji they want next to each other to imply a family group.

### Other characters and sequences
| Codepoint(s) (U+) | Unicode name | Notes |
| ---- | ---- | ---- |
| `a9` `[VS16]` | Copyright sign | |
| `ae` `[VS16]` | Registered sign | |
| `2122` `[VS16]` | Trade Mark | |
| `1f46e` | Police Officer (including all gender and skin tone modified variants) | |
| `1f482` | Guard (including all gender and skin tone modified variants) | |
| `1f693` | Police Car | |
| `1f694` | Oncoming Police Car | | 
| `1f6b9` | Men’s Room | |
| `1f6ba` | Women’s Room | |
| `1f6c2` | Passport Control | |
| `1f6c3` | Customs | |
| `1f3c7` | Horse Racing | | 
| `1f5fe` | Silhouette of Japan | |
