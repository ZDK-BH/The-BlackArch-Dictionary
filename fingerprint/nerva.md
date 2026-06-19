# nerva

**Category:** `fingerprint`  
**Version in source list:** `v1.18.0.r0.gf80de47`  
**Package name:** `nerva`

## What it does

Fast service fingerprinting CLI for 170+ protocols (TCP/UDP/SCTP).

## What it can be used for

Identifying services, frameworks, versions, CMSs, applications, or technologies.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed nerva
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql nerva | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
nerva --help
nerva -h
man nerva
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Start with passive or low-rate fingerprinting.
2. Compare output with headers, certificates, and application behavior.
3. Confirm version findings manually.
4. Use results to plan patching or authorized testing.

## Example commands

```bash
nerva --help
```

```bash
nerva -h
```

```bash
# Owned lab target pattern:
nerva https://example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
