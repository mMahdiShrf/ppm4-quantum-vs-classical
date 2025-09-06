# PPM-4 Error Probability — Classical Photon Counting vs Quantum SRM

This repo compares symbol-error probability \(P_e\) for **4-slot pulse-position modulation (PPM-4)** using two receivers:
1) a **classical photon-counting** detector, and  
2) the **quantum square-root measurement (SRM)** detector.

The code sweeps signal energy \(N_s\) (photons) across several background noise levels \(N\) (photons/slot) and generates plots/data that show the gap between classical and quantum detection.

---

## What’s here

- **Scripts** to compute \(P_e\) for classical and SRM receivers.
- **Figures** that visualize \(P_e\) vs \(N_s\) for multiple \(N\) values.
- **Saved data** (e.g., `.npy`/`.csv`) for downstream analysis.

Typical outputs (filenames may vary depending on your scripts):
- `figs/classical_pe.png` — classical photon-counting error curves  
- `figs/srm_pe.png` — quantum SRM error curves  
- `figs/compare.png` — overlay (classical vs SRM)

---

## Quick start

```bash
# (optional) create a virtual environment
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

# install basics
pip install numpy scipy matplotlib
