# CodexAutoTime — Windows releases

**Latest release: [v1.2.5](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/tag/v1.2.5)**

## Downloads

- **[Portable ZIP (recommended)](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/download/v1.2.5/CodexAutoTime-Windows-v1.2.5.zip)** — includes the GUI executable, local queue scheduler, and Chinese installation/usage notes.
- [GUI executable only](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/download/v1.2.5/CodexAutoTime.exe)
- [SHA-256 checksums](https://github.com/940963818qieke-crypto/CodexAutoTime-Releases/releases/download/v1.2.5/SHA256SUMS.txt)

## Installation

1. Download the portable ZIP and extract all files into the same folder.
2. Ensure Codex CLI is installed and `codex --version` works for the same Windows user.
3. Run CodexAutoTime.exe. The local scheduled-delivery mode depends on the accompanying CodexQueueScheduler.ps1; do not separate it from the other files.
4. Read the included Chinese installation notes before setting up scheduled delivery.

## What it does

CodexAutoTime is a Windows GUI utility for finding local Codex sessions, scheduling messages to a selected session through Windows Task Scheduler, and generating concise native scheduled-task instructions that can be pasted into the current Codex conversation.

It does **not** bypass Codex usage limits. Local delivery is bound to the selected session UUID; chat-instruction mode generates text and cannot guarantee that the Codex client creates or cancels its plans.

## Build status

Release v1.2.5 was built and packaged by the Windows GitHub Actions runner. A successful CI build is not a substitute for testing the GUI and scheduled delivery on your own Windows account.

## Source

The source repository is private: [CodexAutoTime](https://github.com/940963818qieke-crypto/CodexAutoTime).
