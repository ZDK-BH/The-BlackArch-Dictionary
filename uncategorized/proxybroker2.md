# proxybroker2

**Category:** `uncategorized`  
**Version in source list:** `662.44742c6`  
**Package name:** `proxybroker2`

## What it does

Proxy [Finder Checker

## What it can be used for

General security-related tasks; exact purpose depends on the tool.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed proxybroker2
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql proxybroker2 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
proxybroker2 --help
proxybroker2 -h
man proxybroker2
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Install only if you know why you need it.
2. Inspect package files and documentation.
3. Run help/version commands first.
4. Use a lab VM for unknown or unfamiliar tools.

## Example commands

```bash
proxybroker2 --help
```

```bash
proxybroker2 -h
```

```bash
pacman -Ql proxybroker2 | sed -n "1,120p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
