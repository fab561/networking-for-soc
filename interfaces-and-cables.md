# Interfaces and Cables

## 1. RJ-45 and Ethernet

### RJ-45
RJ-45 is a standard connector used for Ethernet networking.
It connects UTP cables to network devices.

### Ethernet
Ethernet is a networking technology used in LANs.
It defines how devices communicate over wired connections.

Ethernet standards are defined by IEEE (Institute of Electrical and Electronics Engineers).

---

## 2. Network Speed Measurement

- Network speed is measured in bits per second (bps).
- 1 byte = 8 bits.
- Examples:
  - 100 Mbps = 100 megabits per second
  - 1 Gbps = 1000 megabits per second

---

## 3. Common Ethernet Copper Standards

| Common Name | IEEE Standard | Speed | Max Length |
|-------------|--------------|--------|------------|
| 10BASE-T    | 802.3i       | 10 Mbps  | 100 meters |
| 100BASE-TX  | 802.3u       | 100 Mbps | 100 meters |
| 1000BASE-T  | 802.3ab      | 1 Gbps   | 100 meters |
| 10GBASE-T   | 802.3an      | 10 Gbps  | 100 meters |

All above use UTP copper cables.

---

## 4. UTP Cables

### UTP (Unshielded Twisted Pair)
- Most common Ethernet cable
- Contains twisted wire pairs
- Twisting reduces EMI (Electromagnetic Interference)

### EMI
Electromagnetic interference affects signal quality.
Twisting wires helps cancel interference.

---

## 5. Straight-Through vs Crossover Cable

### Straight-Through Cable
Used between:
- PC → Switch
- Router → Switch

Transmit pins connect to receive pins automatically via switch.

### Crossover Cable
Used between similar devices:
- PC → PC
- Switch → Switch
- Router → Router

Transmit and receive wires are crossed.

---

## 6. Pin Usage (10BASE-T / 100BASE-TX)

These use 2 pairs (4 wires):

- Pins 1,2 → Transmit (TX)
- Pins 3,6 → Receive (RX)

Example:

| Device Type | TX Pins | RX Pins |
|-------------|--------|--------|
| PC          | 1,2    | 3,6    |
| Switch      | 3,6    | 1,2    |

---

## 7. Auto MDI-X

Auto MDI-X automatically detects cable type.
Modern devices adjust TX/RX automatically.
Crossover cables usually not required today.

---

## 8. 1000BASE-T and 10GBASE-T

These use:
- 4 wire pairs (8 wires total)
- All pairs transmit and receive simultaneously

Speed:
- 1000BASE-T → 1 Gbps
- 10GBASE-T → 10 Gbps

---

## 9. Categories of UTP Cables

| Category | Max Speed | Notes |
|----------|-----------|------|
| Cat5     | 100 Mbps  | Older |
| Cat5e    | 1 Gbps    | Most common |
| Cat6     | 10 Gbps (short distance) | Better shielding |
| Cat6a    | 10 Gbps | Better performance |
| Cat7     | Higher shielding | Less common in LAN |

---

## 10. Fiber Optic Cables

Used for:
- High speed
- Long distance
- Less EMI interference

Uses light instead of electrical signals.

---

## 11. Fiber Optic Cable Components

- Core → carries light
- Cladding → reflects light inward
- Buffer coating → protection
- Outer jacket → physical protection

---

## 12. Single-Mode vs Multi-Mode Fiber

### Single-Mode Fiber (SMF)
- Long distance
- Very small core
- Used in ISPs / WAN

### Multi-Mode Fiber (MMF)
- Shorter distance
- Larger core
- Used in data centers

---

## 13. Fiber Ethernet Standards

| Informal Name | IEEE Standard | Speed | Cable Type | Max Distance |
|--------------|--------------|-------|-------------|--------------|
| 1000BASE-SX  | 802.3z       | 1 Gbps | Multi-mode  | ~550m |
| 1000BASE-LX  | 802.3z       | 1 Gbps | Single-mode | ~5 km |
| 10GBASE-SR   | 802.3ae      | 10 Gbps | Multi-mode | ~300m |
| 10GBASE-LR   | 802.3ae      | 10 Gbps | Single-mode | ~10 km |

---

## 14. UTP vs Fiber Comparison

| Feature | UTP | Fiber |
|----------|------|--------|
| Signal type | Electrical | Light |
| EMI interference | Possible | None |
| Distance | Short (100m typical) | Long (km) |
| Cost | Cheaper | More expensive |
| Speed | High (up to 10G) | Very high |

---

## SOC Relevance

Understanding cables and interfaces helps with:

- Identifying network bottlenecks
- Understanding physical segmentation
- Recognizing infrastructure limitations
- Troubleshooting connectivity issues
