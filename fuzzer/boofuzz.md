# boofuzz

**Category:** `fuzzer`  
**Version in source list:** `v0.4.2.r40.g295f329`  
**Package name:** `boofuzz`

## What it does

No description provided in the source list.

## What it can be used for

Feeding unexpected input to owned software/protocols to find crashes, parsing bugs, and robustness issues.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed boofuzz
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql boofuzz | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
boofuzz --help
boofuzz -h
man boofuzz
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run fuzzers against local test programs or isolated lab services.
2. Start with small corpora and low intensity.
3. Save crashing inputs and reproduce them manually.
4. Fix the bug, add regression tests, and rerun.

## Example commands

```bash
boofuzz --help
```

```bash
boofuzz -h
```

```bash
# Local fuzzing target pattern:
boofuzz ./test-program
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
