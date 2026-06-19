# sshfuzz

**Category:** `fuzzer`  
**Version in source list:** `1.0`  
**Package name:** `sshfuzz`

## What it does

A SSH Fuzzing utility written in Perl that uses Net::SSH2.

## What it can be used for

Feeding unexpected input to owned software/protocols to find crashes, parsing bugs, and robustness issues.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sshfuzz
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sshfuzz | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sshfuzz --help
sshfuzz -h
man sshfuzz
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run fuzzers against local test programs or isolated lab services.
2. Start with small corpora and low intensity.
3. Save crashing inputs and reproduce them manually.
4. Fix the bug, add regression tests, and rerun.

## Example commands

```bash
sshfuzz --help
```

```bash
sshfuzz -h
```

```bash
# Local fuzzing target pattern:
sshfuzz ./test-program
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
