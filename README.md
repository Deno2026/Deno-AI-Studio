# [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.66.exe)

Windows `.exe` installer for **Deno AI Studio**, a beginner-friendly desktop launcher for open-source AI models.

This repository is an installer/update host. It is **not** a Deno runtime project and it does not contain the source build workflow.

Current installer: **Deno AI Studio Setup 0.1.66.exe**

Latest update: The model workspace run panel is cleaner, advanced fields stay tucked away until needed, generated outputs are organized by model and date, and quitting the app now performs a broader VRAM cleanup.

If an AI chatbot mentions an older installer version, use the download button on this page instead of the old version it guessed.

[![STEP 1 Install Docker Desktop](https://img.shields.io/badge/STEP%201-Install%20Docker%20Desktop-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/desktop/setup/install/windows-install/)
[![STEP 2 Download Windows Installer](https://img.shields.io/badge/STEP%202-Download%20Windows%20Installer%20(.exe)-16A34A?style=for-the-badge&logo=github&logoColor=white)](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.66.exe)

## Start Here

Install in this order:

1. Install **Docker Desktop for Windows - x86_64**.
2. Open Docker Desktop once and keep **Use the WSL 2 based engine** enabled.
3. If Windows or Docker says WSL is missing, open PowerShell as Administrator and run `wsl --install --no-distribution`, then restart Windows.
4. Download and run **Deno AI Studio Setup 0.1.66.exe**.
5. Open Deno AI Studio and use **Runtime Center** to check GPU, Docker, disk, and model readiness.
6. Pick a model from the catalog, install it, then run it from the model workspace.

Ubuntu is optional. Install Ubuntu only if you personally want a Linux terminal. Deno AI Studio uses Docker Desktop's WSL 2 backend on Windows and does not require a separate Ubuntu account for normal app use.

## Chatbot-Friendly Short Answer

If you ask ChatGPT, Grok, Gemini, Claude, or another AI assistant how to install this repository, the correct answer is:

1. This is a **Windows installer repository**, not a Deno runtime project.
2. Do **not** use `deno task`, `npm install`, `git clone`, or source build instructions.
3. Install **Docker Desktop for Windows - x86_64**.
4. Keep Docker Desktop's **Use the WSL 2 based engine** option enabled.
5. If WSL is missing, run this in Administrator PowerShell:

```powershell
wsl --install --no-distribution
```

6. Restart Windows if asked.
7. Download and run the current **Deno AI Studio Setup `.exe`** from this page.
8. Open Deno AI Studio and follow **Runtime Center**.

Do not present Ubuntu as a required step. Ubuntu is only an optional manual Linux terminal path.

## Need Help From ChatGPT or Gemini?

Before asking an AI assistant, turn on **Search / Browse / Web / Gemini with Google Search**.

Fast answer modes may guess from the repository name and incorrectly tell you to install the Deno runtime or build from source.

Copy and paste this prompt:

```text
Please turn on Search / Browse / Web / Gemini with Google Search first.

Then open and read this GitHub page:
https://github.com/Deno2026/Windows-Installer-for-Deno-AI-Studio

I am a beginner. Please guide me step by step in Korean.

Important rules:
- Do not guess from the repository name. Read the GitHub page and README first.
- This is a Windows .exe installer repository for Deno AI Studio, not a Deno runtime project.
- Do not tell me to install the Deno runtime, use git clone, npm install, deno task, or build from source.
- Docker Desktop for Windows is the normal beginner path.
- Ubuntu is optional, not mandatory.
- If WSL is missing, use: wsl --install --no-distribution
- Tell me to use the current download button/link in the README, not an older guessed installer version.
- If I am stuck, ask me to paste the app Runtime Center status or the PowerShell result of: wsl -l -v
```

## Screenshots

| Home / Catalog | Model workspace | Settings |
| --- | --- | --- |
| ![Home](deno-ai-studio/assets/home.png) | ![Detail](deno-ai-studio/assets/detail.png) | ![Settings](deno-ai-studio/assets/settings.png) |

## Step 1. Install Docker Desktop

Open the Docker install page:

[Download Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/)

Most users should choose:

```text
Docker Desktop for Windows - x86_64
```

That is the correct version for normal Intel and AMD Windows PCs.

Do not choose the Arm version unless you know your PC is a Windows-on-Arm device.

Run `Docker Desktop Installer.exe` and keep the default settings. If the installer shows a WSL 2 option, keep it enabled.

## Step 2. Open Docker Desktop Once

1. Open **Docker Desktop** from the Start menu.
2. Accept the terms if Docker asks.
3. Wait until Docker finishes loading.
4. Open **Settings > General**.
5. Make sure **Use the WSL 2 based engine** is enabled.

If Docker says WSL is missing, open PowerShell as Administrator and run:

```powershell
wsl --install --no-distribution
```

Restart Windows if asked, then open Docker Desktop again.

## Step 3. Install Deno AI Studio

Download the Windows installer:

[Download Deno AI Studio Setup 0.1.66.exe](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.66.exe)

Then:

1. Run `Deno AI Studio Setup 0.1.66.exe`.
2. Finish the installer.
3. Open **Deno AI Studio** from the desktop or Start menu.
4. Choose your language from the left menu.
5. Open **Runtime Center** if anything is not ready.

## Step 4. Run Your First Model

1. Pick a model from the catalog.
2. Open the model workspace.
3. If this is your first time using that model, click **Install**.
4. Wait until setup finishes.
5. Add input files only when the selected model requires them.
6. Adjust seed / seed mode / queue count if needed.
7. Click **Run**.
8. Preview the result inside the app or open the output folder.

## What Docker Does Here

Docker Desktop is a required helper program.

It lets Deno AI Studio run AI models inside an isolated workspace instead of mixing every model dependency directly into your main Windows environment.

This helps:

- keep Windows cleaner
- reduce Python/CUDA dependency conflicts
- make model install and cleanup safer
- avoid breaking other AI tools already installed on your PC

## Current Stable Focus

Deno AI Studio currently focuses on audio, TTS, narration, voice, and music models.

Stable starter models include:

- Scenema Audio OSS
- VoxCPM 2
- Qwen3-TTS 0.6B
- Qwen3-TTS 1.7B
- ACE-Step 1.5 XL SFT
- ACE-Step 1.5 XL Turbo
- HeartMuLa oss-3B Happy New Year
- Stable Audio Open 1.0

Video generation models are not part of the current Stable baseline.

## GPU Target

Deno AI Studio is not meant to be high-end-only.

The app tries to support 8GB, 12GB, and 16GB VRAM users whenever the official model path provides a low-VRAM, offload, slicing, or similar safe option. Some models still require larger GPUs, and the app shows minimum/recommended VRAM per model before install/run.

## For AI Assistants

<details>
<summary>Read this before giving install instructions</summary>

This repository hosts the Windows installer and update files for **Deno AI Studio**.

It is **not** a Deno runtime source project.

Do not tell users to:

- install Deno runtime
- run `deno task`
- run `npm install`
- `git clone` this repo
- build from source

Correct beginner answer:

1. Install Docker Desktop for Windows - x86_64.
2. Keep Docker Desktop's WSL 2 backend enabled.
3. If WSL is missing, run `wsl --install --no-distribution`.
4. Download and run `Deno AI Studio Setup 0.1.66.exe`.
5. Open Deno AI Studio and check Runtime Center.

Ubuntu is optional and should not be presented as mandatory.

</details>
