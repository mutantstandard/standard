# Color Modifiers (CMs)

Unicode has a series of skin tone modifiers. In Mutant, these are called Color Modifiers - CMs for short.

To make an efficient and easy to remember shortcode encoding for these colours, Mutant uses a notation system inspired by professional drawing markers:

```
<letter indicating rough hue scale> <number indicating level of lightness>

R1 - dark red
R2 - red
R3 - light red
C1 - dark cyan
etc.
```

## Human CMs

These are the only CMs available in the **Mutant Core** bundle.

The original descriptions of these skin tones was based on the Fitzpatrick scale, which is biased and flawed. As a result, Mutant describes them in more generic terms.

Note that because of the way Mutant notes the lightness of a colour, the shortcodes run in the opposite order to the codepoints. When implementing these in an interface, follow the shortcode order.

| codepoint (U+) | Mutant shortcode | Name/Description |
| ---- | ---- | ---- |
| 1f3fb | h5 | light skin tone |
| 1f3fc | h4 | medium-light skin tone |
| 1f3fd | h3 | medium skin tone |
| 1f3fe | h2 | medium-dark skin tone |
| 1f3ff | h1 | dark skin tone |


## Arbitrary CMs

These CMs are only available in the **Mutant Form** bundle.

Most of these modifiers are based on a 13-point hue wheel that is not consistently spaced but perceptually spaced to compensate for the abundance of green in human vision.

2 more hue scales also exist in this system - brown (E) and grayscale (K).

| Mutant codepoint (U+) | Mutant shortcode | Name/Description |
| ---- | ---- | ---- |
| 101600 | r1 | dark red |
| 101601 | r2 | red |
| 101602 | r3 | light red |
| 101603 | d1 | dark red-orange |
| 101604 | d2 | red-orange |
| 101605 | d3 | light red-orange |
| 101606 | o1 | dark orange |
| 101607 | o2 | orange |
| 101608 | o3 | light orange |
| 101609 | y1 | dark yellow |
| 10160a | y2 | yellow |
| 10160b | y3 | light yellow |
| 10160c | l1 | dark lime |
| 10160d | l2 | lime |
| 10160e | l3 | light lime |
| 10160f | g1 | dark green |
| 101610 | g2 | green |
| 101611 | g3 | light green |
| 101612 | t1 | dark teal |
| 101613 | t2 | teal |
| 101614 | t3 | light teal |
| 101615 | c1 | dark cyan |
| 101616 | c2 | cyan |
| 101617 | c3 | light cyan |
| 101618 | s1 | dark sky blue |
| 101619 | s2 | sky blue |
| 10161a | s3 | light sky blue |
| 10161b | b1 | dark blue |
| 10161c | b2 | blue |
| 10161d | b3 | light blue |
| 10161e | v1 | dark violet |
| 10161f | v2 | violet |
| 101620 | v3 | light violet |
| 101621 | m1 | dark magenta |
| 101622 | m2 | magenta |
| 101623 | m3 | light magenta |
| 101624 | p1 | dark pink |
| 101625 | p2 | pink |
| 101626 | p3 | light pink |
| 101627 | e1 | dark brown |
| 101628 | e2 | brown |
| 101629 | e3 | light brown |
| 10162a | k1 | dark gray |
| 10162b | k2 | medium gray |
| 10162c | k3 | light gray |


## Default colour
In most other emoji sets, the default colour of unmodified emoji is yellow, however, because of the white-coded nature of yellow, Mutant opts for a medium grey, the same shade as K2.

