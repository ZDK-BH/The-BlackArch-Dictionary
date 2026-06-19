# rww-attack

**Category:** `webapp`  
**Version in source list:** `0.9.2`  
**Package name:** `rww-attack`

## What it does

Performs a dictionary attack against a live Microsoft Windows Small Business Server.

## What it can be used for

Testing your own web apps, APIs, CMS instances, input validation, authentication flows, and exposed web attack surface.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed rww-attack
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql rww-attack | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
rww-attack --help
rww-attack -h
man rww-attack
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use your own app, a local lab such as DVWA/Juice Shop, or a written-scope assessment.
2. Start with crawling/fingerprinting, then move to targeted checks.
3. Keep request rates reasonable and avoid destructive options.
4. Validate findings manually and fix the code/configuration.

## Example commands

```bash
rww-attack --help
```

```bash
rww-attack -h
```

```bash
# Owned lab app pattern:
rww-attack http://localhost:8080
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
