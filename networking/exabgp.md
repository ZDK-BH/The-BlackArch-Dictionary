# exabgp

**Category:** `networking`  
**Version in source list:** `4.0.2.r2465.g68ce530`  
**Package name:** `exabgp`

## What it does

The BGP swiss army knife of networking.

## What it can be used for

Protocol testing, service diagnostics, routing/tunneling labs, packet handling, and network behavior analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed exabgp
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql exabgp | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
exabgp --help
exabgp -h
man exabgp
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Identify your interface and lab network first.
2. Use read-only/listen modes where available.
3. Keep tests inside owned or authorized networks.
4. Save packet captures/logs for review.

## Example commands

```bash
exabgp --help
```

```bash
exabgp -h
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
