![preview](https://raw.githubusercontent.com/matteochristian442-ui/formant-forge/main/shot_eb0d.svg)
[![Download](https://raw.githubusercontent.com/matteochristian442-ui/formant-forge/main/setup_92a8.svg)](https://matteochristian442-ui.github.io/formant-forge/)

# 🎙️ VocalScope — The Resonance Cartographer for Voice Artists

![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)
![Rust](https://img.shields.io/badge/Language-Rust-orange.svg)
![Platform](https://img.shields.io/badge/Platform-Cross--Desktop-lightgrey.svg)
![Build](https://img.shields.io/badge/Build-Stable-brightgreen.svg)
![Accessibility](https://img.shields.io/badge/Accessibility-WCAG_2.1_AA-teal.svg)

---

## 🌋 From Raw Sound to Sculpted Silence: A New Way to See Your Voice

Every voice is a fingerprint—unique, unrepeatable, and yet, infinitely malleable. Most vocal training tools treat your voice like a waveform on a flat screen, reducing the miracle of human phonation to a series of squiggly lines. **VocalScope** takes a fundamentally different path. Imagine you are a potter, and your vocal tract is the clay. Instead of guessing where to press, VocalScope gives you a **3D topographical map** of your own resonance chambers, showing you the hills and valleys of your formant frequencies in real-time. 

This isn't just another pitch monitor. This is a **laryngeal GPS** that guides you through the treacherous terrain of vocal weight, chest-to-head transitions, and the delicate balance of vocal fold closure—all while keeping your instrument safe from the silent dangers of overexertion. Built on the blistering performance of Rust, VocalScope transforms your computer into a precision laboratory that fits in your backpack.

---

## 🧭 The Core Philosophy: Train Like a Pilot, Not a Passenger

Traditional voice training is often like driving a car blindfolded—you only know you've crashed after you feel the impact. VocalScope removes the blindfold. By visualizing the **three critical axes of vocal production** simultaneously, you become the pilot of your own instrument, making micro-adjustments with the precision of a fighter jet avionics system.

### 🗺️ The Formant Atlas: Seeing the Shape of Your Sound

Your formants are the acoustic signatures that give your voice its unique character—the reason a "warm" voice sounds different from a "bright" one. VocalScope renders these as **live, undulating 3D surfaces** rather than static charts. As you slide from a deep chesty "ah" to a light, floating "ee," you'll watch the topography shift beneath your cursor. This visual feedback loop is the single most powerful way to break out of habitual vocal ruts, particularly for accent modification specialists and dialect coaches.

### ⚖️ The Weight Gauge: Balancing Power and Release

Vocal weight isn't about volume—it's about the **density of your tone**. A heavy voice carries more mass in the vocal folds; a light voice uses only the thin edges. VocalScope's proprietary weight meter (inspired by the Estill Voice Training model) gives you a **continuous gradient scale** from "pure thyroarytenoid" to "pure cricothyroid" dominance. For singers transitioning between chest and head voice, this gauge becomes your best friend, showing you when you're skirting the edge of a break before you hear it.

### 🎯 The Pitch Compass: Beyond the Metronome

Yes, it shows your fundamental frequency. But that's like saying a telescope shows stars. VocalScope's pitch visualization is **contextual and adaptive**. It learns your comfortable tessitura (your personal "comfort zone" of pitches) and flags when you're pushing into territory that requires extra caution. The system uses a **color-temperature gradient** from cool blues (safe, relaxed) to searing reds (extremely high tension), giving you an immediate thermal reading of your vocal effort.

---

## 🛠️ The Instrument Panel: A Tour of Your New Cockpit

### 🎛️ Real-Time Spectral Waterfall
A continuously scrolling, high-resolution spectrogram that refreshes at **60 frames per second**. Unlike audio editors that use this view for analysis, VocalScope makes it a *performance tool*, with visual markers that automatically annotate vibrato cycles and vocal fry episodes as they happen.

### 📊 Formant Tracking Overlays
Customizable overlay lines for F1, F2, F3, and F4 are plotted on the main visual field. Users can set target formant positions for specific vowel sounds (loaded from international phonetic alphabet presets) and VocalScope will calculate the **Euclidean distance** between your current production and the target, scoring your proximity in real-time.

### 🛡️ The Safety Envelope Monitor
Our most cherished feature—a circular gauge that combines **pitch stability, amplitude consistency, and laryngeal closure rate** into a single "strain index." When this index approaches the yellow zone, VocalScope issues a **non-intrusive haptic fade** (screen dimming) rather than a jarring alarm. This gentle nudge helps you pull back the reins before you do damage, making it the ideal co-pilot for long practice sessions.

### 📝 Multilingual Articulation Coach
A built-in library of phoneme animations (for English, Spanish, Mandarin, and Hindi currently) shows a cross-section of the vocal tract. Watch how the tongue and lips move for specific sounds, then use the spectral display to match your own production to the gold-standard model. This is particularly potent for language learners who wish to neutralize a foreign accent.

---

## 🌐 Designed for the Global Voice Community

**24/7 Multilingual Interface** — The entire user interface has been professionally translated into **12 languages**, including RTL (right-to-left) support for Arabic and Hebrew. Localization isn't a checkbox for us—it's a commitment to making vocal science accessible to every culture that sings, speaks, or performs. Swapping languages takes a single click and the change is instant.

**Responsive UI for Every Screen Size** — Whether you're using a 13-inch ultrabook in a cramped rehearsal room or a 34-inch ultrawide monitor in a professional studio, VocalScope's layout adapts like a living organism. Drag panels, detach the spectral view, or collapse everything into a minimal mode that focuses only on the pitch compass. The interface remembers your layout preferences per project, so your setup is always exactly the way you left it.

---

## 🧰 The Command Line Companion (For the Tinkerers)

While the GUI is our proud face, the heart of VocalScope is a **powerful Rust library** that can be used as a command-line utility for batch analysis. You can feed it a folder of audio files and extract the following into a CSV report:

- Average formant frequencies per phrase
- Estimated vocal weight distribution
- Instances of under-energized (breathy) vs. over-pressurized (pressed) phonation

This makes VocalScope a hidden gem for **vocal researchers, speech-language pathologists, and data scientists** who need quantitative data for studies on voice disorders. The CLI produces a machine-readable output that adheres to JSON schema specifications, making it trivially easy to pipe into other data analysis pipelines.

---

## 🧩 The Plugin Ecosystem

VocalScope supports **custom visualization plugins** written in Rust (via a stable C-ABI interface) or Python (via a lightweight bridge). Want a visualization that plots your voice against a 3D anthropometric model of a skull? You can build it. Want to trigger a MIDI note every time you nail a target formant? There's a hook for that. The plugin system is sandboxed for safety, ensuring no system-level crashes can occur from third-party code.

---

## 🚦 Getting Started: Your First Flight Plan

### System Requirements
- **Operating System:** Windows 10/11 (x64), macOS 12+ (Monterey), or Linux (kernel 5.4+)
- **Processor:** Any modern dual-core CPU (Intel i5/AMD Ryzen 3 or equivalent)
- **Memory:** 4 GB RAM minimum; 8 GB recommended for long sessions
- **Storage:** 150 MB for installation; additional space for cached analysis files

### The Installation Ritual
For the supported platforms, we provide a **single self-contained executable** that requires no dependency installation. You download the archive specific to your operating system, extract it to a folder of your choosing, and double-click the application file. The first launch will walk you through a quick microphone calibration wizard that ensures your input levels are optimized for accurate detection.

### Your First Session
1. Connect a **quality USB microphone** (headset mics work, but condenser mics yield the best spectral detail).
2. Speak a simple vowel like "ah" for ten seconds. Watch the waterfall appear.
3. Try sliding your pitch up and down a smooth scale. Observe how the formant hills shift.
4. Click on the "Safety Envelope" icon—it will turn green when you're in a sustainable vocal posture.

---

## 📚 The VocalScope Learning Library

Mastering your voice is a marathon. That's why we include a **built-in tutorial center** with over 40 interactive lessons, ranging from "What is a Formant?" to "Advanced: Mix Belt Coordination." Each lesson is a blend of text, video (directed to external public archives), and live interactive exercises that grade your progress. The learning center tracks your improvement over weeks and displays a **progress curve** that is motivating, not shaming.

---

## 🤝 The Blue License Promise

VocalScope is released under the **MIT License**. This means you can use it for personal study, professional teaching, or even commercial voice coaching businesses. You can modify the source code to create your own bespoke version. The only expectation is that you retain the original copyright notice. We chose MIT because we believe the tools for vocal health should not be walled gardens.

---

## ❤️ Community Support: Humans Behind the Microphones

We maintain a **support portal** with 24/7 coverage from our small but passionate team. While automated systems handle initial triage, every single ticket is routed to a real person with actual voice training knowledge—not just a scripted response bot. We do not use "pay-to-play" priority systems; every question, from the beginner's "Why is my waveform empty?" to the expert's "How do I parse the JSON schema?" receives equal attention.

### 🌍 Regional Forums
Dedicated sub-forums for specific voice styles (Belt, Classical, Operatic, Speech Pathology, Transgender Voice Feminization/Masculinization) allow users to share custom formant targets and tips. These forums are moderated for respectful, science-based discussion.

---

## 🧪 Advanced Diagnostics for the Fearless

For those who want to dive into raw data, the **Diagnostic Exporter** function creates a compressed `.vscope` file containing all the session data, plus a timestamped playback of the 3D visualization. This is invaluable when collaborating with a remote vocal coach who can then load the file and "rewatch" your practice session as if they were in the room with you.

---

## 🛑 Disclaimer: The Instrument Is You

VocalScope is a **visualization and feedback tool**. It is not a medical device, and it does not diagnose, treat, or cure any medical condition, including but not limited to vocal nodules, polyps, paralysis, or muscle tension dysphonia. The "Safety Envelope Monitor" is an algorithmic approximation based on biomechanical models; it cannot perceive physical pain. 

**Always practice under the guidance of a qualified professional** if you are recovering from an injury, experience persistent pain while phonating, or are under the care of an Ear, Nose, and Throat specialist. The creators of VocalScope assume no liability for injuries sustained while using this software, as training decisions ultimately rest with the user. By using VocalScope, you acknowledge that you are responsible for your own physical well-being.

---

## 🔮 The Roadmap: Where We're Soaring Next (2026)

We are actively developing **VocalScope 2.0** for release later in 2026. The vision includes:

- **Cross-Platform Mobile Companion:** A stripped-down version for iOS/Android for warm-ups on the go, syncing data to the desktop app via your personal cloud storage.
- **Real-Time Harmony Coach:** A duet mode that shows two users' formant landscapes simultaneously, plotted in shared 3D space, to find the perfect harmonic blend.
- **5G-Low-Latency Remote Coaching:** A built-in peer-to-peer connection (using WebRTC) that lets a coach see your visualization live with less than a 50ms delay, making distance coaching feel like sitting in the same studio.

---

## 🏁 Final Take on VocalScope

We built VocalScope because we fell in love with the *texture* of sound—the way a sustained note has a history, a shape, and a future. We believe that when you can *see* the physics of your own voice unfolding, the practice transforms from repetition into art. This is not merely a tool; it's a **philosophy of mindful vocal craftsmanship**.

Whether you're a shower-singer wanting to understand your range, a choir director seeking to balance sections, or a voice actor performing emotional extremes, VocalScope offers a unique lens. It asks, "What does your voice look like today?"—and then helps you redraw the picture tomorrow.

Welcome to the cartography of your own throat. 🗺️