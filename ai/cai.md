# cai

**Category:** `ai`  
**Version in source list:** `0.5.9.r26.g1c79507`  
**Package name:** `cai`

## What it does

The framework for AI Security.

## What it can be used for

Testing AI/ML systems, model robustness, adversarial examples, and AI infrastructure exposure.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed cai
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql cai | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
cai --help
cai -h
man cai
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Create a local test project, model endpoint, or intentionally vulnerable AI lab service.
2. Read the tool help and documentation before pointing it at any model/server.
3. Run low-impact checks first, save the output, then manually verify findings.
4. Use findings to harden model servers, exposed dashboards, prompts, datasets, and API keys.

## Example commands

```bash
cai --help
```

```bash
cai -h
```

```bash
# Lab-only pattern after reading help:
cai <lab-model-or-local-endpoint>
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
