# Diego Angarita

Systems and Computing Engineer from Barranquilla, Colombia. I build real-time systems, data pipelines and applied AI.

## Ya Viene

Live bus tracking for Barranquilla: where your bus is, and how far away it is along its route.

- **Real-time backend** ([YaVieneBackend](https://github.com/elDiego5599/YaVieneBackend)): GPS over MQTT, WebSocket fan-out to the apps, SQLite storage.
- **Data pipeline**: a position history consolidated daily into an hourly service summary, with quality checks per day. Route KPIs for bus companies: buses per hour, speed in motion and headway (median and p90 at the route midpoint), exportable to CSV.
- **Applied AI**: a bus occupancy estimator from onboard cameras. EfficientNet-B0 fine-tuned with ordinal thresholds, five-frame averaging and two-camera fusion, thresholds calibrated against over-estimation. Trained on GPU, runs on CPU over RTSP.
- **Apps** ([YaViene](https://github.com/elDiego5599/YaViene)): Flutter passenger app with along-route distance alerts and iOS Live Activities, plus a macOS and Windows fleet control panel.
- **Web** ([YaVieneWeb](https://github.com/elDiego5599/YaVieneWeb)): landing for passengers and a page for bus companies with a live map.
- **Infrastructure**: services under launchd, public access through an ngrok tunnel with a Fly.io backup (failover in under a minute), CI on GitHub Actions with stability and secret scanning.
- **Quality**: more than 1,900 automated tests across the three repos, with mutation testing.

The along-route idea is published on its own as [alongroute](https://github.com/elDiego5599/alongroute).

## Other work

- [Vanta](https://github.com/elDiego5599/Vanta): offline forensic audio and video analysis with local Whisper, SHA-256 chain of custody and AES-256. Tauri (Rust) + React.
- [ParallelAgent](https://github.com/elDiego5599/ParallelAgent): local multi-LLM deliberation for coding tasks on real repositories.

## Stack

TypeScript, Node.js, Dart and Flutter, Python and PyTorch, Rust (Tauri), SQLite and PostgreSQL, MQTT and WebSockets, GitHub Actions, Fly.io, ngrok.
