# php-findsock-shell

**Category:** `webapp`  
**Version in source list:** `2.b8a984f`  
**Package name:** `php-findsock-shell`

## What it does

A Findsock Shell implementation in PHP + C.

## What it can be used for

Testing your own web apps, APIs, CMS instances, input validation, authentication flows, and exposed web attack surface.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed php-findsock-shell
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql php-findsock-shell | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
php-findsock-shell --help
php-findsock-shell -h
man php-findsock-shell
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use your own app, a local lab such as DVWA/Juice Shop, or a written-scope assessment.
2. Start with crawling/fingerprinting, then move to targeted checks.
3. Keep request rates reasonable and avoid destructive options.
4. Validate findings manually and fix the code/configuration.

## Example commands

```bash
php-findsock-shell --help
```

```bash
php-findsock-shell -h
```

```bash
# Owned lab app pattern:
php-findsock-shell http://localhost:8080
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
