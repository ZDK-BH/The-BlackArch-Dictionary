# dontgo403

**Category:** `webapp`  
**Version in source list:** `v2.0.1.r0.g40e7b6c`  
**Package name:** `dontgo403`

## What it does

Tool to bypass 40X response codes..

## What it can be used for

Testing your own web apps, APIs, CMS instances, input validation, authentication flows, and exposed web attack surface.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed dontgo403
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql dontgo403 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
dontgo403 --help
dontgo403 -h
man dontgo403
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use your own app, a local lab such as DVWA/Juice Shop, or a written-scope assessment.
2. Start with crawling/fingerprinting, then move to targeted checks.
3. Keep request rates reasonable and avoid destructive options.
4. Validate findings manually and fix the code/configuration.

## Example commands

```bash
dontgo403 --help
```

```bash
dontgo403 -h
```

```bash
# Owned lab app pattern:
dontgo403 http://localhost:8080
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
