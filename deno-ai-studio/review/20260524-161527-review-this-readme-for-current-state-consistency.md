# Gemma4 Copy Review Transcript

- Created: 2026-05-24 16:15:27 +09:00
- Model: gemma4:31b-it-q4_K_M
- Ollama URL: http://127.0.0.1:11434
- Keep alive: 30m
- Think: false
- Lock: Global\DENO_Gemma4_CopyReview
- ComfyUI queue check: {"url":"http://127.0.0.1:8188","reachable":false,"running":null,"pending":null}
- num_predict: -1
- num_ctx: Ollama default / desktop setting

## Context

Deno AI Studio GitHub installer README for Windows beginners. Current app version: 0.1.69. This repository is the Windows installer/update host, not the source code repository. Screenshots must appear at the top. Current app navigation: Home, Installed, Settings, Runtime Center, Cleanup. Current stable model catalog order: ACE-Step 1.5 XL SFT, ACE-Step 1.5 XL Turbo, HeartMuLa oss-3B Happy New Year, Stable Audio Open 1.0, Scenema Audio OSS, VoxCPM 2, Qwen3-TTS 0.6B, Qwen3-TTS 1.7B. Beginner install path: Docker Desktop for Windows x86_64 with WSL 2 backend. Ubuntu is optional, not required.

## Task

Review this README for current-state consistency, beginner clarity, and overclaiming. Return concise issues and suggested edits only. Do not invent features. Prefer keeping the README short and practical.

## System Prompt

```text
You are a Korean UX copy consultant inside a Codex workflow.
Codex will handle engineering and final judgment.
Your job is to make wording natural, concise, warm, and context-aware.
Return practical copy that can be pasted into UI or scripts.
Do not over-explain. Do not invent product features.
If an exact technical term should stay unchanged, preserve it.
```

## User Prompt

```text
Context:
Deno AI Studio GitHub installer README for Windows beginners. Current app version: 0.1.69. This repository is the Windows installer/update host, not the source code repository. Screenshots must appear at the top. Current app navigation: Home, Installed, Settings, Runtime Center, Cleanup. Current stable model catalog order: ACE-Step 1.5 XL SFT, ACE-Step 1.5 XL Turbo, HeartMuLa oss-3B Happy New Year, Stable Audio Open 1.0, Scenema Audio OSS, VoxCPM 2, Qwen3-TTS 0.6B, Qwen3-TTS 1.7B. Beginner install path: Docker Desktop for Windows x86_64 with WSL 2 backend. Ubuntu is optional, not required.

Task:
Review this README for current-state consistency, beginner clarity, and overclaiming. Return concise issues and suggested edits only. Do not invent features. Prefer keeping the README short and practical.

Current wording or draft:
# [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.69.exe)

<p>
  <img src="deno-ai-studio/assets/home.png" alt="Deno AI Studio home catalog" width="49%">
  <img src="deno-ai-studio/assets/detail.png" alt="Deno AI Studio model workspace" width="49%">
</p>

Windows `.exe` installer for **Deno AI Studio**, a beginner-friendly desktop launcher for open-source AI models.

This repository is an installer/update host. It is **not** a Deno runtime project and it does not contain the source build workflow.

Current installer: **Deno AI Studio Setup 0.1.69.exe**

Latest update: The language selector now opens as a larger opaque flyout, with corrected stacking so model cards cannot overlap it.

If an AI chatbot mentions an older installer version, use the download button on this page instead of the old version it guessed.

[![STEP 1 Install Docker Desktop](https://img.shields.io/badge/STEP%201-Install%20Docker%20Desktop-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/desktop/setup/install/windows-install/)
[![STEP 2 Download Windows Installer](https://img.shields.io/badge/STEP%202-Download%20Windows%20Installer%20(.exe)-16A34A?style=for-the-badge&logo=github&logoColor=white)](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.69.exe)

## Start Here

Install in this order:

1. Install **Docker Desktop for Windows - x86_64**.
2. Open Docker Desktop once and keep **Use the WSL 2 based engine** enabled.
3. If Windows or Docker says WSL is missing, open PowerShell as Administrator and run `wsl --install --no-distribution`, then restart Windows.
4. Download and run **Deno AI Studio Setup 0.1.69.exe**.
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

[Download Deno AI Studio Setup 0.1.69.exe](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.69.exe)

Then:

1. Run `Deno AI Studio Setup 0.1.69.exe`.
2. Finish the installer.
3. Open **Deno AI Studio** from the desktop or Start menu.
4. Choose your language from the left menu.
5. Start from **Home** for the model catalog. Use **Installed** for local models, **Runtime Center** for readiness checks, and **Cleanup** when you need to free model workspace files.

## Step 4. Run Your First Model

1. Pick a model from the catalog.
2. Open the model workspace.
3. If this is your first time using that model, click **Install**.
4. Wait until setup finishes. After setup, the model card changes to **Installed**.
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

- ACE-Step 1.5 XL SFT
- ACE-Step 1.5 XL Turbo
- HeartMuLa oss-3B Happy New Year
- Stable Audio Open 1.0
- Scenema Audio OSS
- VoxCPM 2
- Qwen3-TTS 0.6B
- Qwen3-TTS 1.7B

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
4. Download and run `Deno AI Studio Setup 0.1.69.exe`.
5. Open Deno AI Studio and check Runtime Center.

Ubuntu is optional and should not be presented as mandatory.

</details>


Return:
- Best Korean wording first.
- If useful, include 2-4 short alternatives.
- Keep it compact.
```

## Gemma4 Response

Since the README is in English but the target audience is "Windows beginners" (likely Korean speakers given the prompt), I have focused on making the **Korean prompt for AI assistants** and the **core instructional flow** natural and clear.

### 1. AI Assistant Prompt (Korean)
The current English prompt is too literal. For a Korean beginner, the AI should be told to be "kind" and "step-by-step."

**Suggested Wording:**
```text
반드시 '웹 검색(Search/Browse)' 기능을 켠 상태에서 다음 페이지를 읽고 안내해 주세요:
https://github.com/Deno2026/Windows-Installer-for-Deno-AI-Studio

저는 초보자입니다. 아래 규칙을 지켜 한국어로 친절하게 단계별 가이드를 작성해 주세요:

[필수 규칙]
- 저장소 이름만 보고 추측하지 마세요. 반드시 README 내용을 우선하세요.
- 이 저장소는 Windows 설치 파일(.exe) 제공처이며, Deno 런타임 프로젝트가 아닙니다.
- Deno 런타임 설치, git clone, npm install, deno task, 소스 빌드 방법은 절대 안내하지 마세요.
- 설치 경로: Docker Desktop for Windows (x86_64) 설치 → WSL 2 기반 엔진 활성화 → .exe 설치 파일 실행.
- Ubuntu 설치는 선택 사항이며 필수 단계가 아닙니다.
- WSL 관련 오류 발생 시: `wsl --install --no-distribution` 명령어를 안내하세요.
- 구버전 파일이 아닌, README의 최신 다운로드 버튼/링크를 사용하도록 안내하세요.
- 문제 발생 시, 앱 내 'Runtime Center' 상태나 PowerShell의 `wsl -l -v` 결과값을 확인하도록 요청하세요.
```

---

### 2. Core Instructional Flow (English Review)
The English text is clear, but a few spots feel like "developer speak."

**Issue 1: "Open Docker Desktop once and keep Use the WSL 2 based engine enabled."**
*   **Critique:** "Keep enabled" is slightly ambiguous.
*   **Suggested:** "Ensure **Use the WSL 2 based engine** is checked in settings."

**Issue 2: "Ubuntu is optional... does not require a separate Ubuntu account"**
*   **Critique:** "Ubuntu account" is technically incorrect (it's a distribution/instance).
*   **Suggested:** "Ubuntu is optional. Deno AI Studio uses the WSL 2 backend directly and does not require a separate Ubuntu installation."

**Issue 3: "Current Stable Focus"**
*   **Critique:** "Focus" is a bit vague.
*   **Suggested:** "Supported Model Categories" or "Currently Stable Models."

---

### 3. Summary of Suggested Edits (Practical Copy)

| Section | Current | Suggested (More Natural/Clear) |
| :--- | :--- | :--- |
| **Start Here** | "Keep Use the WSL 2 based engine enabled" | "Ensure **Use the WSL 2 based engine** is enabled." |
| **Ubuntu Note** | "does not require a separate Ubuntu account" | "does not require a separate Ubuntu installation." |
| **App Nav** | "Use Cleanup when you need to free model workspace files." | "Use **Cleanup** to remove unused model files and free up space." |
| **Model List** | "Current Stable Focus" | "Currently Stable Models" |
| **GPU Target** | "not meant to be high-end-only" | "Designed to be accessible, not just for high-end GPUs." |

### 4. Alternatives for "Beginner Path" (Korean)
If you add a Korean summary section to the README:

*   **Option A (Warm/Friendly):** "초보자분들은 이 순서대로 설치해 주세요." (For beginners, please install in this order.)
*   **Option B (Concise/Direct):** "빠른 설치 가이드" (Quick Install Guide)
*   **Option C (Professional):** "Windows 사용자 설치 절차" (Installation Procedure for Windows Users)

## Codex Selection Notes

Fill this section when applying the suggestions:

- Selected:
- Adapted:
- Rejected:
- Reason: