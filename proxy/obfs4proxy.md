# obfs4proxy

**Category:** `proxy`  
**Version in source list:** `0.0.13`  
**Package name:** `obfs4proxy`

## What it does

A pluggable transport proxy written in Go.

## What it can be used for

Intercepting, forwarding, replaying, or debugging traffic in an approved test environment.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed obfs4proxy
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql obfs4proxy | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
obfs4proxy --help
obfs4proxy -h
man obfs4proxy
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run the proxy locally and bind only to localhost unless you know why you need exposure.
2. Use a lab browser profile for proxy certificates and traffic capture.
3. Intercept only traffic you own or are authorized to inspect.
4. Clear captures that contain secrets when finished.

## Example commands

```bash
obfs4proxy --help
```

```bash
obfs4proxy -h
```

```bash
# Local proxy prep:
mkdir -p proxy-captures
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
