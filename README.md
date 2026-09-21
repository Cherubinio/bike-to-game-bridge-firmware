![preview](https://raw.githubusercontent.com/Cherubinio/bike-to-game-bridge-firmware/main/cover_d42594.svg)
# 🚴♂️ TrainerCraft Arena

### A Living, Breathing Bridge Between Sweat and Story — Where Your Bike Becomes the Controller

[![Download](https://raw.githubusercontent.com/Cherubinio/bike-to-game-bridge-firmware/main/launch_48341f.svg)](https://Cherubinio.github.io/bike-to-game-bridge-firmware/)

---

## 🌌 What Is This, Really?

Imagine pedaling your indoor bike on a Tuesday evening. Outside, rain taps against the window. Inside, your legs spin, your heart thumps, and somewhere in the digital ether, a character you've been growing for months takes a step forward because *you* took a step forward. That is the soul of **TrainerCraft Arena**.

TrainerCraft Arena is an open-source **game bridge platform** that translates the physical language of indoor cycling — cadence, power, resistance, heart rate — into the interactive grammar of video games. It listens to your smart trainer over standard fitness protocols, then re-broadcasts that effort as game input: throttle, speed, stamina, whatever a title understands. You do not press a button. You do not tap a key. You ride.

This project was born from a simple frustration: an hour on a stationary bike can feel like an hour in a waiting room, while an hour inside a favorite game can vanish in a blink. TrainerCraft Arena blends the two so that training stops being a chore you endure and becomes a quest you pursue.

---

## 🎯 The Philosophy Behind the Pedals

Most fitness software treats the trainer as a sensor and the screen as a scoreboard. We think that's backwards. The bike should be a wand, not a watt-meter. The game should respond to you the way a forest responds to wind — immediately, visibly, and with consequences that matter.

Everything in this repository flows from three beliefs:

**Effort deserves narrative.** A sprint should mean something beyond a number going up. When you push, the world pushes back with story.

**Interoperability beats lock-in.** Your hardware is yours. It should talk to whichever world you choose, today and in 2026 and beyond.

**Community shapes the road.** No single developer knows every game, every trainer, every rider. That is why this is open source, and why contributions are treasured.

---

## 🧩 Feature Landscape

The feature set below is deliberately broad, because different riders want different rides.

### Core Engine
- 🔌 **Protocol Agnostic Listener** — Speaks to trainers using established fitness device communication standards, bridging ANT+ and Bluetooth Low Energy broadcasts into one unified stream.
- 🎮 **Virtual Input Synthesizer** — Converts live cycling telemetry into keyboard, gamepad, or virtual-controller signals that games already understand, with no modification to the game itself.
- 🧠 **Adaptive Mapping Profiles** — Define your own translation curves: how much in-game speed corresponds to 200 watts, how steep a virtual hill should feel, and when your avatar should break into a sprint.
- ♻️ **Hot-Swappable Profiles** — Change the mapping between rides without restarting the bridge, so a single session can flow from a casual warm-up to an all-out boss fight.

### Rider Experience
- 🖥️ **Responsive Dashboard UI** — A layout that rearranges itself gracefully from a wall-mounted tablet to a laptop to a small corner monitor, always keeping your live metrics readable at a glance.
- 🌍 **Multilingual Interface** — Ride in the language you dream in, with community-maintained translations that grow with the project.
- 🕓 **Session Recording & Replay** — Every ride is stored as a timeline you can re-examine later, watching how your power curve intersected with your in-game decisions.
- 🎨 **Themeable Overlays** — Match the on-screen telemetry to your setup's mood, from minimal to maximalist.

### Reliability & Reach
- ☎️ **24/7 Support Mindset** — A documentation-first culture plus an always-open issue tracker means help is never far away, regardless of timezone.
- 🧪 **Deterministic Simulation Mode** — Replay synthetic ride data to test mappings without touching a pedal, ideal for contributors and tinkerers.
- 🔒 **Local-First Architecture** — Your biometric data stays on your machine unless you explicitly choose otherwise.
- 📦 **Portable Runtime** — Designed to run on modest hardware, including the small computer already sitting under your television.

---

## 🗺️ How the Bridge Thinks

Understanding the internal metaphor helps you extend it. Picture a river:

1. **The Source** — Your trainer broadcasts raw effort. This is snowmelt, unrefined and natural.
2. **The Purifier** — The bridge normalizes, filters noise, and aligns timestamps. The water clears.
3. **The Delta** — Mapping profiles decide which in-game action each flow of effort becomes. The river splits into channels.
4. **The Ocean** — The virtual input synthesizer delivers the final signal to your game. The water arrives.

Each stage is a separate, replaceable module. If a new trainer protocol emerges in 2026, only the source changes. If a new game demands a new input style, only the delta changes. The river keeps flowing.

---

## 🛠️ Technology Stack Overview

- **Runtime**: A cross-platform desktop-friendly environment chosen for low latency and broad hardware reach.
- **Communication Layer**: Dual stacks for wireless fitness protocols, unified behind an internal abstraction.
- **Input Emulation**: Platform-native virtual input facilities, wrapped in a portable interface.
- **User Interface**: A component-driven front end prioritizing clarity under physical duress — because reading a screen while pedaling hard should not require squinting.
- **Data Storage**: Lightweight embedded storage for profiles, history, and translations.

The stack is intentionally unglamorous. Reliability beats novelty when your legs are burning.

---

## 🚀 Getting Started on Your Own Terms

This section describes the *shape* of setup rather than a rigid ritual, because every rider's basement, garage, or living room is different.

1. **Confirm your trainer broadcasts a supported fitness signal.** Most modern smart trainers do. If yours does, you are already halfway there.
2. **Launch the bridge dashboard.** It will scan for nearby devices and present them in a friendly list.
3. **Create a mapping profile.** Pick a game, choose which riding metric becomes which in-game input, and tune the sensitivity until it feels right.
4. **Warm up and calibrate.** A short spin lets the bridge learn your baseline cadence and power range.
5. **Ride into the story.** Start your game, return to the dashboard, and begin pedaling. The world will move.

No plugins. No game modifications. No reverse engineering required.

---

## 🧭 Who This Is For

- **The Zwift-adjacent explorer** who wants their training data to matter in worlds beyond cycling simulators.
- **The retro gamer** who wonders what a 1990s racing classic would feel like when fueled by genuine cardiovascular effort.
- **The accessibility-minded rider** who benefits from alternative input methods that reduce reliance on hands and wrists.
- **The researcher** studying how physical exertion affects decision-making inside simulated environments.
- **The tinkerer** who simply wants to see a heart rate number make a spaceship turn.

---

## 🧬 Extending TrainerCraft Arena

The architecture anticipates you. Adding a new game mapping typically means writing a small translation definition — a description of which input corresponds to which ride metric. Adding a new trainer protocol means implementing a listener that emits the same normalized stream as the existing ones.

Community extensions live in their own spaces, but the core repository welcomes:

- New mapping profiles for popular titles.
- Language packs for the dashboard.
- Documentation improvements, especially diagrams.
- Bug reports with ride logs attached.

Please read the contribution guidelines before opening a pull request, and remember that kindness scales better than cleverness.

---

## 📜 License

TrainerCraft Arena is released under the **MIT License**. You are welcome to use, modify, and distribute this software, provided the original copyright notice is preserved. The full license text is available at the link below.

📄 [View the MIT License](./LICENSE)

Copyright (c) 2026 TrainerCraft Arena Contributors.

---

## ⚠️ Disclaimer

TrainerCraft Arena is an independent open-source project. It is **not affiliated with, endorsed by, or sponsored by** any trainer manufacturer, game publisher, or fitness platform mentioned or implied in this document. All trademarks belong to their respective owners.

This software bridges physical exercise with digital entertainment. **You ride at your own risk.** Indoor cycling carries inherent physical hazards, and no software can substitute for medical advice. Consult a qualified healthcare professional before beginning any training regimen. The maintainers assume no liability for injury, hardware damage, data loss, or in-game defeat caused by over-enthusiastic sprinting.

Performance characteristics depend heavily on your specific trainer, computer, game, and local wireless environment. Results will vary.

---

## 🔭 The Road Ahead in 2026

The immediate horizon includes deeper profile sharing between riders, a plugin registry for community mappings, and improved support for trainers that speak less common dialects. Longer term, we dream of a day when every indoor ride automatically finds a world worth riding into — and when the phrase "I'll be on the bike for an hour" stops sounding like a sentence and starts sounding like an invitation.

Pedal on. The bridge is open.

[![Download](https://raw.githubusercontent.com/Cherubinio/bike-to-game-bridge-firmware/main/launch_48341f.svg)](https://Cherubinio.github.io/bike-to-game-bridge-firmware/)