---
layout: default
katex: true
---
# <center>XJEL/ELEC2140 Learning Tracking</center>
## <center>Yanshan Xie 201199596 2017110397</center>
### <center>Timestamp: April 12th, 2020</center>
You can receive latest update here: [XJEL2140 Learning Tracking](./XJEL2140_Contents.html)

As the Lecture Captures are my major learning material right now, following table are filled.

| Source / Materials | Current Progress | Latest | Feedback & Note |
|:-|:-|:-|:-|
| Lecture Captures (Videos host on Mediasite) |OO_Mobile Phone and RFIC | ZB_FIRST YEAR COMMS REVISION | **No nonplus so far** |
| Lecture Slides | *In sync with lecture captures* | 19_amps_part2 | **No nonplus so far** |
| ADS Screencast Tutorials for CAD Sheets | Cad2p1 | Cad4p1 | **No nonplus so far** |
| PowerPoint Screencasts of the Lectures (in Learning Resources) | 8_Reflections, Standing Waves, Transmission Line Resonators | 13_Digital communications I and Q in transceivers | The Screencasts are not compulsory, and some contents are covered in Lecture Captures. ***Planned for Revision.*** |
| Lab | ***<u>Not started yet</u>*** | Lab 5 TRL Resonator | ***<u>Not pragmatic now</u>*** |

## Detailed Progress
### Lecture Captures (Videos host on Mediasite)
- [x] [AA_Introduction - applications](#1)
- [x] [BB_Lab summary](#2)
- [x] [CC_Transmitters-Receivers Part1](#3)
- [x] [DD_Transmitters-Receivers Part2 (image etc)](#4)
- [x] EE_Filters Part 1 50ohms & Intro
- [x] FF_Filters Part 2 Poles & Zeros, Butterworth/Chebyshev
- [x] GG_Lumped element filter design method
- [x] HH_Parasitics of lumped elements
- [x] II_Introduction to transmission lines
- [x] IX_Reflections and Transmission Line Resonators
- [x] JJ_Microstrip
- [x] KK_Amplifiers Part 1 - Matching and stability
- [x] LL_Amplifiers part2 - Noise and Distortion
- [x] MM_Transmission Line Theory
- [x] MN_Impedance transformation along a line and the Smith Chart
- [x] MO_LAST LECTURE_Impedance transformation along a line
- [x] NN_Satellite TV receiver
- [x] OO_Mobile Phone and RFIC
- [ ] PP_Measurements
- [ ] ZA_FIRST YEAR CIRCUITS REVISION
- [ ] ZB_FIRST YEAR COMMS REVISION

### PowerPoint Screencasts of the Lectures (in Learning Resources)

- [x] 1_Satellite TV and LNBs.mp4
- [x] 2_SMITH CHART PROGRAMME DEMO.wmv
- [x] 3_TheBigFilterMovie.wmv
- [x] 3_filtermoviemp4_720p.mp4
- [x] 4_Transmitters and receivers part1 EvenBiggerReceiversMovie.mp4
- [x] 5_Image problem and digital multiplexes.mp4
- [x] 6_Parasitics in Ls and Cs.mp4
- [x] 7_Transmission line types.mp4
- [x] 8_Reflections, Standing Waves, Transmission Line Resonators.mp4
- [ ] 9_Amplifier design video.mp4
- [ ] 10_Transmission Line Resonators - filters.mp4
- [ ] 11_Transmission line theory & standing waves.mp4
- [ ] 12_TRL_parameters.mp4
- [ ] 13_Digital communications I and Q in transceivers.mp4

***

&nbsp;  
&nbsp;  
<h2 id="1"></h2>

# Note of *Introduction*
> ### *Relevent Materials:*
> 1d_Intro_done.ppt  
> AA_Introduction - applications

Worksheets x 3
* RF Circuit Design & Simulation

Examples x 2
* Mobile Phone
* Satelite TV

Labs x 3
* Filters & Resonators
* Receivers
* Transmission Lines

## Antenna
- Dishes
- Terrestrial (UHF)
- Sector
- Radar
  - Pulsed Radar &rArr; Distance
  - Doppler Radar &rArr; Speed!
- Adaptive Phased Array (Electronically Steered)
  - Beam Forming Network
  - &rArr; Virtual Phased Array (Synthetic Aperture) &nbsp; **Using Motion**

## Antenna Gain
Omnidirectional = *isotropic*

To steer the wave, use *bulb & parabollic reflector*


The Unit:
<center><p style="font-size:18pt;">dBi</p></center>

> `i` refers to *isotropic*  
> $$G(dBi)=10 \log (\eta \frac{\pi^2 D^2}{\lambda^2})$$


&nbsp;  
&nbsp;  
<h2 id="2"></h2>

# Note of *Lab Summary*

> ### *Relevent Materials:*
> 2_Lab_intro.pptx  
> BB_Lab summary

## Lab
1. LCR Filters
2. LC Resonator & CAD1
3. Superheterodyne(***`adj. 超外差的`***) receiver
    * Mixing
    * Picking up weak signals (recover)
4. Pulses on long transmission lines
    > [!IMPORTANT]
    > Reflections
5. Transmission lines as resonators

> **Microwaves:**  
> Waves guided by metal conductors.  
> e.g. Coaxial cables; Hollow waveguides; Microstrips


## Keysight Agilent ADS
* Circuit simulations
  * Frequency domain linear analysis
  * S-parameters
* Microstrip circuit simulations
  * Multi layer boards
* Frequency domain nonlinear analysis
  * Mixing (Multiplying)
* Electromagnetic simulations
* System level analysis
  * MIMO
  * LTE
  
## Key to this module
1. Transmission Lines
2. Frequency Domain
3. S-Parameters
   


> Standard 50Ohms: Characteristic impedances of cables

&nbsp;  
&nbsp;  
<h2 id="3"></h2>

# Note of *Transmitters&Receivers Part 1*
> ### *Relevent Materials:*
> 5_radioTXRX_part1_done.ppt  
> CC_Transmitters-Receivers Part1

## Basic Digital Transmitter
![Basic Digital Transmitter](3/BasicDigitalTransmitter.png)

## AM Radio Receiver (Demodulation)
![AM Radio Receiver](3/AMRadioReceiver.png)

## Sharpness (Selectivity)
depends on losses in the L and C, **Particularly R<sub>L</sub>**.  

To represent the selectivity, Q is introduced.  

$$Q_{factor}=\frac{Fr}{3dB BandWidth}$$  

Bandwitdh increases proportional to the frequency it is tuned to **squared**.  
(i.e. **BandWidth&uarr;; Q&darr;**)  

![Selectivity](3/Selectivity.png)

## Mixing
is the frequency **translation** to a low frequency for processing.
![Mixer](3/Mixer.png)

 > ## [Prosthaphaeresis 和差化积 (from the Greek προσθαφαίρεσις)](https://en.wikipedia.org/wiki/Prosthaphaeresis)  
 > $$ cosA \times cosB = \frac{1}{2} cos(A-B) + \frac{1}{2} cos(A+B)$$

Thus, in frequency domain, the frequency components are changed into:
![Mixer Frequency](3/MixerFreq.png)

## Superheterodyne Receiver
![Superheterodyne Receiver](3/SuperheterodyneReceiver.png)

Terms:
 - LO : Local Oscillator
 - IF : Intermediate Frequency
 - RF : Radio Frequency
 - LNA : Low Noise Amplifier
 - AMP : Amplifier

Tunning/Changing Channel can be accomplished by tunning **the frequency of Local Oscillator**.

In order to achieve sharp frequency response, IF Filter is a bandpass filter that have **fixed** parameters.

**The LO must be very stable in frequency, and tune-able.**
Thus, some frequency sources introduced.

## SAW Devices (Surface Acoustic Wave)
![SAW Devices](3/SAWDevice.png)

## Also the Crystal Oscillator
Piezoelectric Material 压电材料  
Quartz 石英

## PLL (Phase Lock Loop)
The Oscillators above are very stable but relatively low frequency.
PLL can be used as **Clock Multipliers**.

![PLL](3/PLL.png)

> Phase Comparator  
> knows *almost instantly* when the frequency is drifting out.

Tune the frequency can be easily achieved by changing the factor of **digital divider**.

&nbsp;  
&nbsp;  
<h2 id="4"></h2>

# Note of *Transmitters&Receivers Part 2*
> ### *Relevent Materials:*
> 6_radioTXRX_part2_done.ppt  
> DD_Transmitters-Receivers Part2 (image etc)
> 
# `TODO: Add more notes`