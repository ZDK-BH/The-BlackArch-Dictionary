# mitm-relay

**Category:** `proxy`  
**Version in source list:** `41.2d168b2`  
**Package name:** `mitm-relay`

## What it does

Hackish way to intercept and modify non-HTTP protocols through Burp & others.

## What it can be used for

Intercepting, forwarding, replaying, or debugging traffic in an approved test environment.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed mitm-relay
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql mitm-relay | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
mitm-relay --help
mitm-relay -h
man mitm-relay
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run the proxy locally and bind only to localhost unless you know why you need exposure.
2. Use a lab browser profile for proxy certificates and traffic capture.
3. Intercept only traffic you own or are authorized to inspect.
4. Clear captures that contain secrets when finished.

## Example commands

```bash
mitm-relay --help
```

```bash
mitm-relay -h
```

```bash
# Local proxy prep:
mkdir -p proxy-captures
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
