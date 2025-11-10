# AM-USING-PYTHON
---

### Aim:

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries.

---

### Apparatus Required:

- Software: Python with Numpy and Matplotlib libraries.
- Hardware: Personal Computer.

---

### Theory:

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of the message signal. The general form of an AM signal is:

   $$ s(t) = [A_c + A_m cos(2\pi f_m t)] cos(2\pi f_c t)$$

---

### Algorithm:

1. Initialize Parameters: Set the values for carrier frequency, message frequency and sampling frequency.
2. Generate Time Axis: Create a time vector for a signal duration.
3. Generate Message Signal: Define the message signal as a cosine wave.
4. Generate Carrier Signal: Define the carrier signal as a cosine wave.
5. Plot the Signals: Use Matplotlib to plot the message signal, carrier  signal and modulated signal.

---

### Program:

```py
import numpy as np
import matplotlib.pyplot as plt
Am=6.5
fm=504
Ac=13
fc=5040
fs=50400
t= np.arange(0, 3/fm, 1/fs)

m=Am*np.cos(2*3.14*fm*t)
plt.subplot(3,1,1)
plt.plot(t,m)

c=Ac*np.cos(2*3.14*fc*t)
plt.subplot(3,1,2)
plt.plot(t,c)

s=(Ac+m)*np.cos(2*3.14*fc*t)
plt.subplot(3,1,3)
plt.plot(t,s)
```

---

### Output Waveform:

<img width="557" height="413" alt="am" src="https://github.com/user-attachments/assets/d716440b-bbbc-4ad5-a76a-479655683cf4" />


---

### Tabular Column:

<img width="1377" height="798" alt="image" src="https://github.com/user-attachments/assets/04501c7c-5191-49e0-ac34-e5fe6aabd3cb" />

---

### Result:

The message signal, carrier signal and amplitude modulated (AM) signal will be displayed in separate plots. Thus AM is implemented using numPy and Matplotlib.
