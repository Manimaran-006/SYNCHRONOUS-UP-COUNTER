## NAME:MANIMARAN V
## REG.NO:24008541
# EXPERIMENT 11:IMPLEMENTATION SYNCHRONOUS UP COUNTER
# AIM:

To implement 4 bit synchronous up counter and validate functionality.

# SOFTWARE REQUIRED:

Quartus prime

# THEORY

# 4 BIT SYNCHRONOUS UP COUNTER

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

# PROCEDURE

/* write all the steps invloved */

# PROGRAM

![Screenshot 2024-12-21 175932](https://github.com/user-attachments/assets/b2942a1f-e869-4ef0-9da9-c83d6963b4a3)


# RTL LOGIC UP COUNTER
![Screenshot 2024-12-21 175941](https://github.com/user-attachments/assets/8ae179af-3f40-4d89-a8da-1b44cad1a2b1)

# TIMING DIAGRAM FOR IP COUNTER
![Screenshot 2024-12-21 175952](https://github.com/user-attachments/assets/d0da8b9c-95c4-4b48-90c1-28b4597e89a0)

# TRUTH TABLE
![Screenshot 2024-12-21 180001](https://github.com/user-attachments/assets/cebc78f5-9407-42e8-a6ef-74a641215504)

# RESULTS
Thus the 4 bit synchronous up counter is implemented correctly and
program code is successfully executed
