Signals And Systems
=================

******
To add pictures to the link :

Website for picture, https://img.youtube.com/vi/[---------]/maxresdefault.jpg

For the above link, replace [---------] with youtube link code<br>
Code for this youtube link, https://www.youtube.com/watch?v=FhVQjuAtlTs, code is: FhVQjuAtlTs

<a href="https://github.com/zzossig/hugo-theme-zzo/issues/88" target="_blank">external link</a>

Ex:

[![Watch the video](https://img.youtube.com/vi/4PUcOf0koxw/maxresdefault.jpg)](https://youtu.be/4PUcOf0koxw)

****

Table of contents
=================

<!--ts-->
   * [Signals and systems](#signals-and-systems)
   * [Table of contents](#table-of-contents)
   * [Introduction to Systems](#introduction-to-systems)
     * [What is system?](#what-is-system)
     * [Block Diagram](#block-diagram)
     * [Communication Systems](#communication-systems)
     * [Control Systems](#control-systems)
        * [Open loop](#open-loop)
        * [Closed loop](#closed-loop)
     * [MEMS](#mems)
     * [Remote Sensing](#remote-sensing)
     * [Biomedical Signal Processing](#biomedical-signal-processing)  
     * [Auditory Systems](#auditory-systems)  
   * [Properties Of Systems](#properties-of-systems)
      * [Memory](#memory)
      * [Stability](#stability)
      * [Linearity](#linearity)
      * [Causality](#causality)
      * [Invertibility](#invertibility)
      * [Time Invariance](#time-invariance)
   * [LTI Systems](#lti-systems)
      * [Introduction](#introduction)
      * [Impulse response of LTI](#impulse-response-of-lti)
      * [Frequency response of LTI](#frequency-response-of-lti)
      * [Relationship between Frequency and Impulse Response](#relationship-between-frequency-and-impulse-response)
      * [Difference equation Representation of LTI System](#difference-equation-representation-of-lti-system)
   *
<!--te-->


Properties Of Systems
=================

Memory
-----------

Video:
[![Watch the video](https://img.youtube.com/vi/4PUcOf0koxw/maxresdefault.jpg)](https://youtu.be/4PUcOf0koxw)

Description:

<b>Memoryless system:</b> <p>The system is said to be memoryless (in both continuous-time and discrete-time) if its output signal only depends on the present value of the input signal.
The input from the past and future has no influence on the output of the system.

Ex: A resistor is memoryless, since the current i(t) flowing through it in response to the applied voltage v(t) is defined by <br />
![pic1](https://user-images.githubusercontent.com/54907384/124416411-9030e380-dd74-11eb-8aed-cb313be15533.png) where R is resistance of the resistor.</p>

<b>Memory System:</b> <p>
In contrast, the system is said to possess memory if its output signal depends on past or future values of input signal.
These systems are opposite of memory systems.

Ex: An inductor has memory, since the current i(t) flowing through it is related to the applied voltage v(t) by <br />
![pic2](https://user-images.githubusercontent.com/54907384/124416946-bb680280-dd75-11eb-8ff9-a1062a25bb4a.png) where L is inductance of th inductor.</p>

Stability
-----------
<b>Stable System:</b> <p>A system is said to be bounded-input, bounded-output (BIBO) stable (in both continuous-time and discrete-time) if and only if every bounded input results in a bounded output.

i.e., if the output of the system satisfies the condition 
 ![pic3](https://user-images.githubusercontent.com/54907384/124418668-9ffef680-dd79-11eb-9153-df230707c25b.png) <br />
whenever the input of the system satisfies the condition 
![pic4](https://user-images.githubusercontent.com/54907384/124418710-bb6a0180-dd79-11eb-88ee-6c59c99be411.png) <br />
Both Mx and My represent some finite positive numbers.</p>

<b>Unstable system:</b> <p>A system is said to be unstable if it is not a stable system. <br />
Ex:  ![pic5](https://user-images.githubusercontent.com/54907384/124418772-da689380-dd79-11eb-9fbf-7035ad0d3e57.png)

Lets assume the input is bounded and satisfies the condition.
![pic6](https://user-images.githubusercontent.com/54907384/124418880-0c79f580-dd7a-11eb-9236-2d9232dd810e.png) <br />
Then we can find that
![pic7](https://user-images.githubusercontent.com/54907384/124418897-16035d80-dd7a-11eb-92f8-2e25cc41a655.png) <br />

** When <b>r ≥ 1</b>, rn increases as n increases and the magnitude of y[n] increases, thus violates the bibo stable condition. So, the system is  unstable.

** When <b>r < 1</b>, rn decreases as n increases and the magnitude of y[n] reaches zero, thus satisfiying the bibo stable condition. So, the system is  stable.</p>
  
Linearity
-----------
  <b>Linear system:</b> <p>A system is said to be linear (in both continuous-time and discrete-time) if it satisfies the two properties of superposition and homogeneity.</p>

<b>Superposition:</b> <p>Consider a system that is initially at rest. Let the system be subjected to the input x(t) = 	x1(t), producing an output y(t) = y1(t). Next the same system is subjected to the different input x(t) = x2(t), producing an output y(t) = y2(t). Then for the system to follow superposition property, the corresponding input x(t) = x1(t) + x2(t) should produce corresponding output y(t) = y1(t) + y2(t).</p>

<b>Homogeneity:</b> <p>Consider a system that is initially at rest, and an input x(t) results in output y(t). Then for the system to exhibit the homogeneity property, whenever the system x(t) is scaled by a constant a. The ouput y(t) should also be scaled by the exact constant a (i.e., if input is a.x(t), then output must be a.y(t) ).</p>

Ex: y[n] = n.x[n] is a linear system, because it satisfies both  superposition principle and homogeneity property.

If input x[n] is expressed as weighted sum <br />
![pic8](https://user-images.githubusercontent.com/54907384/124420704-95def700-dd7d-11eb-81a3-8313e6bc3f7f.png) <br />
then the resulting output will be <br />
![pic9](https://user-images.githubusercontent.com/54907384/124420750-a4c5a980-dd7d-11eb-9dd8-6e2accc59f8a.png) <br />
![pic10](https://user-images.githubusercontent.com/54907384/124420785-b60eb600-dd7d-11eb-8606-8feadc43ec50.png)

<b>Non-linear System:</b> <p>If the system violates either of the superposition principle or homogeneity property, then it is said to be a Non-linear system.

Ex:
      y(t) = x(t) + 2t <br />
      First we will check superposition theorem <br />
          y1(t) = x1(t) + 2t <br />
          y2(t) = x2(t) + 2t <br />
          y1(t) + y2(t) = x1(t) + x2(t) + 4t <br />

      When input x(t) = x1(t) + x2(t), <br />
                 y(t) = x1(t) + x2(t) + 2t <br />
Since, both are not equal, the system is Non-linear.</p>

Causality
-----------
<b>Causal System:</b> <p>A system is said to be causal (in both continuous-time and discrete-time) if the present value of the output signal depends only on the present or past values of the input signal.</p>

Ex: ![pic11](https://user-images.githubusercontent.com/54907384/124421206-8f9d4a80-dd7e-11eb-974b-8ccf2831968c.png)

<b>Non-causal System:</b> <p>A system is said to be non-causal if it is not a causal system.</p>

Ex: ![pic12](https://user-images.githubusercontent.com/54907384/124421229-9e83fd00-dd7e-11eb-8172-d2c8f7574ecb.png)

Invertibility
-----------
<b>Invertibile System:</b> <p>A system is said to be Invertible (in both continuous-time and discrete-time) if the input of the system can be recovered from the output. <br />
If H is impulse response of a system, then there should exist another system with impulse response Hinv such that <br />
    ![Screenshot from 2021-07-05 10-50-59](https://user-images.githubusercontent.com/54907384/124421372-f6226880-dd7e-11eb-9483-3f8444f7c725.png)
Where I is a identity operator. <br />

![aaaaa](https://user-images.githubusercontent.com/54907384/124421423-105c4680-dd7f-11eb-9ffe-9cd774f096e3.png)
Ex: 
        y(t) = 2x(t)

<b>Non-invertibile System:</b> A system is said to be Non-invertible if the input of system is not recoverable. i.e., there doesn’t exist a system with impulse response Hinv. 

Ex: ![Screenshot from 2021-07-05 10-52-58](https://user-images.githubusercontent.com/54907384/124421494-308c0580-dd7f-11eb-9bc7-f31b99268fa4.png) </p>

Time Invariance
-----------
<b>Time invariant system:</b> <p>A System is said to be time invariant if a time delay or time advance of the input signal leads to an identical time shift in the output signal. i.e., the time invariant system responds identically no matter when the signal is applied.
If H is impulse response of the system, and St0 represents a time shift of t0 seconds. Then, time invariant system satisfies
![Screenshot from 2021-07-05 10-54-51](https://user-images.githubusercontent.com/54907384/124421610-734ddd80-dd7f-11eb-8bb7-057f73533e27.png)

Ex:
y(t) = t.x(t)

<b>Time variant system:</b> A System is said to time variant if it is not a  time invariant system. i.e., the time delay or time advance of the input may not be identical to the time shift of the output. For the time variant system <br />
![Screenshot from 2021-07-05 10-56-11](https://user-images.githubusercontent.com/54907384/124421725-b14b0180-dd7f-11eb-805a-7778f2c6a81a.png)

Ex:
![Screenshot from 2021-07-05 10-56-17](https://user-images.githubusercontent.com/54907384/124421705-a6906c80-dd7f-11eb-950f-34da4430611c.png)

LTI Systems
=================

Introduction
-----------
LTI system is composed of 2 types of systems, linear system and time-invariant system, and possess the properties of both systems.
d/dt(c1x1(t)+c2x2(t)) = c1x’1(t) + c2x’2(t)

Impulse response of LTI
-----------
<p><b>&emsp;&emsp;impulse response</b> of a system is its output when presented with a brief input signal, called an impulse. More generally, an impulse response is the reaction of a system in response to some external change. <br />
  
  &emsp;A <b>linear time-invariant (LTI)</b> system can be represented by its <b>impulse response</b> 
&emsp;If X(t) is the input signal to the system, the output, Y(t), can be written as <br />
&emsp;&emsp;&emsp; ![Screenshot from 2021-07-05 11-37-14](https://user-images.githubusercontent.com/54907384/124424948-7c41ad80-dd85-11eb-8a04-bf3cac57358d.png) <br />
&emsp;The above integral is called the convolution of h and X, and we write <br />
&emsp;&emsp;&emsp;&emsp;![Screenshot from 2021-07-05 11-37-27](https://user-images.githubusercontent.com/54907384/124425071-a6936b00-dd85-11eb-8a50-d641e96b4fca.png) <br />
  
  &emsp; For <b>discrete-time systems</b>, the output can be written as <br />
  &emsp;&emsp;&emsp;&emsp;![Screenshot from 2021-07-05 11-40-36](https://user-images.githubusercontent.com/54907384/124425213-e22e3500-dd85-11eb-93ca-06a88ba58e90.png) </p>


Frequency response of LTI
-----------
<p>As per video, <b>Frequency response</b> tells how the system responds to <b>sinusoids of different frequencies</b>. <br />
&emsp;&emsp;&emsp;&emsp; ![Screenshot from 2021-07-05 11-42-52](https://user-images.githubusercontent.com/54907384/124425445-30433880-dd86-11eb-9c73-54abdc5d37d3.png)</p>

Relationship between Frequency and Impulse Response
-----------
Relationship between Frequency response and impulse response of the system will be <b>determined by Fourier series and Fourier Transforms</b>.

Difference equation Representation of LTI System
-----------
<p>Mainly, we will see <b>linear constant-coefficient difference / differential equations.</b><br />
  
 &emsp; <b>Linear constant-coefficient differential equation: </b> <br />
 &emsp; &emsp;&emsp;&emsp;&emsp; ![Screenshot from 2021-07-05 11-46-53](https://user-images.githubusercontent.com/54907384/124425842-c4ad9b00-dd86-11eb-9a9d-9b9f607c8ac7.png) <br />
  
  &emsp; <b>Linear constant-coefficient difference equation:</b> <br />
&emsp; &emsp;&emsp;&emsp;&emsp;
![Screenshot from 2021-07-05 11-48-48](https://user-images.githubusercontent.com/54907384/124426008-03dbec00-dd87-11eb-8a80-896636809fd6.png) <br />
&emsp;  The order of the differential or difference equation is (N,M), (Often, N >= M)



Causality
=================

Laplace transform causality constraints
-----------




D

