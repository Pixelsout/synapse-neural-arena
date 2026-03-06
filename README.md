<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=gradient&customColorList=0,2,2,5,30&height=200&section=header&text=SYNAPSE&fontSize=90&fontColor=00ffff&animation=fadeIn&fontAlignY=55&desc=NEURAL%20COMBAT%20ARENA&descAlignY=80&descSize=22&descColor=ff00aa" width="100%"/>

<br/>

[![Live Demo](https://img.shields.io/badge/▶%20LIVE%20DEMO-Play%20Now-00ffff?style=for-the-badge&labelColor=020408)](https://pixelsout.github.io/synapse-neural-arena/)
[![GitHub](https://img.shields.io/badge/GitHub-Pixelsout-ff00aa?style=for-the-badge&logo=github&labelColor=020408)](https://github.com/Pixelsout/synapse-neural-arena)
[![TensorFlow.js](https://img.shields.io/badge/TensorFlow.js-4.15-ff6600?style=for-the-badge&logo=tensorflow&labelColor=020408)](https://www.tensorflow.org/js)
[![No Install](https://img.shields.io/badge/Zero%20Install-Single%20HTML%20File-aaff00?style=for-the-badge&labelColor=020408)](https://pixelsout.github.io/synapse-neural-arena/)
[![Stars](https://img.shields.io/github/stars/Pixelsout/synapse-neural-arena?style=for-the-badge&color=ffd700&labelColor=020408&logo=github)](https://github.com/Pixelsout/synapse-neural-arena)

<br/>

> *A cyberpunk arcade experience powered by a **real Convolutional Neural Network** —*
> *trained live in your browser, every single time you load the page.*

</div>

---

## ⚡ What Is This?

SYNAPSE is a **gamified neural network visualizer** built as a single HTML file. You draw a digit (0–9) or letter (A–Z) on a canvas, hit **FIRE**, and watch a real CNN process your drawing layer by layer — showing every activation map, every neuron firing, and every probability score in real time.

**No backend. No server. No install. Just open it and play.**

---

## 🔴 Live Demo

<div align="center">

### **[▶ https://pixelsout.github.io/synapse-neural-arena/](https://pixelsout.github.io/synapse-neural-arena/)**

[![Open in Browser](https://img.shields.io/badge/Open%20in%20Browser-Chrome%20%2F%20Edge%20recommended-00ffff?style=flat-square&labelColor=020408)](https://pixelsout.github.io/synapse-neural-arena/)
[![Train Time](https://img.shields.io/badge/Boot%20Time-~15%20seconds%20CNN%20training-aaff00?style=flat-square&labelColor=020408)]()
[![Characters](https://img.shields.io/badge/Recognizes-0--9%20%2B%20A--Z%20%3D%2036%20classes-ff00aa?style=flat-square&labelColor=020408)]()

</div>

---

## 🧠 How The Neural Network Works

<div align="center">

```
  Your Drawing (280×280px)
          │
          ▼
    Scaled to 28×28
          │
          ▼
    Normalized [0,1]
          │
          ▼
┌─────────────────────────────────────────────────────────────────┐
│                 CONVOLUTIONAL NEURAL NETWORK                    │
│                                                                 │
│  ┌───────┐    ┌────────────┐    ┌──────────┐    ┌──────────┐  │
│  │ INPUT │───▶│ CONV2D(32) │───▶│ MAXPOOL  │───▶│CONV2D(64)│  │
│  │28×28×1│    │   +ReLU    │    │  /2 /2   │    │  +ReLU   │  │
│  └───────┘    └────────────┘    └──────────┘    └──────────┘  │
│                                                       │         │
│   ┌──────────┐    ┌──────────────┐    ┌──────────────▼──┐     │
│   │SOFTMAX   │◀───│  DENSE(128)  │◀───│    FLATTEN      │     │
│   │ 36 class │    │    +ReLU     │    │   + MaxPool     │     │
│   └────┬─────┘    └──────────────┘    └─────────────────┘     │
│        │                                                        │
└────────┼───────────────────────────────────────────────────────┘
         │
         ▼
  TOP PREDICTION + CONFIDENCE SCORE
```

</div>

Each layer is **visualized live** as your drawing passes through:

| Stage | What You See |
|:---:|:---|
| 📥 Input | Your raw 28×28 pixel grid |
| 🔷 Conv Layer 1 | 32 feature maps — edge and stroke detectors |
| 🔶 Conv Layer 2 | 64 feature maps — complex pattern combinations |
| 🔵 Dense Layer | Animated neuron graph with weighted glowing connections |
| 🎯 Output | Probability bars for all 36 classes, top 5 ranked |

---

## 🎮 Features

<div align="center">

| 🧠 Neural Network | 👁️ Visualization | 🕹️ Game System |
|:---|:---|:---|
| Real CNN via TensorFlow.js | 5-stage pipeline view | Score + 10x combo multiplier |
| Conv2D → MaxPool → Conv2D | 96 feature maps (magma colormap) | XP bar + accuracy tracking |
| Dense(128,ReLU) + Softmax | Hover any map to zoom | FREE & CHALLENGE modes |
| Trained fresh on every load | Animated dense neuron graph | Timed rounds + countdown bar |
| 2,880 procedural samples | Real-time probability display | Streak history (last 10 rounds) |
| Async — page never freezes | Live layer activation canvases | 💥 Particle explosion on hits |

</div>

---

## ✨ Visual Effects

<div align="center">

![CRT](https://img.shields.io/badge/CRT-Scanlines%20%2B%20Vignette-00ffff?style=flat-square&labelColor=020408)
![Glitch](https://img.shields.io/badge/CSS-Glitch%20Title%20Animation-ff00aa?style=flat-square&labelColor=020408)
![Particles](https://img.shields.io/badge/Canvas-Ambient%20Particle%20Drift-aaff00?style=flat-square&labelColor=020408)
![Brush](https://img.shields.io/badge/Drawing-Neon%20Brush%20Glow-00ffff?style=flat-square&labelColor=020408)
![Burst](https://img.shields.io/badge/FX-Particle%20Burst%20Explosions-ff6600?style=flat-square&labelColor=020408)
![Score](https://img.shields.io/badge/FX-Floating%20Score%20Text-ffd700?style=flat-square&labelColor=020408)
![Combo](https://img.shields.io/badge/COMBO-DOUBLE!%20TRIPLE!%20GODLIKE!-ff00aa?style=flat-square&labelColor=020408)
![Boot](https://img.shields.io/badge/Boot-Live%20Training%20Progress%20Screen-aaff00?style=flat-square&labelColor=020408)

</div>

---

## 🗂️ Tech Stack

<div align="center">

| Technology | Role |
|:---|:---|
| ![TensorFlow.js](https://img.shields.io/badge/TensorFlow.js-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) | CNN model build, train, inference, intermediate layer extraction |
| ![HTML5](https://img.shields.io/badge/HTML5_Canvas-E34F26?style=flat-square&logo=html5&logoColor=white) | Drawing pad, pixel preview, all visualization rendering |
| ![JavaScript](https://img.shields.io/badge/Vanilla_JS-F7DF1E?style=flat-square&logo=javascript&logoColor=black) | Game logic, particle engine, animation loops |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) | Cyberpunk UI, glitch effects, CRT scanlines, neon glow |
| ![Google Fonts](https://img.shields.io/badge/Google_Fonts-4285F4?style=flat-square&logo=google&logoColor=white) | Audiowide (display) · VT323 (retro) · Rajdhani (body) |

**Zero framework dependencies.** No React. No Vue. No bundler. No Node runtime. One `.html` file.

</div>

---

## 🚀 Run Locally

**Option 1 — VS Code Live Server (recommended)**

```bash
# 1. Install VS Code → https://code.visualstudio.com/
# 2. Install "Live Server" extension by Ritwick Dey
# 3. Open index.html in VS Code
# 4. Click "Go Live" in the bottom status bar
# Opens at → http://127.0.0.1:5500
```

**Option 2 — Python**
```bash
python -m http.server 5500
```

**Option 3 — Node.js**
```bash
npx serve .
```

> ⚠️ **Never open via `file://`** — TensorFlow.js requires an HTTP context to load correctly.

---

## ⌨️ Keyboard Shortcuts

<div align="center">

| Key | Action |
|:---:|:---|
| `Space` | ⚡ Fire — run recognition |
| `C` | 🗑️ Clear the canvas |
| `N` | ▶ Start a new round |

</div>

---

## 🎯 Tips for Best Accuracy

```
✅  Draw LARGE and CENTERED — fill most of the canvas
✅  Use THICK strokes — model was trained on bold geometric shapes
✅  Digits 0–9 score higher confidence than letters
✅  Exaggerate distinctive features (tail on Q, crossbar on A, curve on C)
✅  Challenge mode — speed + accuracy = max combo multiplier
❌  Don't draw tiny or in a corner
❌  Don't use cursive or highly stylized handwriting
```

---

## 📁 Project Structure

```
synapse-neural-arena/
└── index.html                  ← Entire project. One file. ~1900 lines.
    │
    ├── 🎨  CSS                  Cyberpunk UI, CRT scanlines, neon glow, all animations
    ├── ✨  Particle System       Canvas burst, spark, floating text, ambient drift
    ├── 🖊️   Drawing Canvas       Mouse + touch input with neon brush glow effect
    ├── 🧠  CNN Model            TensorFlow.js architecture + chunked async training
    ├── 📊  Data Generator       Procedural character image synthesis (36 classes × 80)
    ├── 👁️   Visualizer           Pipeline view, feature maps, dense layer animator
    └── 🕹️   Game Engine          Score, XP, combo, challenge mode, event ticker
```

---

## 🌐 Browser Support

<div align="center">

| Browser | Status | Notes |
|:---:|:---:|:---|
| ![Chrome](https://img.shields.io/badge/Chrome_90+-4285F4?style=flat-square&logo=googlechrome&logoColor=white) | ✅ **Recommended** | Best WebGL + WASM performance |
| ![Edge](https://img.shields.io/badge/Edge_90+-0078D7?style=flat-square&logo=microsoftedge&logoColor=white) | ✅ Full support | — |
| ![Firefox](https://img.shields.io/badge/Firefox_88+-FF7139?style=flat-square&logo=firefox&logoColor=white) | ✅ Works | Slightly slower training |
| ![Safari](https://img.shields.io/badge/Safari_15+-000000?style=flat-square&logo=safari&logoColor=white) | ⚠️ Works | WebGL may be slower |
| ![Mobile](https://img.shields.io/badge/Mobile_Chrome-34A853?style=flat-square&logo=android&logoColor=white) | ✅ Touch support | Draw with your finger |

</div>

---

## ⚠️ Known Limitations

- Trained on **synthetic geometric strokes**, not real handwriting (MNIST/EMNIST) — works best with clean, deliberate drawing
- Visually similar pairs may be confused: `0 ↔ O` · `1 ↔ I` · `5 ↔ S` — exaggerate differences when drawing
- Model retrains from scratch on every page load — no persistent saved weights

---

## 👤 Author

<div align="center">

Built by **[Pixelsout](https://github.com/Pixelsout)**

[![GitHub followers](https://img.shields.io/github/followers/Pixelsout?label=Follow%20on%20GitHub&style=for-the-badge&logo=github&labelColor=020408&color=ff00aa)](https://github.com/Pixelsout)
[![GitHub stars](https://img.shields.io/github/stars/Pixelsout/synapse-neural-arena?style=for-the-badge&logo=github&labelColor=020408&color=ffd700&label=Star%20this%20repo)](https://github.com/Pixelsout/synapse-neural-arena)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=100&section=footer&animation=fadeIn&text=Draw.%20Fire.%20Watch%20the%20neural%20network%20think.&fontSize=16&fontColor=00ffff&fontAlignY=65" width="100%"/>

</div>
