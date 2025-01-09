
# HW2 Report

* TODO: Put name here

* TODO: Go through each of the statements labeled "TODO". Complete the instructions, then remove the section.

## Tools Installed

* TODO: If on Windows, install WSL2: <https://learn.microsoft.com/en-us/windows/wsl/install>.

* TODO: If on Linux or WSL2, run

```bash
sudo apt install cmake pandoc texlive clang-format
```

* TODO: If on MacOS, install brew: <https://brew.sh/>. Then run

```bash
brew install cmake pandoc librsvg python3 basictex clang-format
```

* TODO: Include a screenshot of your terminal after running:

```bash
cmake --version
pandoc --version
pdflatex --version
clang-format --version
```

## C++ Source Files

* TODO: Create a C++ program that replicates the behavior of `echo`. There is no need to add all the functionality that `echo`. Simply print back all the arguments found in `argv`, separated with spaces.

```cpp
// Paste in your completed C++ file here
```

* TODO: Add C++ source file to `"CMakeLists.txt"`

## Compiling

* TODO: Include a screenshot of yourself performing the following:

1. Create and `cd` into a build directory.
2. Run `cmake` on the directory where the `"CMakeLists.txt"` file exists.
3. Run `make`
4. Run `source /path/to/example.sh`

## Custom Makefile

* TODO: Create a Makefile in the project root directoy with the following targets: `format`, `verify_format`, `report.pdf`.

* TODO: Calling `make format` should apply `clang-format` to all your source files, inplace, with style set to "Google". `clang-format` documentation: <https://clang.llvm.org/docs/ClangFormat.html>.

* TODO: Calling `make verify_format` should run the same `clang-format` command as `make format`, except with the added options `--dry-run --Werror`.

* TODO: Calling `make report.pdf` should run the following:

```bash
pandoc --from=markdown \
       --to=latex \
       --toc \
       -o report.pdf \
       report.md \
       --shift-heading-level-by -1 \
       --number-sections
```

* TODO: For `make report.pdf`, use the constructs `$@` and `$^` in the `pandoc` command to replace the target and dependencies.

```makefile
# Paste in your completed Makefile here
```

Include screenshot of your terminal after running:

```bash
make format
make verify_format
make report.pdf
```
