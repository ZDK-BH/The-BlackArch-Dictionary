# cms-explorer

**Category:** `fingerprint`  
**Version in source list:** `15.23b58cd`  
**Package name:** `cms-explorer`

## What it does

Designed to reveal the specific modules, plugins, components and themes that various cms driven websites are running.

## What it can be used for

Identifying services, frameworks, versions, CMSs, applications, or technologies.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed cms-explorer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql cms-explorer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
cms-explorer --help
cms-explorer -h
man cms-explorer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Start with passive or low-rate fingerprinting.
2. Compare output with headers, certificates, and application behavior.
3. Confirm version findings manually.
4. Use results to plan patching or authorized testing.

## Example commands

```bash
cms-explorer --help
```

```bash
cms-explorer -h
```

```bash
# Owned lab target pattern:
cms-explorer https://example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
