# AM-using-python
#Aim

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries. Apparatus Required
Software: Python with NumPy and Matplotlib libraries

#Apparatus:

Hardware: Personal Computer

#Theory

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of the message signal. The general form of an AM signal is:
<img width="368" height="266" alt="image" src="https://github.com/user-attachments/assets/9a556d06-da9c-4586-93bb-53101452288f" />



#Algorithm:

1.Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency.
2.Generate Time Axis: Create a time vector for the signal duration.
3.Generate Message Signal: Define the message signal as a cosine wave.
4.Generate Carrier Signal: Define the carrier signal as a cosine wave.
5.Modulate Signal: Apply the AM formula to obtain the modulated signal.
6.Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

#Procedure:

• Refer Algorithms and write code for the experiment. 
• Open SCILAB in System • Type your code in New Editor 
• Save the file • Execute the code
• If any Error, correct it in code and execute again Verify the generated waveform using Tabulation and Model Waveform

#PROGRAM:
```
import numpy as np
import matplotlib.pyplot as plt
Am = 5.3
Ac = 10.6
fm = 424
fc = 4240
fs = 42400
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

#OUTPUT WAVEFORM:

<img width="1238" height="738" alt="image" src="https://github.com/user-attachments/assets/14d45c05-021f-4d55-a045-d4130d515942" />


#TABULATION:


![WhatsApp Image 2025-10-26 at 19 09 47_54388b9f](https://github.com/user-attachments/assets/1b1bc905-3a44-422c-a9b5-098ae562608e)

#Result:


The message signal, carrier signal, and amplitude modulated (AM) signal will be displayed in separate plots. Thus AM is implemented using numPy and Matplotlib.
