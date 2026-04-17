# Codex-Prompt-to-usable-App
A reusable Codex prompt for building a Windows voice input app that runs persistently in the system tray.

# Development & Build Prerequisites
Add this directly to your `README.md` as standard English documentation:

## Prerequisites
Before building or developing VoiceBar, please complete the following environment preparation:

- A **Windows 11 x64** device, 23H2 or newer.
  The project targets WPF Windows desktop and is packaged for `win-x64`.
- Install the **x64 .NET SDK**.
  The framework target is `net8.0-windows10.0.22621.0`. A .NET 8 compatible SDK is required for compilation and building.
- Active internet connection.
  Network access is required for initial NuGet package restoration and automatic Whisper speech model downloading on first launch.
- Ensure **PowerShell** is available.
  Built-in model download and signing scripts rely on PowerShell execution.
- `make` is optional.
  You may use `make build` / `make publish` if Make is installed; alternatively, use native `dotnet build` and `dotnet publish` directly.
- A working microphone and enabled Windows microphone privacy permissions (required for full voice recording and transcription features).
- Optional: OpenAI-compatible API information (`API Base URL`, `API Key`, `Model name`) if you need to test and enable LLM text refinement.
- Optional: Code signing certificate, `signtool.exe`, and system environment variables (`SIGN_CERT_PATH`, `SIGN_CERT_PASSWORD`) for signed release builds. Code signing can be skipped for regular usage.

### Minimal Environment Checklist
For basic compilation and testing, only four requirements are mandatory:
1. Windows 11 x64 (23H2+)
2. x64 .NET 8 SDK
3. Internet access
4. Available PowerShell
