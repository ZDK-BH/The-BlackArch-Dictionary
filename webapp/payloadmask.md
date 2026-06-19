# payloadmask

**Category:** `webapp`  
**Version in source list:** `17.58e0525`  
**Package name:** `payloadmask`

## What it does

Web Payload list editor to use techniques to try bypass web application firewall.

## What it can be used for

Testing your own web apps, APIs, CMS instances, input validation, authentication flows, and exposed web attack surface.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed payloadmask
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql payloadmask | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
payloadmask --help
payloadmask -h
man payloadmask
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use your own app, a local lab such as DVWA/Juice Shop, or a written-scope assessment.
2. Start with crawling/fingerprinting, then move to targeted checks.
3. Keep request rates reasonable and avoid destructive options.
4. Validate findings manually and fix the code/configuration.

## Example commands

```bash
payloadmask --help
```

```bash
payloadmask -h
```

```bash
# Owned lab app pattern:
payloadmask http://localhost:8080
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
