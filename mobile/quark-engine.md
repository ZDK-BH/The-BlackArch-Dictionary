# quark-engine

**Category:** `mobile`  
**Version in source list:** `21.6.2`  
**Package name:** `quark-engine`

## What it does

An Obfuscation-Neglect Android Malware Scoring System.

## What it can be used for

Android/iOS app review, APK extraction, mobile forensics, and mobile security testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed quark-engine
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql quark-engine | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
quark-engine --help
quark-engine -h
man quark-engine
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use apps/devices you own or have permission to test.
2. Copy APKs or backups into a lab folder.
3. Start with static analysis before runtime instrumentation.
4. Document permissions, endpoints, secrets, and insecure storage.

## Example commands

```bash
quark-engine --help
```

```bash
quark-engine -h
```

```bash
# Local APK pattern:
quark-engine ./app.apk
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
