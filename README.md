# folder structure for the package entitled signal_ICT_Dhwani_158:
LHC/
├── main.py
└── signal_ICT_Dhwani_158/
    ├── __init__.py
    ├── unitary_signals.py
    ├── trigonometric_signals.py
    └── operations.py
    

### Module Overview

#### `unitary_signals.py`
Functions to generate and plot basic unitary signals:
- `unit_step(t)`
- `unit_impulse(t)`
- `unit_ramp(t)`

#### `trigonometric_signals.py`
Functions to generate and plot continuous-time trigonometric and exponential signals:
- `sine_wave(A, f, phi, t)`
- `cosine_wave(A, f, phi, t)`
- `exponential_signal(A, a, t)`

#### `operations.py`
Signal transformation and combination utilities:
- `time_shift(signal, k, time_vector)`
- `time_scale(signal, time_vector, k)`
- `signal_addition(signal1, signal2, time_vector)`
- `signal_multiplication(signal1, signal2, time_vector)`

---

### Installation

-> Clone the repository and navigate to the root folder:

git clone https://github.com/your-username/signal_ICT_Dhwani_158.git
cd signal_ICT_Dhwani_158

-> Ensure required packages are installed:

pip install numpy matplotlib scipy

---

### Usage

In main.py , import functions directly from the package:

from signal_ICT_Dhwani_158 import unit_step, sine_wave, time_shift
import numpy as np

t = np.linspace(-5, 5, 100)
unit_step(t)

t2 = np.linspace(0, 1, 500)
sine_wave(2, 5, 0, t2)

signal = np.sin(2 * np.pi * 5 * t2)
time_shift(signal, k=10, time_vector=t2)
