# packet-o-matic

**Category:** `networking`  
**Version in source list:** `351`  
**Package name:** `packet-o-matic`

## What it does

A real time packet processor. Reads the packet from an input module, match the packet using rules and connection tracking information and then send it to a target module.

## What it can be used for

Protocol testing, service diagnostics, routing/tunneling labs, packet handling, and network behavior analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed packet-o-matic
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql packet-o-matic | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
packet-o-matic --help
packet-o-matic -h
man packet-o-matic
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Identify your interface and lab network first.
2. Use read-only/listen modes where available.
3. Keep tests inside owned or authorized networks.
4. Save packet captures/logs for review.

## Example commands

```bash
packet-o-matic --help
```

```bash
packet-o-matic -h
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
