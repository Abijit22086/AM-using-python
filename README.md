# AM-using-python

# Aim:

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries. Apparatus Required
Software: Python with NumPy and Matplotlib libraries

# Apparatus:

Hardware: Personal Computer

# Theory

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of the message signal. The general form of an AM signal is:
<img width="368" height="266" alt="image" src="https://github.com/user-attachments/assets/9a556d06-da9c-4586-93bb-53101452288f" />



# Algorithm:

1.Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency.
2.Generate Time Axis: Create a time vector for the signal duration.
3.Generate Message Signal: Define the message signal as a cosine wave.
4.Generate Carrier Signal: Define the carrier signal as a cosine wave.
5.Modulate Signal: Apply the AM formula to obtain the modulated signal.
6.Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

# Procedure:

• Refer Algorithms and write code for the experiment. 
• Open SCILAB in System • Type your code in New Editor 
• Save the file • Execute the code
• If any Error, correct it in code and execute again Verify the generated waveform using Tabulation and Model Waveform

# PROGRAM:
```
import numpy as np
import matplotlib.pyplot as plt
Am = 4.1
Ac = 8.2
fm = 304
fc = 3040
fs = 30400
t = np.arange(0, 3/fm, 1/fs)
m = Am * np.cos(2 * np.pi * fm * t)
c = Ac * np.cos(2 * np.pi * fc * t)
s = (Ac + m) * np.cos(2 * np.pi * fc * t)
plt.figure(figsize=(10, 6))
plt.subplot(3,1,1)
plt.plot(t, m)
plt.xlabel("Time")
plt.ylabel("Amplitude")
plt.grid()
plt.subplot(3,1,2)
plt.plot(t, c)
plt.xlabel("Time")
plt.ylabel("Amplitude")
plt.grid()
plt.subplot(3,1,3)
plt.plot(t, s)
plt.xlabel("Time")
plt.ylabel("Amplitude")
plt.grid()
plt.tight_layout()
plt.show()
```

# OUTPUT WAVEFORM:

<img width="1282" height="729" alt="Screenshot 2025-11-18 105114" src="https://github.com/user-attachments/assets/e4489306-13f9-45d6-9f4d-2924786c821e" />



# TABULATION:

![am using py](https://github.com/user-attachments/assets/2d306135-6eb0-463b-b0dc-688a4c3d524f)



# Result:


The message signal, carrier signal, and amplitude modulated (AM) signal will be displayed in separate plots. Thus AM is implemented using numPy and Matplotlib.
