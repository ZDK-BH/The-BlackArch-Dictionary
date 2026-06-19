# semgrep

**Category:** `code-audit`  
**Version in source list:** `1.164.0`  
**Package name:** `semgrep`

## What it does

Lightweight static analysis for many languages.

## What it can be used for

Finding insecure patterns in code, dependencies, infrastructure-as-code, and application logic.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed semgrep
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql semgrep | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
semgrep --help
semgrep -h
man semgrep
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run it against your own repository or a deliberately vulnerable training repo.
2. Start with default scan settings.
3. Review findings manually to remove false positives.
4. Fix issues, commit changes, and rerun the scan.

## Example commands

```bash
semgrep --help
```

```bash
semgrep -h
```

```bash
# Common local repo pattern:
semgrep ./project
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
