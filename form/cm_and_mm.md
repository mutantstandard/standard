
# Combining MMs and CMs


## Basic formula

MMs always come before CMs if they exist - both in the shortcode and the codepoint.

```
[ character to be modified ] + [ MM ]
character_mm

[ character to be modified ] + [ CM ]
character_cm

[ character to be modified ] + [ MM ] + [ CM ]
character_mm_cm
```

## Basic examples

thumbs up (humanoid hand)
```
1f44d fe0f
thumbs_up_hmn
```
thumbs up (paw hand)
```
1f44d fe0f 101650
thumbs_up_paw
```

thumbs up (claw hand)
```
1f44d fe0f 101651
thumbs_up_clw
```

thumbs up (light skin tone)
```
1f44d fe0f 1f3fb
thumbs_up_h5
```

thumbs up (dark blue)
```
1f44d fe0f 10161b
thumbs_up_hmn_b1
```

thumbs up (claw hand, violet)
```
1f44d fe0f 101651 10161f
thumbs_up_clw_v2
```

ear (dark skin tone)
```
1f442 fe0f 1f3ff
ear_h1
```

ear (yellow-green colour)
```
1f442 fe0f 10160d
ear_l2
```


## Disallowed combinations

As the name implies, Arbitrary CMs are intended to work with any Morph Modifier. For cultural reasons, Human CMs are limited to only human hand appearances. For users seeking a brown colour on a non-human morph, they can use the E series of colours instead.

| CM group | Morph usages |
| ---- | ---- |
| Human (Hx) | Human only (hmn) |
| All other CMs | All |
