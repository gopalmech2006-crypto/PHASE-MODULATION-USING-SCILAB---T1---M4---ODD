\# PHASE-MODULATION-USING-SCILAB---T1---M4---ODD


## Aim
To implement and analyze Phase Modulation (PM) using Scilab.

## Apparatus Required
1. **Software:** Scilab environment
2. **Hardware:** Personal Computer

---

## Theory
Phase Modulation (PM) is a technique where the phase of the carrier wave is varied in proportion to the instantaneous amplitude of the input signal (message signal). Unlike Frequency Modulation (FM), where the frequency is varied, in Phase Modulation, the phase angle of the carrier wave changes with the amplitude of the message signal.

### Mathematical Representation
The general form of a Phase Modulated signal $s(t)$ is given by:

$$s(t) = A_c \cos(2\pi f_c t + k_p m(t))$$

Where:
* $A_c$ : Amplitude of the carrier wave
* $f_c$ : Carrier frequency
* $m(t)$ : Message signal, typically $m(t) = A_m \cos(2\pi f_m t)$
* $k_p$ : Phase deviation sensitivity (in radians/volt)

---
<img width="320" height="525" alt="image" src="https://github.com/user-attachments/assets/0cc6bff3-75d8-43d9-8ccb-4517bc93755f" />
<img width="379" height="213" alt="image" src="https://github.com/user-attachments/assets/70f6ee1f-7d61-4bb0-82b0-08158f0ce408" />


<img width="331" height="557" alt="image" src="https://github.com/user-attachments/assets/96d62bd3-ccf9-42a6-8235-f6e2b13d8591" />

## Algorithm
1. **Initialize Parameters:**
   * Define carrier amplitude ($A_c$), carrier frequency ($f_c$), message frequency ($f_m$), sampling frequency ($f_s$), and phase sensitivity ($k_p$).
2. **Generate Time Axis:**
   * Create a time array $t$ with suitable sampling steps over the signal duration.
3. **Generate Message Signal:**
   * Compute the message signal vector $m(t)$ using the cosine function.
4. **Generate Carrier Signal:**
   * Compute the unmodulated carrier signal vector $c(t) = A_c \cos(2\pi f_c t)$.
5. **Generate PM Signal:**
   * Compute the phase-modulated signal $s(t) = A_c \cos(2\pi f_c t + k_p m(t))$.
6. **Plot the Signals:**
   * Use Scilab's plotting commands (`subplot`, `plot`, `xtitle`, `xgrid`) to display message, carrier, and modulated signals.

---

## MODEL GRAPH
<img width="1761" height="884" alt="PM Signal" src="https://github.com/user-attachments/assets/a158aa5c-fc9b-4f94-ba1e-7556065676fb" />
<img width="254" height="436" alt="image" src="https://github.com/user-attachments/assets/76da0142-7169-4a15-9b6e-658d48af94a5" />


