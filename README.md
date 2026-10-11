# Film audio skills

This repository contains three separate Codex skills:

1. [`film-audio-python`](SKILL.md) analyzes a locked film, creates a detailed cue sheet and PDF, and generates labeled local Python music and sound assets.
2. [`film-audio-video-finish`](skills/film-audio-video-finish/SKILL.md) places those assets against the locked picture, mixes and masters them, and exports a final video plus a 48 kHz/24-bit WAV master.
3. [`film-audio-reaper-mix`](skills/film-audio-reaper-mix/SKILL.md) prepares a labeled REAPER project from the same audio package and mix plan, then guides the picture-synced mix and final WAV render in REAPER.

Install the skills you need as siblings under your Codex skills directory. On Windows, follow [the setup guide](references/windows_setup.md). Run the selected skill's `scripts/smoke_test.py` on the computer that will perform the work before processing a film. The finishing and REAPER skills use Python's standard library and FFmpeg; the first skill additionally needs the packages in [`requirements.txt`](requirements.txt). The REAPER skill also requires an in-app import and render check on the target computer.
