# cntlm

**Category:** `proxy`  
**Version in source list:** `4.b35d55c`  
**Package name:** `cntlm`

## What it does

An NTLM, NTLM2SR, and NTLMv2 authenticating HTTP proxy.

## What it can be used for

Intercepting, forwarding, replaying, or debugging traffic in an approved test environment.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed cntlm
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql cntlm | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
cntlm --help
cntlm -h
man cntlm
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run the proxy locally and bind only to localhost unless you know why you need exposure.
2. Use a lab browser profile for proxy certificates and traffic capture.
3. Intercept only traffic you own or are authorized to inspect.
4. Clear captures that contain secrets when finished.

## Example commands

```bash
cntlm --help
```

```bash
cntlm -h
```

```bash
# Local proxy prep:
mkdir -p proxy-captures
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
