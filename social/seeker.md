# seeker

**Category:** `social`  
**Version in source list:** `379.abbbf80`  
**Package name:** `seeker`

## What it does

Accurately Locate People using Social Engineering.

## What it can be used for

Public-information review, awareness training, and phishing-defense education.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed seeker
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql seeker | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
seeker --help
seeker -h
man seeker
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only test accounts, training domains, or approved awareness programs.
2. Do not collect real credentials or personal data without a formal authorization process.
3. Focus on education, detection, and reporting workflows.
4. Keep logs sanitized and delete sensitive test data after the exercise.

## Example commands

```bash
seeker --help
```

```bash
seeker -h
```

```bash
# Training-only prep:
mkdir -p awareness-lab
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
