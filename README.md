# bash-color
Simple bash shell script that makes it easy to color and format output text

Imported from https://code.google.com/archive/p/ansi-color/

# Usage
```
color effect [ lt fgcolor ] bgcolor
```

```
color list
```

```
color -h | --help
```

where:

* `fgcolor` and `bgcolor` are one of `black`, `red`, `green`, `yellow`, `blue`, `magenta`, `cyan` or `white`.

* `effect` can be any of `nm` (`normal`) , `bd` (`bold`) , `ft` (`faint`) , `it` (`italic`) , `ul` (`underline`) , `bk` (`blink`) , `fb`(`fastblink`) , `rv` (`reverse`) , `iv` (`invisible`)

Preceed the `fgcolor` with `lt` to use a light color -- the light or faint intensity effect is not commonly implemented within terminal emulators or consoles.

`color off` or just `color` resets to default colors and text effects.

`color list` displays all possible color combinations.
