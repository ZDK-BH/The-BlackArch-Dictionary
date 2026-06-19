# powerfuzzer

**Category:** `fuzzer`  
**Version in source list:** `1_beta`  
**Package name:** `powerfuzzer`

## What it does

Powerfuzzer is a highly automated web fuzzer based on many other Open Source fuzzers available (incl. cfuzzer, fuzzled, fuzzer.pl, jbrofuzz, webscarab, wapiti, Socket Fuzzer). It can detect XSS, Injections (SQL, LDAP, commands, code, XPATH) and others.

## What it can be used for

Feeding unexpected input to owned software/protocols to find crashes, parsing bugs, and robustness issues.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed powerfuzzer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql powerfuzzer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
powerfuzzer --help
powerfuzzer -h
man powerfuzzer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run fuzzers against local test programs or isolated lab services.
2. Start with small corpora and low intensity.
3. Save crashing inputs and reproduce them manually.
4. Fix the bug, add regression tests, and rerun.

## Example commands

```bash
powerfuzzer --help
```

```bash
powerfuzzer -h
```

```bash
# Local fuzzing target pattern:
powerfuzzer ./test-program
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
