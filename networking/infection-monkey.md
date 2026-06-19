# infection-monkey

**Category:** `networking`  
**Version in source list:** `v2.2.0.r3599.ga55fc8d`  
**Package name:** `infection-monkey`

## What it does

Automated security testing tool for networks.

## What it can be used for

Protocol testing, service diagnostics, routing/tunneling labs, packet handling, and network behavior analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed infection-monkey
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql infection-monkey | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
infection-monkey --help
infection-monkey -h
man infection-monkey
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Identify your interface and lab network first.
2. Use read-only/listen modes where available.
3. Keep tests inside owned or authorized networks.
4. Save packet captures/logs for review.

## Example commands

```bash
infection-monkey --help
```

```bash
infection-monkey -h
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
