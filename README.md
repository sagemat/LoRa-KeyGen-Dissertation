LoRa Key Generation (Dissertation)

End-to-end key generation over LoRa/LPWAN for constrained devices.
Pipeline: RSSI sampling → quantization → custom packet matching (no ACK) → information reconciliation (BCH-inspired) → SHA-256.

📄 PDF:

GitHub viewer: Alex's LoRa Comms protocol.pdf

Direct (raw): https://raw.githubusercontent.com/sagemat/LoRa-KeyGen-Dissertation/main/Alex%27s%20LoRa%20Comms%20protocol.pdf

Highlights

Packet matching without ACK: keep Alice/Bob vectors aligned using receiver packet counts.

Robust reconciliation: simple, BCH-inspired method to correct bit mismatches before hashing.

Real-world tests: multi-floor lab runs & elevator scenario; synchronized counts and matching final hashes.

Constraints explicit: ~3 minutes time-to-key under low-power assumptions.

Why it matters

LoRa links are low-power and narrow-band. This design favors clarity under constraints: minimal protocol surface, measurable timing/energy, and a practical route to secure pairing in hostile RF conditions.

Contact

Questions or context: Alexandru Mateescu · mateescu.alexandru2001@gmail.com
