<div align="center">

# P.I.L.L.A.R.S

**Parkinson's Intelligent Living, Long-term AIoT Remote Supervision**
A wristband that notices a fall or a freeze, a home hub that hands out the right pills to the right person,
and a caregiver app that sees both, even when the house loses its Internet.

<br />

![Result](https://img.shields.io/badge/🏆_First_Runner--Up-1A9D92?style=for-the-badge)
![Challenge](https://img.shields.io/badge/FPT_IoT_Challenge-2026-14305A?style=for-the-badge)
![Partner](https://img.shields.io/badge/Edge_AI_for_Healthcare-Silicon_Labs-C0392B?style=for-the-badge)

![EFR32](https://img.shields.io/badge/Silicon_Labs_EFR32xG26-14305A?style=flat-square)
![TFLite Micro](https://img.shields.io/badge/TFLite_Micro-14305A?style=flat-square&logo=tensorflow&logoColor=F2F0EA)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi_5-14305A?style=flat-square&logo=raspberrypi&logoColor=F2F0EA)
![ESP32](https://img.shields.io/badge/ESP32-14305A?style=flat-square&logo=espressif&logoColor=F2F0EA)
![FastAPI](https://img.shields.io/badge/FastAPI-14305A?style=flat-square&logo=fastapi&logoColor=F2F0EA)
![Next.js](https://img.shields.io/badge/Next.js_15-14305A?style=flat-square&logo=nextdotjs&logoColor=F2F0EA)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14305A?style=flat-square&logo=postgresql&logoColor=F2F0EA)
![Redis](https://img.shields.io/badge/Redis-14305A?style=flat-square&logo=redis&logoColor=F2F0EA)
![three.js](https://img.shields.io/badge/three.js-14305A?style=flat-square&logo=threedotjs&logoColor=F2F0EA)
![Docker](https://img.shields.io/badge/Docker-14305A?style=flat-square&logo=docker&logoColor=F2F0EA)

</div>

> [!NOTE]
> Team **MLIoT – Edgelectronix**, FPT IoT Challenge 2026 (*Smart Healthcare with Edge AI*, with Silicon Labs),
> May to September 2026. **First Runner-Up** at the Grand Final in Hanoi. This repo is a **showcase**;
> the firmware, Station and Cloud source are private.

> [!IMPORTANT]
> P.I.L.L.A.R.S provides **structured monitoring data only**. It does not diagnose Parkinson's disease,
> does not replace clinical care, and never changes a medication or a dose by itself. Every detected
> event (fall, freeze, cough, missed dose) is a *possible*, model-estimated indicator with a confidence
> score, not a clinical finding.

<p align="center"><img src="assets/hero.jpg" alt="The P-Station at the Grand Final: a blue two-layer pill dispenser with eight cups, a pickup mug at the front and a tablet kiosk on top" /></p>
<p align="center"><sub>The P-Station at the Grand Final: eight medication cups in two layers, the pickup cup at the front, the kiosk on top.</sub></p>

<br />

## 🏆 Result

### **First Runner-Up**, FPT IoT Challenge 2026 Grand Final ✅

Out of the Top 10 finalists, at the Grand Final & Award Ceremony in Hanoi on **18 September 2026**.

<p align="center"><img src="assets/award.jpg" alt="The team on stage receiving the First Runner-Up award, with certificates, flowers and the award board" /></p>

<br />

## 🧠 The problem

People with Parkinson's live on a tight medication clock. Levodopa wears off between doses (the
"OFF" periods), and that is when freezing of gait and falls get more likely. Families can't watch all
day, and clinic visits only see a 15-minute snapshot.

P.I.L.L.A.R.S tries to close that gap at home:

1. **Take the right pills on time**: a dispenser that only opens for the right person, at the right time
2. **Notice what happens between doses**: a wristband that flags a possible fall, freeze or SOS on its own
3. **Tell someone**: a caregiver app with a live feed, alerts and the history a doctor can actually read

<br />

## 👥 Team

**MLIoT – Edgelectronix**, two Electrical-Electronic and two Robotics & Mechatronics engineering students.

<p align="center"><img src="assets/team.jpg" width="560" alt="The four team members standing in front of the Silicon Labs logo" /></p>

| | Who | What |
| :--- | :--- | :--- |
| 🧠 | **Đặng Như Phước** (lead) | Fall, fall-direction and freezing-of-gait models, the voice and cough model, wristband firmware, Cloud backend and caregiver app, Station pairing and the BLE pipeline |
| 💊 | **Trương Gia Bảo** (me) | Fall-detection dataset collection, pill dispenser hardware and firmware (2 × ESP32 motor layers, Pi-side IR counting, cup-pickup sensor), bench bring-up, the Station's smart-home kiosk UI |
| 🖥️ | **Huỳnh Trọng Khiêm** | Raspberry Pi Station backend, kiosk dose flow, dispense scheduling and status LEDs, prescription reading, the LAN-only demo fallback |
| 🔌 | **Hồ Minh Thao** | Wearable hardware (sensors, MCUs, mic, buzzer), power and charging, schematics and PCBs, the movement safety dashboard and 3D patient twin |

<br />

## 📷 The build

<p align="center"><img src="assets/station.gif" width="480" alt="The P-Station inside its lit acrylic display case at the venue" /></p>
<p align="center"><sub>The Station in its display case, set up at the venue the night before the final.</sub></p>

<table>
<tr>
<td width="50%" align="center"><img src="assets/wearable.jpg" alt="Close-up of the wearable prototypes: a wrist board with a round display on a strap, and a second board with a small screen" /><br /><sub>The P-Wearable prototypes on their straps</sub></td>
<td width="50%" align="center"><img src="assets/wearable-held.jpg" alt="The wristband prototype held up at the booth next to a smartwatch" /><br /><sub>The wristband at the booth</sub></td>
</tr>
</table>

<table>
<tr>
<td width="50%" align="center"><img src="assets/slide-wrist-pcb.jpg" alt="Wristband schematic (power and charging, MCU A for IMU fusion and fall/FoG, MCU B for BLE and voice) and its two-layer PCB layout" /><br /><sub>Wristband schematic and PCB: power, MCU A (IMU fusion, fall / FoG), MCU B (BLE, voice)</sub></td>
<td width="50%" align="center"><img src="assets/slide-ankle-pcb.jpg" alt="Ankle band schematic built around the BGM220 with its IMU, and its PCB layout" /><br /><sub>Ankle band schematic and PCB: BGM220 + IMU</sub></td>
</tr>
</table>

<p align="center"><img src="assets/booth.jpg" alt="Two booth photos: the team demoing the Station kiosk to visitors and judges, and a team member using the kiosk on top of the dispenser" /></p>
<p align="center"><sub>Demoing the Station to judges and visitors at the booth.</sub></p>

<br />

## 🏗️ Three tiers, one rule

**The Cloud decides, the home executes, every event is written down before it travels.**

```mermaid
flowchart LR
    subgraph W["⌚ P-Wearable"]
        ANK["Ankle node<br/>BGM220 IMU"]
        A["Wrist MCU A · EFR32xG26<br/>Fall / FoG model · buzzer"]
        B["Wrist MCU B · EFR32xG26<br/>TFT · cough model · BLE gateway"]
        ANK -- BLE --> A
        A -- "UART event + ACK" --> B
    end

    subgraph S["🏠 P-Station · Raspberry Pi 5"]
        BLE["ble-ingestor"]
        SAPI["station-api<br/>FaceID · PIN · schedule"]
        SDB[("PostgreSQL<br/>events + outbox")]
        SYNC["cloud-sync-worker"]
        KIOSK["Kiosk UI"]
        DISP["Dispenser<br/>2 × ESP32 · 8 cups"]
        BLE --> SAPI --> SDB
        SDB <--> SYNC
        KIOSK <-- "REST + SSE" --> SAPI
        SAPI --> DISP
    end

    subgraph C["☁️ P-Cloud"]
        API["cloud-api"]
        CDB[("PostgreSQL")]
        WEB["Caregiver app"]
        API --> CDB
        WEB <-- "REST + SSE" --> API
    end

    B -- "BLE notify" --> BLE
    BLE -- "dose reminder" --> B
    SYNC <-- "HTTPS · station token" --> API
```

| Tier | Owns | Keeps working without… |
| :--- | :--- | :--- |
| **P-Wearable** | Sensing and the first, fastest decision: fall, freeze, SOS, cough | the Pi and the Internet: the buzzer fires on the wrist |
| **P-Station** | Who is standing in front of it, which pills are due, turning the motors, writing every event locally | the Internet: dispensing, alerts and the kiosk all run offline |
| **P-Cloud** | Accounts, patients, consent, confirmed medication plans, long-term history, caregiver alerts | nothing; it's the source of truth the Station caches |

<br />

## ⌚ The wristband

A wristband with **two Silicon Labs EFR32xG26 MCUs** and an ankle node:

- **MCU A** pairs with the ankle IMU, fuses both, and runs the **fall and freezing-of-gait** models
  on-device. It drives the buzzer itself, so a fall alarm never waits on Bluetooth or Wi-Fi.
- **MCU B** is the gateway: it takes compact events from MCU A over UART, listens on its microphone
  for **"help", "good" and coughs**, draws on a round GC9A01 TFT, and serves BLE to the Station.
- In normal use it sends **events, not raw streams**. Raw IMU (10 Hz, 20-byte samples) is a debug and
  dataset-collection switch only.

<p align="center"><img src="assets/ble-packet.png" alt="The 12-byte BLE event packet: version, type, seq, flags, a 4-byte timestamp and a 4-byte payload, and the table of event codes from fall (P0) to cough (P2)" /></p>

The wristband never knows **who** is wearing it. The Cloud owns the wrist ↔ patient assignment and
syncs it to the Pi, which tags each event with the right patient. Unpair a wrist and its events stop
belonging to anyone.

<br />

## ⚡ Edge AI on the wrist

Both models run **on the wristband**, full INT8, on Silicon Labs EFR32xG26 MCUs. Nothing has to reach
the Pi or the Cloud before the wearer gets an alert.

### Fall direction and freezing of gait, on MCU A

<p align="center"><img src="assets/slide-training.jpg" alt="Training pipeline: UCI, UMAFall and UP-Fall datasets for falls, FoG-STAR for freezing of gait; wrist and ankle IMU at 25 Hz, 64-sample windows with stride 16, 1,122 handcrafted features, LightGBM plus TreeSHAP ranking, a fixed Shared-256 feature set, temporal input of shape B by K by 256, then a binary FoG head and a 4-class fall-direction head" /></p>

- **Data.** Falls from **UCI, UMAFall and UP-Fall**; freezing of gait from **FoG-STAR**. Wrist and ankle
  IMUs are synchronised at **25 Hz**.
- **Features you can explain.** Each 2.56 s window (64 samples, hop 0.64 s) becomes **1,122
  UCI-HAR-style features**. **LightGBM + TreeSHAP** ranks them across both tasks, and the top
  **256** become one fixed, ordered feature contract shared by training and firmware.
- **One model, two heads.** A **depthwise-separable temporal convolutional network (DS-TCN)** reads the
  last 10 windows (`[B, 10, 256]`): three dilated depthwise blocks (d = 1, 2, 4) with LayerNorm, GELU and
  residuals, then a **freezing-of-gait** head (sigmoid, binary, scored on PR-AUC) and a
  **fall-direction** head (softmax: no fall, forward, backward, lateral; scored on macro-F1).

<p align="center"><img src="assets/slide-dstcn.jpg" alt="DS-TCN architecture: input of 10 windows by 256 features, linear projection to 64, three depthwise 1D convolution blocks with dilation 1, 2 and 4, then a fall/direction head with 4-way softmax and a freezing-of-gait head with a sigmoid and a 0.4 threshold" /></p>

### Running it on the MVP accelerator

The EFR32xG26 has a **Matrix Vector Processor (MVP)** next to its Cortex-M33. TensorFlow Lite Micro
keeps control of the graph; the supported kernels (fully connected, conv, depthwise conv, add, mul)
are offloaded to the MVP, and everything else falls back to CMSIS-NN on the CPU.

<p align="center"><img src="assets/slide-mvp.jpg" alt="Measured on a real xG26 over 100 runs: 236.3 ms CPU-only versus 191.6 ms with partial MVP offload, 18.89% lower latency, 1.233× speedup, 23.29% more throughput, inference uses 29.94% of the 640 ms window, leaving 448.4 ms of headroom" /></p>

| Measured on a real xG26, 100 runs, same INT8 model | |
| :--- | ---: |
| CPU only | 236.3 ms |
| Partial MVP offload | **191.6 ms** (1.23× faster) |
| Share of each 640 ms window | **29.9 %**, leaving 448 ms of headroom |

### "Help", "good" and coughs, on MCU B

A **TENet12** keyword model (a small temporal-efficient CNN, INT8) listens on MCU B's microphone for four
classes: **help** (distress), **good** (all fine), **cough**, and **unknown** for everything else.
It was trained on English keywords from the Multilingual Spoken Words Corpus (4,437 "help" and
9,711 "good" clips), **COUGHVID** (EPFL, 30k+ recordings), and Silicon Labs MLTK's background speech for
"unknown". A spoken "help" goes out as an SOS.

<p align="center"><img src="assets/slide-tenet.jpg" alt="TENet12 architecture: a 98 by 104 INT8 spectrogram input, a convolutional stem and three residual stages of depthwise convolutions, classifying help, good, cough and unknown" /></p>

<br />

## 💊 The dispenser

Eight cups in two layers, one shared pickup cup at the front.

<p align="center"><img src="assets/slide-dispenser-parts.jpg" alt="The dispensing mechanism laid out: the cup, a rotating disc sized to one pill, a sweeper arm, an agitator piece and a motor coupler, next to the assembled two-layer Station with its tablet" /></p>

Each cup is a small 3D-printed pill feeder. A motor turns a **rotating disc** whose pocket is cut to the
thickness of that pill, so it carries exactly one pill at a time to the drop hole. A **sweeper arm**
blocks any extra pill riding on top, and an **agitator** stirs the stack so pills keep flowing instead
of bridging and jamming.

```mermaid
flowchart LR
    API["station-api"] -- HTTP --> D["medication-dispenser<br/>(Pi)"]
    D -- "USB serial<br/>motor_start / motor_stop" --> L1["ESP32 · layer 1<br/>cups 1–4 · 2 × L298N"]
    D -- "USB serial" --> L2["ESP32 · layer 2<br/>cups 5–8 · 2 × L298N"]
    IR["8 × through-beam IR<br/>one per cup"] -- GPIO --> D
    CUP["Pickup-cup IR"] -- GPIO --> D
    D -- "SPI0" --> LED["2 × WS2812B strips<br/>blue · amber · green"]
```

- **The ESP32s only turn motors.** Each one gets `motor_start` / `motor_stop` and runs a forward-back
  jog between them, so pills don't jam in the cup.
- **The Pi counts.** All nine IR sensors are wired straight to the Pi's GPIO. A background thread
  debounces each beam, counts pills per cup, and stops that cup's motor at the right count, or after
  a jam timeout with no new pill.
- **Every cup runs at once.** A dose of three medications turns three motors in parallel, across both
  layers, each stopping on its own count.
- **Did they actually take it?** After a dispense, the pickup-cup sensor arms. Lift the cup and the
  Station logs `medication.cup_removed`; leave it and it raises `medication.missed`, a P1 alert to the
  caregiver.
- **Tunable live.** Jog timing and motor power are set from a PIN-gated Control tab and applied on the
  next dispense, no restart. A set of bench scripts (identify sensors, identify motors, check
  direction, tune jog) made bring-up repeatable.

### Who gets pills, and when

```mermaid
sequenceDiagram
    autonumber
    participant P as Patient
    participant K as Kiosk
    participant S as station-api
    participant D as Dispenser
    participant C as Cloud
    P->>K: stands in front of the Station
    K->>K: FaceID in the browser (or PIN)
    K->>S: identity + request dose
    S->>S: re-checks the face match<br/>finds a dose due within ±30 min, not yet taken
    S->>D: one request, every cup in the dose
    D-->>S: per-cup result (pills counted)
    S->>S: dispense log + medication.taken in the outbox
    S-->>K: SSE: dose taken, LED green
    S-)C: sync when online (same event ID)
    Note over D: pickup-cup sensor armed:<br/>lifted → cup_removed · timeout → missed
```

<br />

## 🖥️ The Station kiosk

A touch screen on the Station, designed for an older adult from across the room: big type, one thing
per tab, and the next dose always visible.

<p align="center"><img src="assets/kiosk.png" alt="The P-Station kiosk home screen: weather, today's pills, the time and a family photo frame" /></p>
<p align="center"><sub>"Your day": weather, today's pills, the clock and a family photo frame, readable from across the room.</sub></p>

| Tab | What's on it |
| :--- | :--- |
| **Your day** | Clock, weather, today's pills, to-do list and a family photo |
| **Pills** | Each medication's schedule and stock, adherence, which cup holds what |
| **Photos** | A full-screen memory frame, with the time and next dose kept quiet in the corners |
| **Music** | A large-target player for the radio and old records |
| **Wearables** | Wrist and ankle battery, an ON/OFF mobility strip against dose times, fall detection status |
| **Settings** | Users, FaceID enrolment, sound, Control tab (PIN-gated: manual dispense, jog tuning, emergency stop) |

When a dose comes due, a full-screen alarm takes over, and the same reminder is pushed down to the
wristband over BLE so the patient feels it on the wrist too.

<br />

## 📱 The caregiver app

- **Onboarding**: create a patient, pair the Station by its device code, pick the wristband from a live
  Bluetooth radar of what the Station can see, record consent, enrol FaceID
- **Prescription to plan**: photograph a prescription; **Tesseract OCR** (Vietnamese + English) reads
  it and a text LLM structures it into an editable draft. Nothing is activated until a caregiver checks
  every line and assigns a cup
- **Live overview**: a **3D patient digital twin** (three.js) with the wrist and ankle sensors anchored
  on it, a movement safety dashboard, and realtime events as they happen
- **Alerts first**: fall and SOS jump to the top across both the Station and the caregiver app
- **Assistant**: answers questions about the patient's own logged data, scoped to that patient

```mermaid
flowchart LR
    PH["📷 Prescription photo"] --> OCR["Tesseract OCR<br/>vie + eng"]
    OCR --> LLM["Text LLM<br/>→ editable draft"]
    LLM --> REV["Caregiver reviews<br/>every line + picks cups"]
    REV --> PLAN["Plan version N<br/>immutable · checksum"]
    PLAN --> JOB["Sync job"]
    JOB --> PI["Station applies in one<br/>transaction, then ACKs"]
```

<br />

## 🔁 How an event travels

From a possible freeze on the wrist to a caregiver's screen:

```mermaid
sequenceDiagram
    participant A as Wrist MCU A
    participant B as Wrist MCU B
    participant I as ble-ingestor (Pi)
    participant S as station-api (Pi)
    participant W as sync worker (Pi)
    participant C as cloud-api
    participant G as Caregiver app
    A->>A: model flags a possible freeze → buzzer
    A->>B: UART event
    B->>I: BLE notify, 12 bytes
    I->>S: decoded event + patient ID + UUID
    S->>S: commit: event + outbox row
    S-->>S: kiosk SSE (no Internet needed)
    W->>C: batch of up to 100 events
    C->>C: dedupe by event ID, store, raise alert
    C-->>G: SSE: live alert
    C-->>W: accepted / duplicate / rejected
```

- **Written down first.** Nothing counts as received until it's in the Station's PostgreSQL. If the
  Internet drops, events wait in the outbox.
- **Retries are safe.** Every event carries one UUID for life; the Cloud rejects duplicates, so a retry
  never creates a second fall.
- **Config flows the other way the same way.** Patient profiles, face descriptors and medication plans
  go down as versioned, checksummed sync jobs; the Station applies each in one transaction and only
  then ACKs.

<br />

## 🔧 Problems that took the most iterations

<details open>
<summary><b>Who counts the pills: the ESP32 or the Pi?</b></summary>
<br />

The first rig had each ESP32 read its own four IR sensors, count pills and decide when to stop. It
worked on the bench, but every tuning change meant reflashing two boards, and a miscount was invisible
to the Pi until the dispense was over.

So the split moved: **the ESP32s only turn motors**, and all IR sensors moved to the Pi's GPIO. The
Pi now owns debounce, counting and jam detection in one place, the HTTP contract to the rest of the
Station didn't change, and tuning became a config change instead of a firmware build.

The move came with its own lessons: a **common ground across everything** (Pi, both 12 V motor
supplies, all eight sensor rails), or the sensor lines float and read noise; a **voltage divider** on
each 5 V sensor before it touches a 3.3 V Pi pin; and **measuring each sensor's polarity one by one**,
because they weren't all the same.

</details>

<details>
<summary><b>LEDs on a Raspberry Pi 5</b></summary>
<br />

The usual `rpi_ws281x` library drives WS2812B through PWM and DMA via `/dev/mem`, which doesn't work
on the Pi 5's new RP1 chip. The strips are driven over **SPI0's MOSI line** instead. Two strips sit on
either side of the chute, Y-split from the same data pin, so they mirror each other: the pixel count
is 10, not 20, which only showed up on the bench when half of each strip stayed dark.

</details>

<details>
<summary><b>One wristband, the right patient</b></summary>
<br />

BLE packets carry no patient ID by design. The Cloud is the only source of truth for which wrist
belongs to whom, versioned and synced to the Pi before it connects. Dose reminders going *down* to
the wrist are checked twice: the command records the exact wrist it was meant for, and the BLE writer
re-checks the assignment right before writing. A reminder queued for a wrist that has since been
unpaired is dropped, never delivered to the new one.

</details>

<details>
<summary><b>Reading a prescription without freezing the app</b></summary>
<br />

The first version sent the photo to a vision model inside the request. It was slow, hit rate limits,
and froze the API while it waited. Reading now runs in a **background worker**: local Tesseract OCR
(no network, no per-call cost), then one small text-only LLM call to structure it. If the LLM is
unavailable, the caregiver still gets the OCR text to type from. Uploads also go **straight to the
API with a short-lived ticket**, after a proxy in the middle was found dropping 2 MB photos mid-transfer.

</details>

<details>
<summary><b>A demo venue with no reliable Internet</b></summary>
<br />

The whole point is that the home keeps working offline, but the *caregiver* side needs the Cloud. For
the live demo, the team built a **LAN-only Cloud** that runs on the local network, plus two scripts
that switch the Station between production and LAN demo without hand-editing config mid-demo.

</details>

<br />

## 🗓️ How it was built

Four months, from a pitch in May to the Grand Final on 18 September.

| When | Stage |
| :--- | :--- |
| **Month 1** | Wearable hardware MVP on Silicon Labs dev kits; fall and FoG dataset collection |
| **Month 2** | Fall / FoG and voice models trained; first wearable firmware; initial Pi station |
| **Month 3** | A fully working Raspberry Pi Station: BLE gateway, dispenser, kiosk, offline database |
| **Month 3 – 4** | Wearable, Station and Cloud joined end to end; caregiver app, pairing, realtime alerts |
| **Month 4** | Custom wristband and ankle PCBs, dispenser bring-up on real hardware, the 3D patient twin, prescription reading |
| **Final weeks** | Debugging on the real rig, the LAN-only demo fallback, rehearsing the full demo |

<br />

## 🧰 Stack

| Layer | Stack |
| :--- | :--- |
| **Wearable** | 2 × Silicon Labs EFR32xG26 (BRD2608A), BGM220 ankle node, Simplicity SDK, ICM-40627 IMU, GC9A01 round TFT, I²S mic, custom PCBs |
| **Edge AI** | LightGBM + TreeSHAP feature selection, DS-TCN (fall direction + FoG), TENet12 (keywords + cough), full-INT8 TensorFlow Lite Micro, MVP accelerator, Silicon Labs MLTK |
| **Dispenser** | 2 × ESP32 (PlatformIO, C), 4 × L298N, 8 DC motors, 9 IR sensors, 2 × WS2812B strips |
| **Station** | Raspberry Pi 5, Docker Compose, FastAPI, PostgreSQL, Redis (AOF), Bleak (BLE), Next.js kiosk, face-api.js |
| **Cloud** | FastAPI, PostgreSQL + Alembic, Redis, background worker, SSE, Tesseract OCR + an LLM via OpenRouter |
| **Caregiver app** | Next.js 15, React 19, three.js / React Three Fiber, Recharts, face-api.js |
| **Security** | HttpOnly JWT cookies with rotating refresh, per-patient access roles, hashed station tokens, encrypted face descriptors (no face images stored), short-lived SSE tickets |

<br />

<div align="center">

| 👥 4 people | 🧱 3 tiers | 🔌 6 boards | 💊 8 cups |
| :---: | :---: | :---: | :---: |
| **~17k** lines of Python | **~14k** lines of TypeScript | **38** test files | **0** real patient data |

</div>

<br />

---

<div align="center">

**[Bảo Trương](https://github.com/baotrq)** · with Đặng Như Phước, Huỳnh Trọng Khiêm and Hồ Minh Thao · Team MLIoT – Edgelectronix · FPT IoT Challenge 2026

</div>
