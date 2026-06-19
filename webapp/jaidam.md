# jaidam

**Category:** `webapp`  
**Version in source list:** `18.15e0fec`  
**Package name:** `jaidam`

## What it does

Penetration testing tool that would take as input a list of domain names, scan them, determine if wordpress or joomla platform was used and finally check them automatically, for web vulnerabilities using two well-known open source tools,

## What it can be used for

Testing your own web apps, APIs, CMS instances, input validation, authentication flows, and exposed web attack surface.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed jaidam
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql jaidam | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
jaidam --help
jaidam -h
man jaidam
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use your own app, a local lab such as DVWA/Juice Shop, or a written-scope assessment.
2. Start with crawling/fingerprinting, then move to targeted checks.
3. Keep request rates reasonable and avoid destructive options.
4. Validate findings manually and fix the code/configuration.

## Example commands

```bash
jaidam --help
```

```bash
jaidam -h
```

```bash
# Owned lab app pattern:
jaidam http://localhost:8080
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
