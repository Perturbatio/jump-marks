# jump-marks
My custom jump marks implementation based on that by @jeroenjanssens and things I've found on the net.

## Installation:
checkout the repo
add a source directive to your `.bash_profile`, `.bashrc` or wherever else you prefer.

```
source /path/to/.jump_marks file
```
and re-source (type `source ~/.bash_profile`) or logout and back into your terminal

## OSX/MacOS users
There's an osx `marks` function in the file you'll need to uncommment that and comment out the marks function
then rename the osx `marks` function to `marks`

## Usage
cd to a dir and type `mark <alias>` to mark the directory using the given alias
type `marks` to list your existing marks
`jump <alias>` to jump (change dir) to the given mark
`unmark <alias>` to remove the mark

`jump` and `unmark` both have command completion i.e. type `jump a<tab>` to get all marks beginning with `a`

if you use `jump` or `unmark` with no parameters you'll be given a choice of mark aliases to choose from

## TODO:
automatic OS detection to switch the marks function depending on whether it's OSX or not
