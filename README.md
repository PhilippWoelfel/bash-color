# bash-color
Simple bash shell script that makes it easy to color and format output text

Imported from https://code.google.com/archive/p/ansi-color/

## Usage
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

## Examples

```
echo "$(color ul)Underlined text$(color off)"

echo "Make $(color rv)this$(color nm) reverse video text"

echo "$(color white blue) White text on a blue background $(color)"

echo "$(color ltyellow green) lt prefix on the yellow text text $(color off)"

echo "$(color bold red yellow blink) Blinking bold red text on a yellow background $(color)"
```

Note that results may vary with these standard ANSI escape sequences because of the different configurations of terminal emulators.

## Installation
* As root:
  Clone the repository and install with `make install`.
  To uninstall run `make uninstall`.
  
* As non-root:
  copy file [color]() to a directory in $PATH

## Credit
The shell script is taken from https://code.google.com/archive/p/ansi-color/
