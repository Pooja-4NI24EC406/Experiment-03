# Experiment-03
<h1>Differential Amplifier</h1>
This reports contains the information about differential amplifier
<h3>CONTENTS</h3>
Introduction
Theory of Differential Amplifier
Circuit Diagram and Working Principle
Types of Differential Amplifiers
Design and Analysis
Common-Mode Rejection Ratio (CMRR)
Frequency Response and Gain Calculation
Applications of Differential Amplifier
Simulation and Experimental Results
Inference and Conclusion
References



<h3>INTRODUCTION/THEORY</h3>
  A Differential amplifier is used to amplify the difference between two input signals, while rejecting any signals that are common to both inputs. Here in differential amplifier circuit replacing resistors with MOSFET'S, The main advantage is increasing power, area and           and also disadvantage is Gain is reducing.  It is commonly used in operational amplifiers (op-amps) and is essential for applications like signal processing, noise reduction, and sensor interfacing. It consists of TWO MOSFET'S that amplify the difference between two input signals while rejecting common mode noise. Differencial amplifier is the combination of inverting and non inverting amplifier.

The daigram where an operation amplifier is used as a differencial amplifier


Differencial amplifier using op-amp
<h4>Vo=Ad(V1-V2)</h4> 
<br>The voltage difference present at the inverting and non-inverting terminal gets amplified and thus an amplified output is received. Because of input configuration, all op-amps are considered to be differential amplifiers.</br>
<br>When two inputs are applied at the two terminals the voltage difference produced resultantly will be proportional to the difference of the two applied input signals. Differential amplifier behaves as subtractor circuit, that basically subtracts the two input signal. The differential amplifier can be constructed by making use of BJTs and FETs and Mosfet's.</br>

<br>In an Integrated Circuit(IC) high value capacitor is difficult to fabricate in IC
To get rid of this, in amplifiers the capacitors are replaced without losing the effect of capacitors
This is possible using differential amplifier.</br>
V1-V2=Vd(differencial input)
Output can be either differencial ended or single ended
for V1=V2 Then ideally output will be 0
V1 can also be written as 
V1=V1/2+V1/2
V1=V1+V2/2 + (V1-V2)/2 ---1
Similarly
V2=V2/2+V2/2
V2=(V1+V2/2 - (V1-V2)/2 ---2
From 1 and 2
V1+V2/2    it is common voltage(COMMON MODE SIGNAL Vcm)
V1-V2/2    (DIFFERENTIAL MODE SIGNAL Vdm)
V1=Vcm+Vdm
V2=Vcm-Vdm

<h3> WORKING PRINCIPLE </h3>
Operating in active region for proper amplification, it can Work in Different Modes i.e, It can function in common-mode (same signal on both inputs) and differential-mode (different signals on inputs).
The output is affected by the resistors(Rd) <h4>Vout=Vdd-Id*Rd,</h4>
The circuit is designed symmetrically, so for this reason current is equally distrubuting
It receives two input signals and compares them.
It strengthens only the difference between the two inputs.
Any noise or interference that is present in both inputs is removed
Both transistors share the same power source and work together to balance the signals.
The input signals control how the current splits between the two transistors, determining the output.
The output changes based on how different the input signals are.
It often uses feedback to stabilize gain and improve performance.
Both transistors or mosfets work in a balanced way, reducing errors due to temperature changes.

<h3>TYPES OF DIFFERENCIAL AMPLIFIER</h3>
1.Resistive Load Differential Amplifier – Uses resistors as load (simple but low gain).
2. Active Load Differential Amplifier – Uses MOSFET loads for higher gain.
3. Current Mirror Differential Amplifier – Provides improved matching and increased gain.
4. Fully Differential Amplifier – Provides both differential inputs and outputs for better noise rejection.


<h3>ANALYSING THE QUESTION with proper formulas</h3>
<h4>Design differencial amplifier for the following specifications Vdd=3.2V  P<=2.8mW  Vicm=1,6V  Vocm=1.7V Vp=0.6V. Perform DC Analysis,Transient analysis and frequency response and extract the required parameters. </h4>
Given,
  Vdd=3.2V
  P<=2.8mW
  Vicm=1.6V
  Vocm=1.7V
  Vp=0.6V
Vout=Vdd-Id*Rd
1.7 = 3.2-Id*Rd
From P=VI
Iss=P/V
2.8m/3.2=0.875mA
Id=0.875m/2=0.43mA
Rd=Vdd-Vocm/Id=3.2-1.7/0.43m=3.48k
Rss=Vp/Iss=0.6/0.875m=0.68k

Values of each components:
Rd=3.48K
Rss=0.68K
Iss=0.875mA
Id=43mA
Vdd=3.2V P<=2.8mW Vicm=1.6V Vocm=1.7V Vp=0.6V

<h3>CIRCUIT DAIGRAM WITH REQUIRED COMPONENTS & SPECIFICATION</h3>




Power supply(Vdd)=3.2V
2 Input voltage (Vicm)=1.6V
2 Drain resistor Rd1=Rd2=Rd = 3.48K
Rss=0.68K
2 Vocm=1.7V
node voltage Vp=0.6V
groung-0V

<h4>ANALYSING the circuit by using LTSpice</h4>


 |PARAMETER INCREASED  |EFFECT ON Rd                                             |EFFECT ON Rss                                     |EFFECT ON Vout                                      |EFFECT ON Vin        
                       |EFFECT ON GAIN                                           |
                       
|----------------------|---------------------------------------------------------|--------------------------------------------------|----------------------------------------------------|-------------------------------------------------|---------------------------------------------------------|

|Vdd                   |No direct effect, but voltage across RD increasing       |No direct effect, but ISS may need adjustment     |Increases (more headroom, higher swing)             |No direct effect, but biasing may shift      |Increases (higher VDD allows a larger RD)|
