# Mutant encoding

**(This repository is incomplete. I am slowly working on migrating old technical documentation to here!)**

This document outlines the encoding mechanics of various symbols within Mutant emoji, and what makes them differ (if any) from Unicode. This is aimed at developers wishing to use Mutant emoji in their apps as well as emoji designers who wish to use the semantic structure of Mutant for their own designs.

These documents are licensed MIT.

## General
- [Terms](terms.md)

## Bundles
- [Bundles overview](bundles.md)

### Mutant Core
The core set which other bundles can potentially into.
- [Unicode deviations](core/unicode_deviations.md)
- [Color modifiers](core/cm.md)

### Communication extensions
#### Mutant Spectrum
The bundle that focuses on symbols and expressions for the queer community.
- [Non-standard ZWJs](spectrum/non_standard_zwj.md)

#### Mutant Form
Modifiers, symbols and expressions catering to furries and those who use non-human representations of themselves.
- [Color modifiers](form/cm.md)
- [Morph modifiers](form/mm.md)
- [Combining Color and Morph modifiers](form/cm_and_mm.md)

## PUA (Private Use Area)
What PUA encodings Mutant uses.
- [Overview](pua/overview.md)
- [10160x - 10164x Color Modifiers](pua/10160x_10164x_cm.md)
