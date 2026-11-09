# Open Chime

Open Chime is an open-source smart doorbell system that runs entirely on hardware you own. No cloud account, no subscription, and no video leaving your home.

It aims to be as beautiful as a designer doorbell, as secure as an expensive security system, and as private as your own home.

## Products

| Product | What it is | Hardware | Status |
|---------|------------|----------|--------|
| **Chime** | Speaker box that plays doorbell sounds when triggered over MQTT | Raspberry Pi Zero W, MAX98357A I2S amp, 3D-printed enclosure | In active development |
| **Ring** | The doorbell: camera, buttons, audio, and door relays | Raspberry Pi Zero 2 W, Camera Module 3 Wide, Kailh BOX buttons | Next up |
| **Base** | Future product, details to come | TBD | Planned |

Each device runs a custom minimal Linux image built with Buildroot. It boots in seconds, runs compiled C++ services, and updates over the air with A/B root filesystem slots.

## Why local-first

A doorbell sees everyone who comes to your door. Open Chime keeps that data on your network:

- **No cloud dependency.** Devices talk to each other over your local network via MQTT. The system keeps working when the internet is down or a vendor shuts down.
- **Private by default.** Camera, audio, and event data stay on hardware you control.
- **Open and auditable.** All software, hardware designs, and wiring are in the open. You can read, build, and change every part of it.

## Get started

- Code, OS images, and hardware: [openchime-org/openchime](https://github.com/openchime-org/openchime)
- Website: [openchime.org](https://openchime.org)
- Build and flash an image: [Buildroot guide](https://github.com/openchime-org/openchime/blob/main/buildroot/README.md)
- Hardware, BOM, and wiring: [Chime](https://github.com/openchime-org/openchime/blob/main/hardware/chime/README.md), [Ring](https://github.com/openchime-org/openchime/blob/main/hardware/ring/README.md)

## Contribute

Issues and pull requests are welcome in [openchime-org/openchime](https://github.com/openchime-org/openchime).
