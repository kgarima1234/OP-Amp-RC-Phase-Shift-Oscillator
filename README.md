# OP Amp RC Phase Shift Oscillator
An electrical oscillator circuit that generates sine waves is known as a phase shift oscillator. Either a transistor or an Op-amp can be used to design the inverting amplifier. In an RC phase shift oscillator, the RC network will be formed in feedback path, The amplifier provides a 180 degree of phase shift due to inverting in nature and the feedback path will also prodvide 180 degree of phase shift (to get the sustained oscillations, in the RC phase shift oscillator), so the overall phase shift will be 360 degree (or zero degree) and by tuning the gain of this amplifier and the feedback circuit it is possible to achieve the loop gain that is equal to 1. <br><br>  

Schematic Diagram of RC Phase Shift Oscillator using Opamp in Ltspice software
![schematic of Opamp RC Phase Shift Oscillator](https://user-images.githubusercontent.com/111141190/192093672-fcbfaab0-7fb2-45b8-a96f-73c853352f88.jpg)
In this RC Phase shift oscillator, the attenuation that is introduced by this feedback stage is equal to 1/29. So, to get a unity loop gain, the gain that is provided by this op-amp should be equal to 29. As we know the formula of gain of an inverting amplifier is A=mod(-Rf/R1), where Rf is feedback resistance. As, the gain of opamp RC phase shift is greater that and equal to 29, so Rf should also be greater than and equal to 29 times of R1.
<br><br>
The output waveform of the Op-amp
![waveform of RCPS oscillator](https://user-images.githubusercontent.com/111141190/192093662-e5f0101d-8c0d-42de-90a4-f107c41450ad.jpg)
This Circuit will provide a unity gain only at one particular frequency and at only one particular frequency only the overall phase shift of the circuit will be equal to 360 degree oe zero degree and if three stages are used then this frequency f can be given by the expression 1/(2piRC*2.45), where R and C are resistor and capacitror of the feedback path respectively. Here I am taking R=650ohm and C=0.1micro Farad, by hand calculation I am getting 999.6 Hz but from the wavefrom I am getting 995.28 Hz. The error is 0.4% in frequency of oscillation.
<br><br>
The stable output waveform of the Op-amp
![Frequency and amplitude of waveform of RCPS oscillator](https://user-images.githubusercontent.com/111141190/192093646-6ddf4d81-79f4-4133-83e1-a5e23d8ce24a.jpg)

 We have calculated the frequency of oscillation using the time period of the stable periodic waveform. The frequency will be inverse of time period.
