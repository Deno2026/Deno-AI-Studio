# Install Deno AI Studio on Windows

This repository provides the Windows installer for **Deno AI Studio**.

It is **not** a Deno runtime project. Do not install Deno, do not clone this repository, and do not build from source.

## Correct install order

1. Install **Docker Desktop for Windows - x86_64**.
2. Open Docker Desktop once.
3. Keep **Use the WSL 2 based engine** enabled.
4. If Windows or Docker says WSL is missing, open **PowerShell as Administrator** and run:

```powershell
wsl --install --no-distribution
```

5. Restart Windows if asked.
6. Download and run the current **Deno AI Studio Setup `.exe`** from the README.
7. Open Deno AI Studio.
8. Use **Runtime Center** to check Docker, GPU, disk, and model readiness.

## Important

Ubuntu is optional. Install Ubuntu only if you personally want a Linux terminal.

Normal Deno AI Studio use on Windows relies on Docker Desktop's WSL 2 backend, not a mandatory separate Ubuntu account.

If an AI assistant mentions an older installer version, ignore the old version and use the current download link in the README.
