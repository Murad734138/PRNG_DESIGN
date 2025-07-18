# PRNG_DESIGN


# Custom Pseudorandom Number Generator (PRNG)

This project implements and analyzes a custom **Linear Congruential Generator (LCG)** to simulate pseudorandom numbers and compares it with NumPy’s built-in uniform generator.

## PRNG Logic

We use the standard LCG formula:

    Xₙ₊₁ = (a * Xₙ + c) mod m

Normalized to the range [0, 1) using:

    X_normalized = Xₙ / m

### Parameters used:
- `modulus (m)` = 2³¹
- `multiplier (a)` = 1103515245
- `increment (c)` = 12345
- `seed` = 42

##  Visualizations

Two types of analysis are done:

1. **Scatter Plot** – Visualizes dependency and clustering.
2. **Histogram** – Examines distribution shape and uniformity.

##  Requirements

Install required packages:

```bash
pip install numpy matplotlib
```

##  Usage

Run the script:

```bash
python prng.py
```

##  Output

The script outputs:
- Two plots
- Console statistics of distributions

##  Analysis

LCG shows uniformity but may exhibit subtle patterns or dependencies compared to cryptographically secure PRNGs. Histograms help visualize its bias or deviation.

##  References

- NumPy PRNG Documentation

---

© 2025 by Muraduzzaman Asha
