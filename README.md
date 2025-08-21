# Moodify — Ready-to-Run Web Prototype

This package is **plug-and-play**:

## Quick Start (VS Code)
1. Open this folder in **VS Code**.
2. Install the **Live Server** extension (by Ritwick Dey) if not already.
3. Right‑click `index.html` → **Open with Live Server**.
4. Click **Start camera & scan** → allow camera access.

> If you see `models not found — run get_models.py`: double‑click **get_models.py** or run it once (see below).

## Models (face-api.js)
Run the helper script to download the small pretrained models into `./models/`:

```bash
# from this folder
python get_models.py
```

This will download:
- `tiny_face_detector_model-weights_manifest.json`
- `tiny_face_detector_model-shard1`
- `face_expression_model-weights_manifest.json`
- `face_expression_model-shard1`

## Demo Music
Royalty‑free **WAV demo tones** are included in `songs/`:
- `happy.wav`, `sad.wav`, `angry.wav`, `neutral.wav`

You can replace them with your own MP3/WAV files and update paths in `script.js`.

## Quotes
Edit `data/quotes.json` to customize motivational messages per mood.

## Docs
- `docs/architecture.png` — bright infographic flow of the app
- `docs/architecture.pdf` — print‑friendly version

## Notes
- For camera to work on mobile, serve over HTTPS or use `localhost`.
- If detection feels jittery, adjust the threshold `> 0.6` in `script.js`.
