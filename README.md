# Trex Story AI — Khmer Dub V2 🦖

This version is designed for the exact workflow:
**Upload foreign-language video → speech recognition → Khmer translation → Khmer TTS → audio/video mixing → Khmer-dubbed MP4.**

The UI and backend are ready, but a real production dub still needs API/provider adapters and server-side media processing. The code deliberately refuses to claim a finished MP4 when provider keys/adapters are missing.

Recommended production architecture:
1. Extract audio with FFmpeg.
2. Speech-to-text with timestamps.
3. Translate each dialogue segment into natural Khmer.
4. Generate Khmer speech for each segment.
5. Time-stretch/pad segments when needed.
6. Mix Khmer voice with original music/SFX.
7. Export MP4 and provide a download link.

Use only videos you have permission to process and redistribute.
