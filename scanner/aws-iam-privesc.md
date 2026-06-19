# aws-iam-privesc

**Category:** `scanner`  
**Version in source list:** `11.2983efd`  
**Package name:** `aws-iam-privesc`

## What it does

AWS IAM policy scanner that helps determine where privilege escalation can be achieved.

## What it can be used for

Finding exposed services, misconfigurations, versions, certificates, web paths, and vulnerability indicators.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed aws-iam-privesc
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql aws-iam-privesc | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
aws-iam-privesc --help
aws-iam-privesc -h
man aws-iam-privesc
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Scan only approved IP ranges/domains.
2. Start with low-rate or passive scans if available.
3. Export results and verify findings manually.
4. Fix or report validated issues with clear evidence.

## Example commands

```bash
aws-iam-privesc --help
```

```bash
aws-iam-privesc -h
```

```bash
# Owned lab host pattern:
aws-iam-privesc 192.0.2.10
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
