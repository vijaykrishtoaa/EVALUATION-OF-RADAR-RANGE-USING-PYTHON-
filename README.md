# EVALUATION-OF-RADAR-RANGE-USING-PYTHON-

__Aim__:

To calculate the maximum range of a radar system using the Radar Range Equation and verify the results 
through Python programming.

__Theory__:

The Radar Range Equation is a fundamental formula used in radar system design to determine the maximum 
range at which a radar can detect a target. It is given by:

<img width="573" height="442" alt="image" src="https://github.com/user-attachments/assets/ba374d30-d11f-41e5-a4fc-a42dde71d8e7" />

__Procedure__:

1. Set Up the Python Environment: Ensure that Python is installed on your system. You can use 
Anaconda for managing Python packages and environments, or any other Python IDE of your choice. 
2. Import Necessary Libraries: Import the math library in Python. 
3. Define the Radar Range Equation Function: Create a function to calculate the maximum range using 
the Radar Range Equation. 
4. Input Parameters for the Radar System: Define the input parameters such as transmitted power, 
transmitter gain, receiver gain, radar frequency, radar cross section, and minimum detectable power. 
5. Calculate the Maximum Range: Use the function to calculate the maximum range of the radar. 
6. Execute the Program: Run the Python script to calculate and display the maximum range of the radar.


   ___Algorithm__:
   10

import numpy as np
import matplotlib.pyplot as plt

Pt = 1000
G = 40
lambda_ = 0.05
sigma = 10
pi4 = (4 * np.pi) ** 3

R = np.linspace(1e3, 200e3, 500)
Pr_R = (Pt * G*2 * lambda_2 * sigma) / (pi4 * R*4)
plt.figure()
Pr_R_dB = 10 * np.log10(Pr_R)
plt.plot(R / 1000, Pr_R_dB)
plt.xlabel("Power Received")
plt.ylabel("Range")
plt.show()

Pt_values = np.linspace(100, 10000, 500)
R_fixed = 50e3
Pr_Pt = (Pt_values * G*2 * lambda_2 * sigma) / (pi4 * R_fixed*4)
plt.figure()
plt.plot(Pt_values, Pr_Pt)
plt.xlabel("Power Received")
plt.ylabel("Power Transmitted")
plt.show()

G_values = np.linspace(5, 60, 500)
Pt_fixed = 3000
Pr_G = (Pt_fixed * G_values*2 * lambda_2 * sigma) / (pi4 * R_fixed*4)
plt.figure()
plt.plot(G_values, Pr_G)
plt.xlabel("Power Received")
plt.ylabel("Gain")
plt.show()


Tabulation:
![WhatsApp Image 2025-11-26 at 20 02 52_7c739a5d](https://github.com/user-attachments/assets/9b0a9cf4-b67b-4b00-baa8-10a45f874277)








   __Output__:
   
![WhatsApp Image 2025-11-26 at 20 03 31_ff55c28f](https://github.com/user-attachments/assets/d0bde3fe-e23f-408d-b7f9-f82ebf01252a)
![WhatsApp Image 2025-11-26 at 20 03 32_8cb22ae0](https://github.com/user-attachments/assets/b9d00b87-ad71-4fea-9380-e1c6b1d4d9da)
![WhatsApp Image 2025-11-26 at 20 03 32_0d4d4f30](https://github.com/user-attachments/assets/dd26a30c-5fad-4f82-aa99-df0359737538)









   __Result__:
   
Thus, the maximum range of a radar system using radar range equation is verified using python



