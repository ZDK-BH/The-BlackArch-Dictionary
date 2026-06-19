# fuzzball2

**Category:** `fuzzer`  
**Version in source list:** `0.7`  
**Package name:** `fuzzball2`

## What it does

A fuzzer for TCP and IP protocol options. It sends a bunch of more or less bogus packets to the target.

## What it can be used for

Feeding unexpected input to owned software/protocols to find crashes, parsing bugs, and robustness issues.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed fuzzball2
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql fuzzball2 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
fuzzball2 --help
fuzzball2 -h
man fuzzball2
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run fuzzers against local test programs or isolated lab services.
2. Start with small corpora and low intensity.
3. Save crashing inputs and reproduce them manually.
4. Fix the bug, add regression tests, and rerun.

## Example commands

```bash
fuzzball2 --help
```

```bash
fuzzball2 -h
```

```bash
# Local fuzzing target pattern:
fuzzball2 ./test-program
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
