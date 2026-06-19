# sslstrip

**Category:** `proxy`  
**Version in source list:** `0.9`  
**Package name:** `sslstrip`

## What it does

Python tool to hijack HTTPS connections during a MITM attack.

## What it can be used for

Intercepting, forwarding, replaying, or debugging traffic in an approved test environment.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sslstrip
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sslstrip | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sslstrip --help
sslstrip -h
man sslstrip
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run the proxy locally and bind only to localhost unless you know why you need exposure.
2. Use a lab browser profile for proxy certificates and traffic capture.
3. Intercept only traffic you own or are authorized to inspect.
4. Clear captures that contain secrets when finished.

## Example commands

```bash
sslstrip --help
```

```bash
sslstrip -h
```

```bash
# Local proxy prep:
mkdir -p proxy-captures
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
