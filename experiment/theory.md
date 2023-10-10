
<div style="font-family: 'Nunito Sans', sans-serif; font-size: 20px;text-align: justify;">
<h2>Introduction</h2>

The electronic circuits which can perform the mathematical operations such as logarithm and anti-logarithm with an amplification are called as Logarithmic and Anti-Logarithmic amplifiers respectively. The applications for log/anti-log amplifiers include signal compression and process control.<br>

### 1) Log Amplifier

A logarithmic amplifier is an electronic circuit that produces an output that is proportional to the logarithm of the applied input. An op-amp based logarithmic amplifier produces a voltage at the output, which is proportional to the logarithm of the voltage applied to the resistor connected to its inverting terminal. The circuit diagram of op-amp based logarithmic amplifier is shown in figure 1. <br>
<center><img src="[images/log1.jpg](https://user-images.githubusercontent.com/57490073/273801545-2e919ccf-0909-4c1f-a503-3a69ba5ad47b.jpg)" style=" height: 180px" align="center"></center><br>
<center><b>Fig 1: Op-amp based Logarithmic Amplifier</b></center><br>
In the above circuit, the non-inverting input terminal of the op-amp is connected to ground. That means zero volts is applied at the non-inverting input terminal of the op-amp.<br>
The nodal equation at the inverting input is as follows<br>
<center>0 - V<sub>i</sub>/R<sub>1</sub> + I<sub>f</sub> = 0  ..........(1)</center><br>
from the equation 1,the feedback current is<br><center>I<sub>f</sub> = V<sub>i</sub>/R<sub>1</sub></center><br>
When the diode is forward biased, the current flowing through the diode is<br><center>I<sub>f</sub> = I<sub>s</sub>𝑒<sup>(V<sub>f</sub>/nV<sub>T</sub>)</sup>..........(2)</center><br>
Where,<br>
I<sub>s</sub> is the saturation current of the diode,<br>
V<sub>f</sub> is the voltage drop across diode, when it is in forward bias,<br>
V<sub>T</sub> is the diode's thermal equivalent voltage.<br>
The KVL equation around the feedback loop of the op amp will be<br>
<center>0 - V<sub>f</sub> - V<sub>0</sub> = 0</center><br>
<center>V<sub>f</sub> = -V<sub>0</sub></center><br>
Substituting the value of V<sub>f</sub> in Equation 2, we get<br>
<center>I<sub>f</sub> = I<sub>s</sub>𝑒<sup>(-V<sub>0</sub>/nV<sub>T</sub>)</sup> ..........(3)</center><br>
<center>V<sub>i</sub>/R<sub>1</sub> = I<sub>s</sub>𝑒<sup>(-V<sub>0</sub>/nV<sub>T</sub>)</sup></center><br>
<center>V<sub>i</sub>/R<sub>i</sub>I<sub>s</sub> = 𝑒<sup>(-V<sub>0</sub>/nV<sub>T</sub>)</sup></center><br>
Applying natural logarithm on the both sides<br>
<center>ln(V<sub>i</sub>/R<sub>1</sub>I<sub>s</sub>) = -V<sub>0</sub>/nV<sub>T</sub></center><br>
<center>V<sub>0</sub> = -nV<sub>T</sub>ln(V<sub>i</sub>/R<sub>1</sub>I<sub>s</sub>)</center><br>
In the above equation, the parameters n, V<sub>T</sub> and I<sub>s</sub> are constants. So, the output voltage V<sub>0</sub> will be proportional to the natural logarithm of the input voltage V<sub>i</sub> for a fixed value of resistance R<sub>1</sub>.<br>
The output voltage V<sub>0</sub> has a negative sign, which indicates that there exists a 180° phase difference between the input and the output.<br><br>


### 2) Antilog Amplifier 

An op-amp based anti-logarithmic amplifier produces a voltage at the output, which is proportional to the anti-logarithm of the voltage that is applied to the diode connected to its inverting input. The circuit diagram of an op-amp based anti-logarithmic amplifier is shown in figure 2.<br>
<center><img src="images/anti.jpg" style=" height: 180px" align="center"></center><br>
<center><b> Fig 2:Op-amp based Anti-Logarithmic Amplifier</b></center><br>
In the circuit shown above, the non-inverting input of the op-amp is connected to ground. According to the virtual ground concept, the voltage at the inverting input of op-amp will be equal to the voltage present at its non-inverting input. So, the voltage at its inverting input will be zero volts.<br>
The nodal equation at the inverting input node is <br>
<center>-I<sub>f</sub>+0-V<sub>0</sub>/R<sub>f</sub> = 0</center><br>
<center>V<sub>0</sub> = -I<sub>f</sub>*R<sub>f</sub> ..........(4)</center><br>
When the diode is forward biased, the current flowing through the diode is given by <br>
<center>I<sub>f</sub> = I<sub>s</sub>𝑒<sup>(V<sub>f</sub>/nV<sub>T</sub>)</sup></center><br>
Substituting the value of I<sub>f</sub> in Equation 4, then<br>
<center>V<sub>0</sub> = -R<sub>f</sub>I<sub>s</sub>𝑒<sup>(V<sub>f</sub>/nV<sub>T</sub>)</sup>..........(5)</center><br>
The KVL equation at the inverting input of the op-amp will be<br>
<center>V<sub>i</sub> - V<sub>f</sub> = 0</center><br>
So,<br>
<center>V<sub>i</sub> = V<sub>f</sub></center><br>
Substituting the value of V<sub>f</sub> in equation 5, then<br>
<center>V<sub>0</sub> = -R<sub>f</sub>I<sub>s</sub>𝑒<sup>(V<sub>i</sub>/nV<sub>T</sub>)</sup></center><br>
In the above equation the parameters n, V<sub>T</sub> and I<sub>s</sub> are constants. So, the output voltage V<sub>0</sub> will be proportional to the anti-natural logarithm of the input voltage V<sub>i</sub>, for a fixed value of feedback resistance R<sub>f</sub>.<br>
The output voltage V<sub>0</sub> has a negative sign, which indicates that there exists a 180° phase difference between the input and the output.
</div>
