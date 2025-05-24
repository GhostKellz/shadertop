# 🧵 ShaderTop

[![Zig](https://img.shields.io/badge/Built_with-Zig-orange?style=flat-square\&logo=zig)](https://ziglang.org)

A blazing-fast GPU utilization monitor for Linux — written in Zig for the GhostKellz homelab stack. Designed for Wayland/NVIDIA users who want a clean, headless-friendly GPU dashboard.

---

## 📊 What it does

`shadertop` reads from `/sys/class/drm/` or NVIDIA-specific telemetry and prints:

```
GPU0 [GeForce RTX 4090] ▓▓▓▓▓▓▓▓▓░░░░ 72% | 62°C
GPU1 [NVIDIA A6000]    ▓▓▓░░░░░░░░░░ 28% | 45°C
```

* Works over SSH
* Detects multiple GPUs
* Designed to integrate into `ghostctl monitor` or `ghostctl sys`

---

## 🚀 Usage

```bash
zig build run
```

Or if compiled:

```bash
./shadertop
```

---

## ⚙️ Features (Planned)

* [ ] NVIDIA + AMD GPU support
* [ ] TUI dashboard using `zig-tui` or `crossterm`
* [ ] Temperature, usage, fan speeds
* [ ] Integrated clipboard/export to JSON
* [ ] Remote mode over SSH (serial output)

---

## 🧠 Name ideas

Still deciding — some candidates:

| Name         | Notes                       |
| ------------ | --------------------------- |
| `shadertop`  | Shader activity + `top`     |
| `nvtop-zig`  | Like `nvtop` but Zig-native |
| `ectogpu`    | Ghosty + GPU                |
| `ghostdraw`  | Ghost + GPU draw monitoring |
| `spectractl` | Ghost spectrum stats CLI    |

---

© 2025 [GhostKellz](https://ghostkellz.sh) / CK Technology — MIT License
