# XASM – SHARP PC-E500S (SC62015)

This repository contains the **original XASM 1.40 sources** (N. Kon / E. Kako)
and **example assembly programs** for the SHARP PC-E500S.

## Contents
- `src/xasm/` – XASM sources in C (1995–1996, E. Kako)
- `examples/` – sample `.ASM` programs
- `docs/INFORMATION.txt` – original documentation

## Build
```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build --config Release
```

## License
Original XASM: (c) N. Kon & E. Kako, 1990–1996.
This repo packaging: MIT (2025).
