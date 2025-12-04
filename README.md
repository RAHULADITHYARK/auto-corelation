# SIMULATION OF AUTOCORRELATION AND PSD USING SCILAB
# AIM:
Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation.

# EQUIPMENTS Needed
• Computer with i3 Processor • SCI LAB

# THEORY:
The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.
<img width="1454" height="235" alt="image" src="https://github.com/user-attachments/assets/bb173f6e-9a8b-4617-bee0-304285264072" />

# Algorithm
Load or Define the Signal: Input your time-domain signal.

Compute Autocorrelation: Calculate the autocorrelation function of the signal.

Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.

Plot Results: Visualize the autocorrelation function and PSD.

# PROCEDURE
• Refer Algorithms and write code for the experiment.

• Open SCILAB in System

• Type your code in New Editor

• Save the file

• Execute the code

• If any Error, correct it in code and execute again

• Verify the generated waveform using Tabulation and Model Waveform

# PROGRAM:
```scilab
t=0:0.01:2*%pi;
x=6*sin(2*t);
subplot(3,2,1);
plot(x);
au=xcorr(x,x);
subplot(3,2,2);
plot(au);
v=fft(au);
subplot(3,2,3);
plot(abs(v));
fw=fft(x);
subplot(3,2,4);
plot(fw);
fw2=(abs(fw)).^2;
subplot(3,2,5);
plot(fw2);
```
# OUTPUT:
<img width="1721" height="768" alt="image" src="https://github.com/user-attachments/assets/30d3e013-1d40-4dc0-8ef7-3061bb5f0f5d" />
![WhatsApp Image 2025-12-04 at 10 23 27_a6d7b163](https://github.com/user-attachments/assets/55fd2830-c1c1-4342-857f-88cb9cf72e04)



# RESULT:
Thus the Autocorrelation and PSD are executed in Scilab and output is verified.
