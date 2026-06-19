# hexorbase

**Category:** `fuzzer`  
**Version in source list:** `7`  
**Package name:** `hexorbase`

## What it does

A database application designed for administering and auditing multiple database servers simultaneously from a centralized location. It is capable of performing SQL queries and bruteforce attacks against common database servers (MySQL, SQLite, Microsoft SQL Server, Oracle, PostgreSQL).

## What it can be used for

Feeding unexpected input to owned software/protocols to find crashes, parsing bugs, and robustness issues.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed hexorbase
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql hexorbase | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
hexorbase --help
hexorbase -h
man hexorbase
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run fuzzers against local test programs or isolated lab services.
2. Start with small corpora and low intensity.
3. Save crashing inputs and reproduce them manually.
4. Fix the bug, add regression tests, and rerun.

## Example commands

```bash
hexorbase --help
```

```bash
hexorbase -h
```

```bash
# Local fuzzing target pattern:
hexorbase ./test-program
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
