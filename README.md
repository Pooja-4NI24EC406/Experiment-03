# Experiment-03
<h1>Differential Amplifier</h1>
This reports contains the information about differential amplifier
<h3>CONTENTS</h3>
INTRUDUCTION

<h3>INTRODUCTION/THEORY</h3>
  A Differential amplifier is used to amplify the difference between two input signals, while rejecting any signals that are common to both inputs. Here in differential amplifier circuit replacing resistors with MOSFET'S, The main advantage is increasing power, area and           and also disadvantage is Gain is reducing.  It is commonly used in operational amplifiers (op-amps) and is essential for applications like signal processing, noise reduction, and sensor interfacing. It consists of TWO MOSFET'S that amplify the difference between two input signals while rejecting common mode noise. Differencial amplifier is the combination of inverting and non inverting amplifier.

The daigram where an operation amplifier is used as a differencial amplifier


Differencial amplifier using op-amp
<h4>Vo=Ad(V1-V2)</h4> 
<br>The voltage difference present at the inverting and non-inverting terminal gets amplified and thus an amplified output is received. Because of input configuration, all op-amps are considered to be differential amplifiers.</br>
<br>When two inputs are applied at the two terminals the voltage difference produced resultantly will be proportional to the difference of the two applied input signals. Differential amplifier behaves as subtractor circuit, that basically subtracts the two input signal. The differential amplifier can be constructed by making use of BJTs and FETs and Mosfet's.</br>

<h3>CIRCUIT OF DIFFERENCIAL AMPLIFIER</h3>


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
V1-V2/2    is differencial mode signal

