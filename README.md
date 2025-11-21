# F1 Race Replay

A Python application for visualizing Formula 1 race telemetry and replaying race events with interactive controls and a graphical interface.

## Features

- **Race Replay Visualization:** Watch the race unfold with real-time driver positions on a rendered track.
- **Leaderboard:** See live driver positions and gaps to the car ahead.
- **Lap & Time Display:** Track the current lap and total race time.
- **Driver Status:** Drivers who retire or go out are marked as "OUT" on the leaderboard.
- **Interactive Controls:** Pause, rewind, fast forward, and adjust playback speed using on-screen buttons or keyboard shortcuts.
- **Loading Screen:** Animated loading bar with driver progress.
- **Legend:** On-screen legend explains all controls.

## Controls

- **Pause/Resume:** SPACE or Pause button
- **Rewind/Fast Forward:** ← / → or Rewind/Fast Forward buttons
- **Playback Speed:** ↑ / ↓ or Speed button (cycles through 0.5x, 1x, 2x, 4x)
- **Set Speed Directly:** Keys 1–4

## Requirements

- Python 3.8+
- [FastF1](https://github.com/theOehrly/Fast-F1)
- [Arcade](https://api.arcade.academy/en/latest/)
- numpy

Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

Run the main script and specify the year and round:
```bash
python main.py --year 2025 --round 12
```

## File Structure

- `main.py` — Entry point, handles session loading and starts the replay.
- `src/f1_data.py` — Telemetry loading, processing, and frame generation.
- `src/arcade_replay.py` — Visualization and UI logic.

## Customization

- Change track width, colors, and UI layout in `src/arcade_replay.py`.
- Adjust telemetry processing in `src/f1_data.py`.

## Contributing

- Open pull requests for UI improvements or new features.
- Report issues on GitHub.

# Known Issues

- Occasional telemetry data gaps cause accuracy issues with the leaderboard

## 📝 License

This project is licensed under the MIT License.

---

Built with ❤️ by [Tom Shaw](https://tomshaw.dev)