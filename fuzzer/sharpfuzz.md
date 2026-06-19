# sharpfuzz

**Category:** `fuzzer`  
**Version in source list:** `v2.2.0.r7.gd300db0`  
**Package name:** `sharpfuzz`

## What it does

AFL-based fuzz testing for .NET.

## What it can be used for

Feeding unexpected input to owned software/protocols to find crashes, parsing bugs, and robustness issues.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sharpfuzz
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sharpfuzz | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sharpfuzz --help
sharpfuzz -h
man sharpfuzz
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run fuzzers against local test programs or isolated lab services.
2. Start with small corpora and low intensity.
3. Save crashing inputs and reproduce them manually.
4. Fix the bug, add regression tests, and rerun.

## Example commands

```bash
sharpfuzz --help
```

```bash
sharpfuzz -h
```

```bash
# Local fuzzing target pattern:
sharpfuzz ./test-program
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
