# apkleaks

**Category:** `mobile`  
**Version in source list:** `v2.6.3.r2.gdd5271a`  
**Package name:** `apkleaks`

## What it does

Scanning APK file for URIs, endpoints & secrets.

## What it can be used for

Android/iOS app review, APK extraction, mobile forensics, and mobile security testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed apkleaks
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql apkleaks | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
apkleaks --help
apkleaks -h
man apkleaks
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use apps/devices you own or have permission to test.
2. Copy APKs or backups into a lab folder.
3. Start with static analysis before runtime instrumentation.
4. Document permissions, endpoints, secrets, and insecure storage.

## Example commands

```bash
apkleaks --help
```

```bash
apkleaks -h
```

```bash
# Local APK pattern:
apkleaks ./app.apk
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
