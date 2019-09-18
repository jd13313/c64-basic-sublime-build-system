# Note
This is intended for use on Linux, but could easily be re-worked for use on Windows. I'd think it should work fine as-is on macOS, but not able to verify that.

Also this was a quick/dirty solution I threw together out of frustration for lack of options for c64 BASIC dev/testing on linux. I will likely be updating this as time goes on to be more polished. But for now consider it to be "as is"

# Instructions

* Install [VICE](http://vice-emu.sourceforge.net/)
* build.sh should be good to go as-is if you're looking to convert .bas to .prg for the C64. [petcat](https://www.mankier.com/1/petcat) has some good docs so build.sh can easily be updated to output for a different platform if needed.
* In SublimeText, click "Tools" -> "Build System" -> "New Build System" and copy/paste the contents of c64-basic.sublime-build to it. Alternatively you can just move the file itself over to wherever Sublime keeps its build system config files.
* To use it, select "Tools" -> "Build System" and select "c64-basic". Then from an open .bas file you can use CTRL+B to convert the file to .prg and run it via VICE