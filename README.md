# CodexAutoTime — Windows releases

**Latest release: [v1.2.6](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/tag/v1.2.6)**

## Downloads

- **[Portable ZIP (recommended)](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/download/v1.2.6/CodexAutoTime-Windows-v1.2.6.zip)** — includes the GUI executable, local queue scheduler, and Chinese installation/usage notes.
- [GUI executable only](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/download/v1.2.6/CodexAutoTime.exe)
- [SHA-256 checksums](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/download/v1.2.6/SHA256SUMS.txt)

## v1.2.6 changes

- Fixed startup failure in the compiled EXE when `$PSScriptRoot` is empty.
- Added a visible Codex CLI status check that runs `codex --version`.
- Added a one-click installer using OpenAI's official Windows installer endpoint.
- Added fallback log paths for unusual Windows user profiles.

## Installation

1. Download the portable ZIP and extract all files into the same folder.
2. Run `CodexAutoTime.exe`.
3. Check the Codex CLI status at the top of the window. If it is missing, use **Install Codex CLI**; the installer requires internet access and then verifies `codex --version`.
4. The local scheduled-delivery mode depends on the accompanying `CodexQueueScheduler.ps1`; do not separate it from the other files.
5. Read the included Chinese installation notes before setting up scheduled delivery.

## What it does

CodexAutoTime is a Windows GUI utility for finding local Codex sessions, scheduling messages to a selected session through Windows Task Scheduler, and generating concise native scheduled-task instructions that can be pasted into the current Codex conversation.

It does **not** bypass Codex usage limits. Local delivery is bound to the selected session UUID; chat-instruction mode generates text and cannot guarantee that the Codex client creates or cancels its plans.

## Verification note

GitHub Actions confirms that v1.2.6 compiled and its release assets were uploaded. Please still test GUI startup, CLI installation, session discovery, queue delivery, and task cancellation on the target Windows account.

## Previous release

[CodexAutoTime GUI v1.2.5](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/tag/v1.2.5)

## Source

The source repository is private: [CodexAutoTime](https://github.com/940963818qieke-crypto/CodexAutoTime).
