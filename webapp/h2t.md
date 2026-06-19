# h2t

**Category:** `webapp`  
**Version in source list:** `38.56e1447`  
**Package name:** `h2t`

## What it does

Scans a website and suggests security headers to apply.

## What it can be used for

Testing your own web apps, APIs, CMS instances, input validation, authentication flows, and exposed web attack surface.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed h2t
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql h2t | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
h2t --help
h2t -h
man h2t
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use your own app, a local lab such as DVWA/Juice Shop, or a written-scope assessment.
2. Start with crawling/fingerprinting, then move to targeted checks.
3. Keep request rates reasonable and avoid destructive options.
4. Validate findings manually and fix the code/configuration.

## Example commands

```bash
h2t --help
```

```bash
h2t -h
```

```bash
# Owned lab app pattern:
h2t http://localhost:8080
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
