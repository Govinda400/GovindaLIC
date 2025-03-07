# LIC 1
Experiment-1
Objective:
The goal of this experiment is to perform the DC operating point determination, gain analysis using transient response, and frequency behavior analysis through AC response for two MOSFET-based circuit designs. Additionally, the effect of varying the MOSFET's width and length on the output current is investigated.


# Design-1

![Screenshot 2025-02-17 221608](https://github.com/user-attachments/assets/864a490e-8c8b-4409-8b01-4c3160e326fa)

Objective:
To analyze the circuit's behavior under DC, transient, and AC conditions, and to determine the MOSFET's operating parameters, such as gain and drain current.
![Screenshot 2025-02-17 231421](https://github.com/user-attachments/assets/b1bd6f61-a8a3-4e79-8456-c7e165d28065)


Components Used:
MOSFET
Resistors
DC Power Supply

Procedure:
Set up the circuit as shown in the schematic.
Connect the drain terminal to a resistor, and the gate terminal to a DC power supply and the resistor.
The source terminal is connected to ground.
The input voltage (Vin) is set to 0.9V, and the supply voltage (VDD) is set at 1.8V.
Using the formula 
𝑃
=
𝑉
×
𝐼
P=V×I, the drain current (Id) is calculated as 
5.554
×
10
−
5
 
𝐴
5.554×10 
−5
 A.
The channel length (L) and width (W) of the MOSFET are adjusted to achieve the desired current, as shown in the schematic.


DC Analysis:
To perform DC analysis, select the DC operating point option in the simulation tool and run the simulation.
The results show that the calculated drain current (Id) matches the expected value based on the input power and voltage.

Transient Analysis:
![Screenshot 2025-02-17 133650](https://github.com/user-attachments/assets/60485db8-7f29-4fa9-b362-96f8c25f918d)
![Screenshot 2025-02-17 133738](https://github.com/user-attachments/assets/a06a622a-b6cd-4ffd-84d9-af8115ed3c54)

For transient analysis, a stop time of 1ms is selected, and the simulation is run to observe the circuit’s time-domain behavior.
The results show that the circuit transitions smoothly, confirming its stable operation over time.

AC Analysis:
![Screenshot 2025-02-17 134952](https://github.com/user-attachments/assets/836fe730-107c-4822-83b6-49f4e2a8f5d5)

In AC analysis, the simulation tool is configured for frequency response testing, and the circuit is evaluated across a range of frequencies.
The gain is found to be -9.94 dB, with a phase shift near 180°, which matches theoretical predictions.

Results:
DC Analysis: The drain current (Id = 
5.554
×
10
−
5
 
𝐴
5.554×10 
−5
 A) was successfully achieved by adjusting the MOSFET dimensions (L = 200nm, W = 288nm). The circuit performs as expected under DC conditions.
Transient Analysis: The transient response is stable, and the circuit shows no unexpected delays or distortions.
AC Analysis: The circuit maintains stability and performance across a range of frequencies, with theoretical gain and phase shift values being confirmed.

Conclusion:
The experiment demonstrates that adjusting the MOSFET dimensions (length and width) effectively controls the drain current. The width (W) has a significant influence on Id—larger width increases the drain current. The circuit behaves reliably in all three analyses, confirming the feasibility of the design.

# Design-2
![Screenshot 2025-02-17 232318](https://github.com/user-attachments/assets/8c3a7104-8d27-4ac8-809a-43ba36f77314)

Objective:
To evaluate the circuit’s behavior and performance by performing DC, transient, and AC analyses using two MOSFETs (M1 and M2), and to determine the drain current for different MOSFET dimensions.

Components Used:
Two MOSFETs (M1 and M2)
DC Power Supply
Procedure:
Set up the circuit as depicted in the schematic.
The gate terminals of both MOSFETs are connected to the DC power supply, while the source terminals are grounded.
The input voltage is set using the Voltage Transfer Characteristic (VTC) curve, and the supply voltage is set to 1.8V.
Using the power formula 
𝑃
=
𝑉
×
𝐼
𝑛
P= 
n
V×I
​
 , the drain current (Id) is calculated as 
5.56
×
10
−
5
 
𝐴
5.56×10 
−5
 A.
The channel dimensions (L and W) for both MOSFETs are adjusted to meet the desired current:
M1: L = 500nm, W = 950nm
M2: L = 300nm, W = 1020nm
DC sweep analysis is performed to find the operating voltage (Vin = 0.8V) that places the MOSFETs in the saturation region, as shown in the VTC curve.
![Screenshot 2025-02-17 232500](https://github.com/user-attachments/assets/052828e2-4845-476e-8b52-b212487a905b)
![image](https://github.com/user-attachments/assets/87ef0939-34cc-4bf9-992e-6e559381eb79)
![Screenshot 2025-02-17 232700](https://github.com/user-attachments/assets/e4810989-207f-457e-a7fd-f7ad07b51aff)



DC Analysis:
Perform DC analysis by selecting the DC operating point option and running the simulation.
The results show that the calculated drain current (Id) aligns with the expected value, and by adjusting the MOSFET dimensions, the desired current is achieved for both MOSFETs (M1 and M2).
![image](https://github.com/user-attachments/assets/d216fab2-4ada-476f-a4f2-e55c3415ac4b)


Transient Analysis:
A transient analysis is performed with a stop time of 1ms, and the circuit’s time-domain response is observed.
The results confirm that the circuit transitions smoothly and responds effectively to changes in input voltage, indicating stable operation.
![Screenshot 2025-02-17 232915](https://github.com/user-attachments/assets/c49d0122-4317-4e15-bba2-514d0b66468e)

AC Analysis:
For AC analysis, the circuit’s frequency response is examined across different frequencies.
The gain is found to be 3.8 dB, with a phase shift of nearly 180°, confirming the theoretical expectations.
![Screenshot 2025-02-17 233036](https://github.com/user-attachments/assets/b1806728-3a09-4517-bca9-e3d012aa5151)

Results:
DC Analysis: The drain current (Id = 
5.56
×
10
−
5
 
𝐴
5.56×10 
−5
 A) is consistent with the expected value, and the desired current is achieved by adjusting the MOSFET dimensions (M1: L = 500nm, W = 950nm; M2: L = 300nm, W = 1020nm).
Transient Analysis: The transient response shows smooth transitions, and the circuit operates reliably.
AC Analysis: The circuit performs well in the frequency domain, with gain and phase shift values matching theoretical predictions.
Conclusion:
This experiment verifies that by properly selecting the MOSFET dimensions (L and W), the drain current can be precisely controlled. The voltage transfer characteristics (VTC) curve helped in choosing the correct operating voltage (0.8V) for the saturation region.

Impact of Width Adjustments:
M1 has a smaller influence on the drain current; changes in its width result in minimal variations in Id.
M2 has a stronger influence on Id; increasing its width significantly raises the drain current.
The design meets the expected performance criteria and follows theoretical predictions, making it a feasible solution for practical applications.

Inference:
The experiment successfully demonstrates the ability to control MOSFET drain current by adjusting the width and length of the MOSFETs. The behavior of both designs was thoroughly analyzed through DC, transient, and AC simulations, and the results closely match theoretical expectations. This validates the circuit designs and proves their practical applicability in real-world scenarios.
