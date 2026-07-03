# Aura Privacy Policy

**Last updated:** 4 July 2026  
**App:** Aura for macOS  
**Developer:** Dipock Das

Aura turns what was said into something useful. This policy explains what Aura processes, what stays on your Mac, and what can leave your device.

---

## Summary

- **Audio is not stored.** Aura transcribes live and does not create or save audio recordings.
- **Transcription runs on your Mac** by default.
- **Transcript text stays on your Mac** until you run Transform and you are using a cloud AI provider.
- **Transform is optional.** Text leaves your Mac only when you choose a provider that processes it outside the device.
- **Aura does not collect, share or sell your data** and does not use third-party analytics in the current release.

---

## What Aura processes

Aura will process:

- Microphone audio (live, during recording)
- System audio (live, in lecture and meeting modes)
- Transcript text you create or edit
- Saved transcript files you choose to export
- API credentials you configure for cloud Transform providers to store them in your Keychain
- App settings stored on your Mac

---

## What stays on your Mac

| Data | Stays on-device |
|------|-----------------|
| Live microphone and system audio | Yes — processed in memory, not saved as audio files |
| Waveform / visualisation data | Yes |
| Apple Speech / Speech Analyzer transcription | Yes |
| Whisper transcription (when used) | Yes |
| On My Mac Transform (Ministral model) | Yes — after the model is downloaded |
| Ollama / LM Studio Transform | Yes — when those run locally |
| Transcripts | Yes — until you save or copy them to another location |
| Cloud API keys | Stored in the macOS Keychain |

---

## What Aura needs internet access for

| Action | What is it? | Where |
|--------|-------------|--------|
| Download Whisper model | Public model files | `huggingface.co` (HTTPS) |
| Download On My Mac Transform model | Public model files | Model host (HTTPS) |
| Transform if you choose a cloud provider | Cloud AI transformation of transacript | Ollama host (HTTPS) |

---


## What can leave your Mac (only when you choose)

| Action | What leaves | Where |
|--------|-------------|--------|
| Transform — Private Cloud | Transcript text | Your Ollama account (HTTPS) |
| Transform — Your AI Provider | Transcript text | OpenAI, Anthropic, or Google (HTTPS), using your API key |

Nothing is sent for **transcription** itself. Network use for Transform happens only when you press **Transform** with a configured provider that processes text outside your Mac.

---

## Permissions

Aura will request:

- **Microphone** — to capture your voice
- **Speech Recognition** — for Apple Speech on supported macOS versions
- **Screen Recording** — macOS uses this permission gate for **system audio** in lecture and meeting modes

Aura does **not** record or transmit screen pixels. The Screen Recording permission is required by macOS for system-audio capture only.

---

## Storage locations

| Data | Location |
|------|----------|
| Saved transcripts | Folder you choose, or Aura's app container by default |
| Whisper models | Aura's sandboxed Application Support |
| On My Mac Transform model | Aura's models folder in Application Support |
| Settings | UserDefaults in Aura's app container |
| API keys | macOS Keychain |

You control retention by deleting saved files and removing downloaded models in Settings.

---

## Sandboxing

Aura runs inside the macOS App Sandbox. It can access the microphone, make network requests when you trigger downloads or Transform, and read/write files you select through system panels. It cannot browse arbitrary folders without your action.

---

## Privacy manifest (App Store)

Aura's privacy manifest declares:

- No tracking
- No blanket developer-collected data types in the manifest
- UserDefaults access for app-private settings only (`CA92.1`)

---

## Help Others (charity links)

Aura is free. Settings includes optional links to external charity search pages. Aura does not process donations in the app and does not track whether you use those links in the current release.

---

## Children's privacy

Aura is not directed at children under 13. Aura does not knowingly collect personal information from children.

---

## Changes

This policy may be updated before or after App Store releases. The **Last updated** date at the top will change when it does.

---

## Contact

- **Bug reports and feature requests:** [github.com/dipockdas/aura-support/issues](https://github.com/dipockdas/aura-support/issues)
- **Privacy questions:** open an issue in the same repository and include "Privacy" in the title
