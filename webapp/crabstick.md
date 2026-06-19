# crabstick

**Category:** `webapp`  
**Version in source list:** `47.bb7827f`  
**Package name:** `crabstick`

## What it does

Automatic remote/local file inclusion vulnerability analysis and exploit tool.

## What it can be used for

Testing your own web apps, APIs, CMS instances, input validation, authentication flows, and exposed web attack surface.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed crabstick
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql crabstick | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
crabstick --help
crabstick -h
man crabstick
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use your own app, a local lab such as DVWA/Juice Shop, or a written-scope assessment.
2. Start with crawling/fingerprinting, then move to targeted checks.
3. Keep request rates reasonable and avoid destructive options.
4. Validate findings manually and fix the code/configuration.

## Example commands

```bash
crabstick --help
```

```bash
crabstick -h
```

```bash
# Owned lab app pattern:
crabstick http://localhost:8080
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
