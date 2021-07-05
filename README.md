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

Ex: A resistor is memoryless, since the current i(t) flowing through it in response to the applied voltage v(t) is defined by
![pic1](https://user-images.githubusercontent.com/54907384/124416411-9030e380-dd74-11eb-8aed-cb313be15533.png) where R is resistance of the resistor.</p>

<b>Memory System:</b> <p>
In contrast, the system is said to possess memory if its output signal depends on past or future values of input signal.
These systems are opposite of memory systems.

Ex: An inductor has memory, since the current i(t) flowing through it is related to the applied voltage v(t) by
![pic2](https://user-images.githubusercontent.com/54907384/124416946-bb680280-dd75-11eb-8ff9-a1062a25bb4a.png) where L is inductance of th inductor.</p>

Stability
-----------
Stable System: A system is said to be bounded-input, bounded-output (BIBO) stable (in both continuous-time and discrete-time) if and only if every bounded input results in a bounded output.


i.e., if the output of the system satisfies the condition


whenever the input of the system satisfies the condition


Both Mx and My represent some finite positive numbers.

Unstable system: A system is said to be unstable if it is not a stable system.

Ex: 

Lets assume the input is bounded and satisfies the condition.


Then we can find that



When r ≥ 1, rn increases as n increases and the magnitude of y[n] increases, thus violates the bibo stable condition. So, the system is  unstable.

When r < 1, rn decreases as n increases and the magnitude of y[n] reaches zero, thus satisfiying the bibo stable condition. So, the system is  stable.
Linearity
-----------
Linear system: A system is said to be linear (in both continuous-time and discrete-time) if it satisfies the two properties of superposition and homogeneity.

Superposition: Consider a system that is initially at rest. Let the system be subjected to the input x(t) = 	x1(t), producing an output y(t) = y1(t). Next the same system is subjected to the different input x(t) = x2(t), producing an output y(t) = y2(t). Then for the system to follow superposition property, the corresponding input x(t) = x1(t) + x2(t) should produce corresponding output y(t) = y1(t) + y2(t).

Homogeneity: Consider a system that is initially at rest, and an input x(t) results in output y(t). Then for the system to exhibit the homogeneity property, whenever the system x(t) is scaled by a constant a. The ouput y(t) should also be scaled by the exact constant a (i.e., if input is a.x(t), then output must be a.y(t) ).

Ex: y[n] = n.x[n] is a linear system, because it satisfies both  superposition principle and homogeneity property.

If input x[n] is expressed as weighted sum


then the resulting output will be





Non-linear System: If the system violates either of the superposition principle or homogeneity property, then it is said to be a Non-linear system.



Ex:
y(t) = x(t) + 2t
First we will check superposition theorem
y1(t) = x1(t) + 2t
y2(t) = x2(t) + 2t
y1(t) + y2(t) = x1(t) + x2(t) + 4t

When input x(t) = x1(t) + x2(t),
y(t) = x1(t) + x2(t) + 2t

Since, both are not equal, the system is Non-linear.


Causality
-----------
Causal System: A system is said to be causal (in both continuous-time and discrete-time) if the present value of the output signal depends only on the present or past values of the input signal.

Ex:

Non-causal System: A system is said to be non-causal if it is not a causal system.

Ex: 

Invertibility
-----------
Invertibile System: A system is said to be Invertible (in both continuous-time and discrete-time) if the input of the system can be recovered from the output.
If H is impulse response of a system, then there should exist another system with impulse response Hinv such that 
H.Hinv = I
Where I is a identity operator.



Ex: 
y(t) = 2x(t)

Non-invertibile System: A system is said to be Non-invertible if the input of system is not recoverable. i.e., there doesn’t exist a system with impulse response Hinv.

Ex: 
Time Invariance
-----------
Time invariant system: A System is said to be time invariant if a time delay or time advance of the input signal leads to an identical time shift in the output signal. i.e., the time invariant system responds identically no matter when the signal is applied.
If H is impulse response of the system, and St0 represents a time shift of t0 seconds. Then, time invariant system satisfies

HSt0 = St0H


Ex:
y(t) = t.x(t)

Time variant system: A System is said to time variant if it is not a  time invariant system. i.e., the time delay or time advance of the input may not be identical to the time shift of the output. For the time variant system
HSt0 ≠ St0H

Ex:
y[n] = rnx[n]

LTI Systems
=================

Introduction
-----------
Introduction:
LTI system is composed of 2 types of systems, linear system and time-invariant system, and possess the properties of both systems.
d/dt(c1x1(t)+c2x2(t)) = c1x’1(t) + c2x’2(t)

Impulse response of LTI
-----------
impulse response of a system is its output when presented with a brief input signal, called an impulse. More generally, an impulse response is the reaction of a system in response to some external change.
A linear time-invariant (LTI) system can be represented by its impulse response
If X(t) is the input signal to the system, the output, Y(t), can be written as
Y(t)=-∞∞ h(𝛼)X(t-𝛼) d𝛼 =-∞∞ X(𝛼)h(t-𝛼) d𝛼
    The above integral is called the convolution of h and X, and we write 
Y(t)= h(t)*X(t) = X(t)*h(t)
For discrete-time systems, the output can be written as 
Y[n]= h[n]*X[n] = X[n]*h[n]
-∞∞= h(t)*X(t) = X(t)*h(t) =k = -∞∞h[k]X[n-k]
 =k = -∞∞X[k]h[n-k]

Frequency response of LTI
-----------

Relationship between Frequency and Impulse Response
-----------

Difference equation Representation of LTI System
-----------


Causality
=================

Laplace transform causality constraints
-----------




D

