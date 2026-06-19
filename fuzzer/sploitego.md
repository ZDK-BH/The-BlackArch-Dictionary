# sploitego

**Category:** `fuzzer`  
**Version in source list:** `153.d9568dc`  
**Package name:** `sploitego`

## What it does

Maltego Penetration Testing Transforms.

## What it can be used for

Feeding unexpected input to owned software/protocols to find crashes, parsing bugs, and robustness issues.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sploitego
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sploitego | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sploitego --help
sploitego -h
man sploitego
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run fuzzers against local test programs or isolated lab services.
2. Start with small corpora and low intensity.
3. Save crashing inputs and reproduce them manually.
4. Fix the bug, add regression tests, and rerun.

## Example commands

```bash
sploitego --help
```

```bash
sploitego -h
```

```bash
# Local fuzzing target pattern:
sploitego ./test-program
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
