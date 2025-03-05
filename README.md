# Experiment-03
<h1>Differential Amplifier</h1>
This reports contains the information about differential amplifier
<h3>CONTENTS</h3>
<br>Introduction/Theory of Differential Amplifier<br>
<br>Circuit Diagram with specifications <br>
<br>Working principle and Types of Differential Amplifiers<br>
<br>Analysis of circuit Design and question <br>
<br>Steps for LTSpice<br>
<br>Circuit daigram simulation results<br>
<br>Role of each components<br>
<br>Comparison table<br>
<br>Result,Inference and Conclusion<br>
<br>References<br>



<h3>INTRODUCTION/THEORY</h3>
  A Differential amplifier is used to amplify the difference between two input signals, while rejecting any signals that are common to both inputs. Here in differential amplifier circuit replacing resistors with MOSFET'S, The main advantage is increasing gain and disadvantage is reducing/dicreasing area and power.  It is commonly used in operational amplifiers (op-amps) and is essential for applications like signal processing, noise reduction, and sensor interfacing. It consists of TWO MOSFET'S that amplify the difference between two input signals while rejecting common mode noise. Differencial amplifier is the combination of inverting and non inverting amplifier.

<br><h4>The daigram where an operation amplifier is used as a differencial amplifier</h4><br>

![image](https://github.com/user-attachments/assets/f8a08798-46a2-4d7f-a7f1-898239cb5f2c)

<br>Differencial amplifier using op-amp Vo=Ad(V1-V2)<br> 
<br>The voltage difference present at the inverting and non-inverting terminal gets amplified and thus an amplified output is received. Because of input configuration, all op-amps are considered to be differential amplifiers.</br>
<br>When two inputs are applied at the two terminals the voltage difference produced resultantly will be proportional to the difference of the two applied input signals. Differential amplifier behaves as subtractor circuit, that basically subtracts the two input signal. The differential amplifier can be constructed by making use of BJTs and FETs and Mosfet's.</br>


<h3>CIRCUIT DAIGRAM WITH REQUIRED COMPONENTS & SPECIFICATION</h3>
<p>In an Integrated Circuit(IC) high value capacitor is difficult to fabricate in IC
so for this reason, in amplifiers the capacitors are replaced without losing the effect of capacitors
This is possible using differential amplifier.</p>
<br>Power supply(Vdd)=3.2V<br>
<br>2 Input voltage (Vicm)=1.6V<br>
<br>2 Drain resistor Rd1=Rd2=Rd = 3.48K<br>
<br>Rss=0.68K<br>
<br>2 Vocm=1.7V<br>
<br>node voltage Vp=0.6V<br>
<br>groung-0V<br>

![daigram](https://github.com/user-attachments/assets/a4a89b43-9b69-4de0-9994-87b0e2f803a6)

<br>V1-V2=Vd(differencial input)<br>
<br>Output can be either differencial ended or single ended<br>
<br>for V1=V2 Then ideally output will be 0 V1 can also be written as <br>
<br>V1=V1/2+V1/2<br>
<br>V1=V1+V2/2 + (V1-V2)/2 ---1<br>

Similarly,
<br>V2=V2/2+V2/2<br>
<br>V2=(V1+V2/2 - (V1-V2)/2 ---2<br>

From 1 and 2
<br>V1+V2/2    it is common voltage(COMMON MODE SIGNAL Vcm)<br>
<br>V1-V2/2    (DIFFERENTIAL MODE SIGNAL Vdm)<br>
<br>V1=Vcm+Vdm<br>
<br>V2=Vcm-Vdm<br>

<h3>Key points about common mode and differential mode analysis in a differential amplifier:</h3>
<br><h4>Common mode signal:<h4></h4>When both inputs of the differential amplifier receive the same signal, this is considered a common-mode signal.<br>
<br><h4>Differential mode signal:</h4>When the inputs receive signals that are different from each other, this is considered a differential mode signal. 
It is important, because of Noise rejection: A good differential amplifier should have a high "common-mode rejection ratio" (CMRR), meaning it should significantly amplify the differential mode signal while rejecting any common-mode noise present on both inputs.<br>
<br><h4>Common mode analysis:</h4>Calculate the output voltage when the same input signal is applied to both input terminals of the differential amplifier.<br>
<br><h4>Differential mode analysis:</h4>Calculate the output voltage when two different input signals are applied to the input terminals of the differential amplifier.<br>   



<h3> WORKING PRINCIPLE </h3>
<br>Operating in active region for proper amplification, it can Work in Different Modes i.e, It can function in common-mode (same signal on both inputs) and differential-mode (different signals on inputs).<br>
<br>The output is affected by the resistors(Rd) Vout=Vdd-Id*Rd.<br>
<br>The circuit is designed symmetrically, so for this reason current is equally distrubuting<br>
<br>It receives two input signals and compares them.<br>
<br>It strengthens only the difference between the two inputs.<br>
<br>Any noise or interference that is present in both inputs is removed<br>
<br>Both transistors share the same power source and work together to balance the signals.<br>
<br> The input signals control how the current splits between the two transistors, determining the output.<br>
<br>The output changes based on how different the input signals are.<br>
<br>It often uses feedback to stabilize gain and improve performance.<br>
<br>Both transistors or mosfets work in a balanced way, reducing errors due to temperature changes.<br>

<br><h3>TYPES OF DIFFERENCIAL AMPLIFIER</h3><br>
<br>1.Resistive Load Differential Amplifier – Uses resistors as load (simple but low gain).<br>
<br>2. Active Load Differential Amplifier – Uses MOSFET loads for higher gain.<br>
<br>3. Current Mirror Differential Amplifier – Provides improved matching and increased gain.<br>
<br>4. Fully Differential Amplifier – Provides both differential inputs and outputs for better noise rejection.<br>


<h3>ANALYSING THE QUESTION with proper formulas</h3>
<h4>Design differencial amplifier for the following specifications Vdd=3.2V  P<=2.8mW  Vicm=1,6V  Vocm=1.7V Vp=0.6V. Perform DC Analysis,Transient analysis and frequency response and extract the required parameters. </h4>
  
Given,
 <br> Vdd=3.2V<br>
  <br>P<=2.8mW<br>
  <br>Vicm=1.6V<br>
  <br>Vocm=1.7V<br>
  <br>Vp=0.6V<br>
<br>Vout=Vdd-Id*Rd<br>
<br>1.7 = 3.2-Id*Rd<br>
<br>From P=VI<br>
<br>Iss=P/V<br>
<br>2.8m/3.2=0.875mA<br>
<br>Id=0.875m/2=0.43mA<br>
<br>Rd=Vdd-Vocm/Id=3.2-1.7/0.43m=3.48k<br>
<br>Rss=Vp/Iss=0.6/0.875m=0.68k<br>
<br>Values of each components:<br>
<p>Rd=3.48K
Rss=0.68K
Iss=0.875mA
Id=0.43mA</p>
<br>Vdd=3.2V P<=2.8mW Vicm=1.6V Vocm=1.7V Vp=0.6V<br>



<h4>Steps for LTSpice Simulation</h4>

<br>Step 1: Design the circuit in LTSpice as per the circuit daigram<br>
<br>Step 2: Set the input voltage as an AC source.<br>
<br>Step 3: Run a DC, Transient, and AC Analysis to observe current and signal amplification.<br>
<br>Step 4: Verify the current and phase inversion in the waveform.<br>
<br>Step 5: Relace a Rss(R3) with a current and follow the same procedure<br>
<br>Step 6: Again replace current source with a MOSFET, observe DC, transient and Ac analysis<br>
<br>Step 7: last step is replace Rd1 and Rd2 with a mosfet and follow the same steps<br>
   by replacing these resistors then gain is increasing so ths is the main advantages of doing these steps

<h3>DC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/0db3dfd9-b2fd-4a00-b877-9e643d963033)





<h3>TRANSIENT ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/b4bdb08b-d146-47c8-a1df-6960ef73b312)







<h3>AC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/d47373d5-f0be-4c65-80ff-6414871a317b)

Ac gain = 20log10(328.9*10^3/99.25*10^3)
<br>10.406<br>


<h4>ANALYSING the circuit by using LTSpice</h4>

| PARAMETER INCREASED | EFFECT ON GAIN | EFFECT ON Rss | EFFECT ON Vout | EFFECT ON Vin |
|---------------------|---------------|--------------|---------------|--------------|
| Vdd ↑ | No direct effect, but voltage across RD increases | No direct effect, but ISS may need adjustment | Increases (more headroom, higher swing) | No direct effect, but |
| RD ↑ | Increases (higher VDD allows a larger RD) | No direct effect, but affects current balance | Increases (higher gain, larger swing) | No direct effect |
| ISS ↑ | No direct effect | Improves CMRR, but excessive ISS may reduce gain | Improves CMRR, but excessive ISS may reduce gain | Differential input range |
| W/L (Width/Length) ↑ | Can improve CMRR, but too large RSS reduces gain | No direct effect, but affects bias current | May decrease (if lower RD is used) | Increases input |
| Capacitance ↑ | Increases (since gm increases) | No direct effect | Can increase (better channel control) | No direct effect, and |
| Speed decreases | Increases slightly (higher output resistance) | No direct effect | | |

<br>More VDD : More Vout, More Gain<br>
<br>More RD : More Vout, More Gain<br>
<br>More RSS : Better CMRR, but can reduce gain<br>
<br>More W: More Current, Less Vout (if RD fixed), More Gain<br>
<br>More L: More Gain, Better Output Resistance<br>


<h3>ROLE OF EACH COMPONENTS in the circuit</h3>
<br>M1 & M2                : Amplify the difference between inputs.<br>
<br>M3 (ISS Source)        : Provides a stable tail current, after replace.<br>
<br>M4 & M5 (Active Load)  :Replace resistors to improve gain, This is after replacing RD-MOSFETS<br>
<br>RD                     :Converts current to voltage (affects gain).<br>
<br>RSS                    :Improves CMRR but can reduce gain.<br>
<br>Biasing Circuit (VBIAS):Sets MOSFET operating points.<br>






<h3>REPLACED RESISTOR(Rss) WITH A Iss(CURRENT SOURSE</h3>

![image](https://github.com/user-attachments/assets/f0ee53a8-b699-47e9-9029-6b550eff3532)

When we replacing RSS with a current source, the common-mode rejection ratio (CMRR) improves significantly because the current source provides high impedance, which enhances circuit balance. This results in better gain stability, improved linearity, and reduced dependence on resistor mismatches.


<h3>DC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/badf0034-32d8-423b-9fcb-9b4fef129275)






<h3>TRANSIENT ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/c8f6a61d-a717-4fcc-9062-dc455189f017)






<h3>AC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/52ae2cde-485f-4538-b1f4-d24dda0be620)

Ac gain = 20log10(328.9*10^3/99.25*10^3)
<br>10.406<br>



<h3>REPLACED CURRENT SOURCE WITH A MOSFET</h3>

![image](https://github.com/user-attachments/assets/1acbb66a-6fcf-4a9e-8a00-c218f82bca33)

When we replace the current source with a MOSFET (acting as an active current source), the circuit achieves better current regulation, higher output impedance, and improved CMRR. The MOSFET provides dynamic resistance, reducing variations due to temperature or component mismatches. This leads to better differential gain and improved linearity compared to a simple resistor or current source. However, proper biasing is crucial to ensure stable operation.





<h3>DC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/ff1e6d91-5d55-4c7d-bc08-fadbf93837c1)






<h3>TRANSIENT ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/0206307b-9589-4af4-8994-18f101411cfe)





<h3>AC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/98fb0bb8-28d4-490a-8e27-8ed34223ec95)

Ac gain = 20log10(328.9*10^3/99.25*10^3)
<br>10.406<br>











<h3>REPLACE Rd with MOSFET</h3>

 ![image](https://github.com/user-attachments/assets/3340a503-d272-472e-809e-54c775b8e765)

Replacing ISS with a MOSFET and RD1, RD2 with MOSFETs transforms the differential amplifier into a fully active-loaded differential amplifier.Gain is increasing more.



<h3>DC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/5af68060-f852-4183-bf41-3d27f0a1df34)






<h3>TRANSIENT ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/b28f37c4-ce2b-45c0-af54-9d58b22751de)





<h3>AC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/1a3d2325-9c9f-40a5-9447-0ad37665d975)



<h3>Comparison Before & After MOSFET Replacements</h3>

|Features                   | Before (RD & ISS)                          | After (MOSFET Active Load & MOSFET ISS)                      |
|---------------------------|--------------------------------------------|--------------------------------------------------------------|
|Gain                       | high                                       | Even Higher (MOSFET loads have much higher resistance)
|CMRR                       |	Good (ISS improves CMRR)	                 | Much Better (MOSFET ISS further improves rejection)
|Output Swing               |	Limited by RD voltage drop                 |	Better Swing (MOSFET loads adjust dynamically)
|Power Consumption	        | Moderate (Resistors still consume voltage) | Lower Power (No resistors, more efficient)
|Bias Stability	            |Stable (ISS provides constant current)      | More Stable (MOSFET ISS further stabilizes current)
|Speed & Bandwidth          |	Moderate (RD & ISS introduce parasitics)   |	Faster Response (MOSFETs reduce parasitic effects)
|Design Complexity          |	Moderate (Requires ISS circuit)	           | More Complex (Needs biasing for both MOSFET ISS & active loads)

<h3>RESULT</h3>
After designing, analyzing, and simulating this circuit,

Current is calculated , theorical value is 0.43uA, after simulating in LTspice we get or setted as 0.43uA.The circuit provided a significant voltage amplification.

The gain was calculated and verified using LTSpice simulation.
The output waveform was inverted with respect to the input.

The voltage gain depends on the transconductance and drain resistor Av=-Gm*Rd. LTSpice simulation results match with theoretical calculations.
Simulated using LTSpice, simulated the circuit, Vdd=3.2V, 
  P<=2.8mW        
  Vicm=1.6V
  Vocm=1.7V
  Vp=0.6V <p>Rd=3.48K
Rss=0.68K
Iss=0.875mA
Id=0.43mA
  Av=10.4</p>
  <br>theoritically we setted as perfectly same as possible.

Observed differential gain of approximately 10.4dB.Experimental Observations ( MOSFETs)

The circuit performed as expected, amplifying differential input while rejecting common-mode signals.





<h3>INFERENCE</h3>
The differential amplifier perfectly amplifies differential signals while rejecting noise.

operating points is set as required values.

CMRR is enhanced using current sources and active loads.

MOSFET based designs offer better power efficiency and high input impedance.

The circuit is widely used in modern analog and mixed-signal designs and also it is used to increase the gain

And main disadvantage is reducing area and power by using this differential amplifier 


<h3>FINAL CONCLUSION</h3>
After simulating this circuit we get to know that,The differential amplifier is a fundamental circuit in analog electronics, crucial for applications in op-amps, instrumentation, and communication systems. With proper design, high gain, low noise, and excellent common-mode rejection can be achieved. Simulation and experimental results confirm its effectiveness in signal amplification and noise reduction.


<h3>REFERENCE</h3>

https://electronicscoach.com/differential-amplifier.html

https://chatgpt.com/share/67c2e955-8f2c-8013-bbcd-2ba0aba04355
