# chameleon

**Category:** `networking`  
**Version in source list:** `29.4414287`  
**Package name:** `chameleon`

## What it does

A tool for evading Proxy categorisation.

## What it can be used for

Protocol testing, service diagnostics, routing/tunneling labs, packet handling, and network behavior analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed chameleon
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql chameleon | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
chameleon --help
chameleon -h
man chameleon
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Identify your interface and lab network first.
2. Use read-only/listen modes where available.
3. Keep tests inside owned or authorized networks.
4. Save packet captures/logs for review.

## Example commands

```bash
chameleon --help
```

```bash
chameleon -h
```

```bash
ip addr
```

```bash
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
