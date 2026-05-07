# J1939 Sniffer Pro

> A Python CAN bus and J1939 traffic decoder with 50+ pre-configured PGNs, DM1 fault code parsing, and a built-in traffic simulator — replace $3,000 commercial CAN analyzers with a $59 Python tool.
<img width="1280" height="720" alt="封面" src="https://github.com/user-attachments/assets/7bdf070e-7ef5-4606-b951-c69d977fd8e1" />

**This is a commercial tool, sold on Gumroad.** Source code is included in your purchase.

---

## What it does

- **Real-time J1939 PGN decoding** with 50+ pre-configured Parameter Group Numbers
- **DM1 fault code parser** — see active diagnostic codes from your ECU as text, not raw hex
- **Built-in traffic simulator** — generate realistic J1939 frames without needing a real truck or genset
- **CAN bus support** via python-can — works with PCAN, Vector, Kvaser, SocketCAN, virtual CAN
- **Live message decoder** — SPNs broken out with units (RPM, °C, kPa, %, etc.)
- **CSV logging** — every decoded message timestamped for offline analysis
- **Single-file Python** with python-can backend

## Why this exists

Commercial J1939 analyzers like Vector CANalyzer cost $3,000-8,000 per seat. Most engineers debugging fleet vehicles, gensets, or off-highway equipment don't need a full suite — they need to decode 10-20 common PGNs and read DM1 fault codes during commissioning.

This tool covers 80% of those workflows for less than 2% of the price.

## Pre-configured PGNs include

- **EEC1** (Electronic Engine Controller 1) — speed, torque, mode
- **EEC2** — accelerator pedal position, load
- **DM1 / DM2** — active and previously active diagnostic codes
- **VEP1** (Vehicle Electrical Power) — battery voltage, alternator current
- **EFC** (Engine Fluid Level/Pressure)
- **CCVS** (Cruise Control / Vehicle Speed)
- **AT1IG1** (Aftertreatment 1 Intake Gas)
- **TCO1** (Tachograph)
- **HOURS** — engine total hours, trip distance
- ...and 40+ more

## Use cases

| Scenario | Why this tool fits |
|---|---|
| Fleet maintenance debugging | Read DM1 codes without OEM scan tools |
| Genset commissioning | Verify EEC1/EEC2 messages from new engines |
| Off-highway equipment | Cummins, Caterpillar, John Deere J1939 streams |
| ADAS/AV development | Inject simulated CAN traffic for testing |
| Education / training | Visualize J1939 protocol without real hardware |

## Get it

→ **[J1939 Sniffer Pro on Gumroad — $59](https://philyeh.gumroad.com/l/j1939-decoder-pro)**

Or grab the **[Industrial Toolkit Bundle](https://philyeh.gumroad.com/l/industrial-toolkit-bundle)** ($129) — J1939 + Modbus + MQTT + EtherNet/IP together.

## What's in the purchase

- `j1939_sniffer.py` — Single-file Python application
- `pgn_definitions.json` — 50+ PGN definitions (extend it yourself)
- `requirements.txt` — Pinned dependencies
- `README.md` — Setup guide for PCAN / SocketCAN / Vector
- Commercial use license per Gumroad EULA

## License

Commercial use license per Gumroad EULA. You may use this software at the company that purchased it for any commercial purpose. Redistribution, resale, or open-sourcing the code is not permitted.

## Support

- Reply to your Gumroad purchase email
- Bug reports / new PGN requests via [GitHub Issues](https://github.com/PhilYeh1212/Python-CAN-Bus-J1939-Sniffer-GUI/issues)

---

I write about industrial Python and protocol internals at **[dev.to/philyeh](https://dev.to/philyeh)**, and post Chinese versions on [iThelp](https://ithelp.ithome.com.tw/users/20171204).

— Phil Yeh · Senior Automation Engineer · Industrial Python · Developer Tools
