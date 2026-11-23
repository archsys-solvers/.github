<div align="center">

# ArchSys Solvers

**High-Performance Cache-Aware Computing & Hardware-Conscious Scientific Solvers**

[![Language](https://img.shields.io/badge/Language-C%2B%2B17-00599C?logo=c%2B%2B&logoColor=white)](https://en.cppreference.com/w/cpp/17)
[![Architectures](https://img.shields.io/badge/Architectures-x86--64%20%7C%20ARM64%20%7C%20RISC--V-0969da)](#)
[![Vectorization](https://img.shields.io/badge/SIMD-AVX--512%20%7C%20AVX2%20%7C%20NEON-7a3e9d)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-2ea44f.svg)](https://opensource.org/licenses/MIT)

<p align="center">
  <em>Bridging algorithmic mathematical computing and silicon memory hierarchies through Data-Oriented Design (DOD).</em>
</p>

</div>

---

### Scientific Philosophy & Mission

Modern CPU microarchitectures spend the vast majority of their energy and execution cycles stalled on memory retrieval (the **Memory Wall**). While classic Object-Oriented Programming (OOP) groups heterogeneous attributes into individual objects (Array-of-Structures, AoS), modern cache hierarchies demand continuous, contiguous streaming of homogeneous data (Structure-of-Arrays, SoA).

**ArchSys Solvers** investigates, engineers, and publishes zero-overhead computational frameworks engineered from the silicon up:

```
[ Traditional AoS Layout - Cache Stalled ]
| Pos.X | Pos.Y | Pos.Z | Mass | Temp | Pressure |  --> High Cache Pollution & Scatter

[ Data-Oriented SoA Layout - Hardware Streamed ]
| Pos.X | Pos.X | Pos.X | Pos.X | Pos.X | Pos.X |  --> 100% Cache Utilization & SIMD
```

---

### Core Research & Engineering Pillars

* **Data-Oriented Memory Transformations:** Eliminating cache-line pollution and pointer chasing through compile-time Structure-of-Arrays (SoA) layout transformations.
* **Multi-Architecture Hardware Vectorization:** Native SIMD acceleration targeting 512-bit registers (x86 AVX-512), 256-bit registers (AVX2), and 128-bit vector pipelines (ARM NEON) without runtime penalty.
* **Compile-Time Expression DSLs:** C++17 expression templates that eliminate intermediate array allocations, fusing arithmetic kernels directly into hardware vector registers.
* **Empirical Micro-Benchmarking:** Multi-platform cache analysis across L1D, private L2, and shared L3/LLC cache boundaries.

---

### Flagship Software

| Repository | Focus | Architectures | Docs |
| :--- | :--- | :--- | :--- |
| [**data-oriented-solver**](https://github.com/archsys-solvers/data-oriented-solver) | Cache-aware scientific computing engine with SoA layout transformations and fused expression kernels | x86-64, ARM64, RISC-V | [Live Documentation](https://ahmedez-zouine.github.io/data-oriented-solver/) |

---

### Hardware Validation Testbed

All computational kernels are verified and benchmarked across dedicated bare-metal hardware platforms:

* **x86-64 AVX-512:** Intel Xeon / Core i9 (10-core / 20-thread, 19.25 MB L3 Cache, 512-bit ZMM registers)
* **Server-Grade ARM64:** Ampere Altra (Neoverse-N1, 3.0 GHz, 1 MB private L2 cache per core, Dual 128-bit NEON)
* **Client ARM64:** Apple Silicon M-series (High-bandwidth unified memory architecture)
* **RISC-V:** Multi-architecture validation and vector extension emulation

---

### Global Research Reach

<div align="center">
  <a href="https://mapmyvisitors.com/web/1c9kq" target="_blank" rel="noopener noreferrer">
    <img src="https://mapmyvisitors.com/map.png?cl=2e3a4f&w=1200&t=tt&d=DgbseS68tbhFmnePsrKjWwI4qLL6DWkohB75KvmvBLo&co=ffffff&cmo=3acc3a&cmn=ff5353&ct=1973d8" alt="Global Readership Map" width="680" style="max-width: 100%; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.08);">
  </a>
  <p><em>Visitor activity across multi-architecture computing research centers worldwide.</em></p>
</div>

---

<div align="center">
  <sub>Founded & Maintained by <a href="https://github.com/ahmedez-zouine">Ahmed EZ-ZOUINE</a> &bull; Rabat, Morocco</sub>
  <br>
  <sub>Inquiries & Scientific Collaboration: <code>ahmed.ezzouine@um5r.ac.ma</code></sub>
</div>
