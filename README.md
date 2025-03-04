# Experiment-03
<h1>Differential Amplifier</h1>
This reports contains the information about differential amplifier
<h3>CONTENTS</h3>
<br>Introduction<br>
<br>Theory of Differential Amplifier<br>
<br>Circuit Diagram and Working Principle<br>
<br>Types of Differential Amplifiers<br>
<br>Design and Analysis<br>
<br>Common-Mode Rejection Ratio (CMRR)<br>
<br>Frequency Response and Gain Calculation<br>
<br>Applications of Differential Amplifier<br>
<br>Simulation and Experimental Results<br>
<br>Inference and Conclusion<br>
<br>References<br>



<h3>INTRODUCTION/THEORY</h3>
  A Differential amplifier is used to amplify the difference between two input signals, while rejecting any signals that are common to both inputs. Here in differential amplifier circuit replacing resistors with MOSFET'S, The main advantage is increasing gain and disadvantage is reducing/dicreasing area and power.  It is commonly used in operational amplifiers (op-amps) and is essential for applications like signal processing, noise reduction, and sensor interfacing. It consists of TWO MOSFET'S that amplify the difference between two input signals while rejecting common mode noise. Differencial amplifier is the combination of inverting and non inverting amplifier.

<br><h4>The daigram where an operation amplifier is used as a differencial amplifier</h4><br>


<br>Differencial amplifier using op-amp<br>
Vo=Ad(V1-V2) 
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

<h4>Analysis</h4>
<br><h4>Common mode analysis:</h4>Calculate the output voltage when the same input signal is applied to both input terminals of the differential amplifier.<br>



<br><h4>Differential mode analysis:</h4>Calculate the output voltage when two different input signals are applied to the input terminals of the differential amplifier.<br>   




<h3> WORKING PRINCIPLE </h3>
<br>Operating in active region for proper amplification, it can Work in Different Modes i.e, It can function in common-mode (same signal on both inputs) and differential-mode (different signals on inputs).<br>
<br>1. The output is affected by the resistors(Rd) Vout=Vdd-Id*Rd.<br>
<br>2. The circuit is designed symmetrically, so for this reason current is equally distrubuting<br>
<br>3. It receives two input signals and compares them.<br>
<br>4. It strengthens only the difference between the two inputs.<br>
<br>5. Any noise or interference that is present in both inputs is removed<br>
<br>6. Both transistors share the same power source and work together to balance the signals.<br>
<br>7. The input signals control how the current splits between the two transistors, determining the output.<br>
<br>8. The output changes based on how different the input signals are.<br>
<br>9. It often uses feedback to stabilize gain and improve performance.<br>
<br>10.Both transistors or mosfets work in a balanced way, reducing errors due to temperature changes.<br>

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
Id=43mA</p>
<br>Vdd=3.2V P<=2.8mW Vicm=1.6V Vocm=1.7V Vp=0.6V<br>



<h4>ANALYSING the circuit by using LTSpice</h4>


 |PARAMETER INCREASED  |EFFECT ON Rd                                             |EFFECT ON Rss                                     |EFFECT ON Vout                                      |EFFECT ON Vin        
                       |EFFECT ON GAIN                                           |
                       
|----------------------|---------------------------------------------------------|--------------------------------------------------|----------------------------------------------------|-------------------------------------------------|---------------------------------------------------------|

|Vdd                   |No direct effect, but voltage across RD increasing       |No direct effect, but ISS may need adjustment     |Increases (more headroom, higher swing)             |No direct effect, but biasing may shift      |Increases (higher VDD allows a larger RD)|
|RD ↑                  |	—                                                      |No direct effect, but affects current balance     |	Increases (higher gain, larger swing)              |No direct effect	 
                       |Increases (Av = -gm * RD)                                |
|RSS ↑	               |No direct effect                                         |	—                                               |	Improves CMRR, but excessive RSS may reduce gain	 |Differential input range may reduce             |	Can improve CMRR, but too large RSS reduces gain       |
|W (Width) ↑           |No direct effect,but higher gm reduces needed RD same Av | No direct effect, but affects bias current       |	May decrease (if lower RD is used)                 | 	Increases input capacitance            |	Increases (since gm increases)                         |
|L (Length) ↑          |	No direct effect, but increases output resistance      |	No direct effect                                |	Can increase (better channel control)	             |No direct effect, but speed decreases	       |Increases slightly (higher output resistance)            |

IN Simple words:
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

<h4>Steps for LTSpice Simulation</h4>
<br>Step 1: Design the circuit in LTSpice<br>
<br>Step 2: Set the input voltage as an AC source.<br>
<br>Step 3: Run a DC, Transient, and AC Analysis to observe current and signal amplification.<br>
<br>Step 4: Verify the current and phase inversion in the waveform.<br>

<h3>DC ANALYSIS</h3>





<h3>TRANSIENT ANALYSIS</h3>







<h3>AC ANALYSIS</h3>











<h3>REPLACED RESISTOR(Rss) WITH A Iss(CURRENT SOURSE</h3>





<h3>DC ANALYSIS</h3>







<h3>TRANSIENT ANALYSIS</h3>







<h3>AC ANALYSIS</h3>









<h4> ADVANTAGES</h4>




<h3>REPLACED CURRENT SOURCE WITH A MOSFET</h3>






<h3>DC ANALYSIS</h3>






<h3>TRANSIENT ANALYSIS</h3>






<h3>AC ANALYSIS</h3>







INFORMATION






<h3>REPLACE Rd with MOSFET</h3>



<h3>DC ANALYSIS</h3>




<h3>TRANSIENT ANALYSIS</h3>





<h3>AC ANALYSIS</h3>






COMPARISON INFORMATION





<h3>RESULT</h3>







<h3>INFERENCE</h3>







<h3>REFERENCE</h3>



<h3>FINAL CONCLUSION</h3>
