# easyfuzzer

**Category:** `fuzzer`  
**Version in source list:** `3.6`  
**Package name:** `easyfuzzer`

## What it does

A flexible fuzzer, not only for web, has a CSV output for efficient output analysis (platform independent).

## What it can be used for

Feeding unexpected input to owned software/protocols to find crashes, parsing bugs, and robustness issues.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed easyfuzzer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql easyfuzzer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
easyfuzzer --help
easyfuzzer -h
man easyfuzzer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run fuzzers against local test programs or isolated lab services.
2. Start with small corpora and low intensity.
3. Save crashing inputs and reproduce them manually.
4. Fix the bug, add regression tests, and rerun.

## Example commands

```bash
easyfuzzer --help
```

```bash
easyfuzzer -h
```

```bash
# Local fuzzing target pattern:
easyfuzzer ./test-program
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
