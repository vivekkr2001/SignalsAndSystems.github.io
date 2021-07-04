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
   * [Causality](#causality)
      * [Laplace transform causality constraints](#laplace-transform-causality-constraints)
      * [Z transform and causality, stability](#z-transform-and-causality-stability)
   * [Integration of Systems](#integration-of-systems)
      * [Cascading](#cascading)
      * [Parallel](#parallel)
      * [Feedback](#feedback)
<!--te-->

Introduction to Systems
=================

What is system?
-----------




Description:

In this Video, he described the system as a source which manipulates the given input signal. With a system we can perform many operations on input signals and get the desired output.
He also mentioned the types 0f systems which are continuous and discrete systems. And then he discusses them.


Block Diagram
-----------




Description:

Lecture is about how to represent the signal transformation using a block diagram. He described every block for a particular operation. 

Block diagram consists of : 

Blocks – these represent subsystems – typically modeled by, and labeled with, a transfer function

 Signals – inputs and outputs of blocks – signal direction indicated by arrows – could be voltage, velocity, force, etc.

 Summing junctions – points were signals are algebraically summed –subtraction indicated by a negative sign near where the signal joins the
summing junction.
For adding signals we use summation junctions and also closed loop systems for performing iterative operations on the input signals. This lecture covers block diagrams used to represent control systems, methods of manipulation of block diagrams (including an Example) as well as covering steady state errors and their determination.


Communication Systems
-----------




Description:

In this video, we can understand the basic structure of communication systems with a block diagram.
Below is the block diagram of the communication system.


Communication is the exchange of information between the two or more points.
Electronics point of view, it is the exchange of information using the electronic device or gadget between two or more points which can be far away from each other.

The communication system contains the following basic blocks:

1) The Source
2) Input Transducer
3) Transmitter
4) Channel 
5) Receiver
6) Output Transducer

Source:
The source is the origin from where the message signal is generated.
The message could be voice signal, email, Television Signal, or data.

Input Transducer:
Using the input transducer, the message signal is converted into the electrical signal.

Transmitter:
The transmitter signal modifies the input signal for efficient transmission.
The transmitter may contain several subsystems like modulator, analog to digital converter, encoder, amplifier etc.

Channel:
The channel is the medium over which the transmitted signal is transmitted.
The channel could be physical channel (e.g optical fiber, coaxial cable) or wireless channel (radio link)
The channel partly behaves like a filter and attenuates and distorts the transmitted signal.

The receiver:
For faithful communication, the receiver should be able to recover the message signal from the received (distorted and attenuated) signal.
The receiver also contains several subsystems like, demodulator, decoder, digital to analog converter, amplifier.

Output Transducer:
The output of the receiver is given to the output transducer. Speaker, monitor screen are examples of the output transducer.



Control Systems
-----------




Description:

This video is about the control systems and their types, A control system is a mechanical state that alters the future state of a system. 
Control system is of two types:
Open loop 
Closed loop

Open loop
-----------
In this system, input signal is not controlled by any feedback from output or conditions. The system is automatic. It continues to alter the input until the given time. Example: Dishwasher which  keeps on cleaning the dishes until the timer stops, it doesn't check whether the dish is clean or not. Once the timer stops it discontinues the process.

Closed loop
-----------
In this system, it has a regulation for the input before altering in the plant unlike open loop, closed loop system controls the input signal through feedback system.

MEMS
-----------




Description:

Micro Electro-Mechanical Systems are devices built with micro sensors and mechanical parts along signal processing circuits. These devices provide a channel between computing systems and the physical world. Basic I/O ’s are built using MEMS. They provide I/O to information systems like sensing and creating motion, radio waves etc. 
The distinctive features of MEMS :
Miniaturization 
Multiplicity
Microelectronics.


Remote Sensing
-----------




Description:

In this video, we learn about the term remote sensing. As it was coined by the US scientist Evelyn L. Pruitt, the term remote sensing means understanding or studying the information of the characteristics of an object or phenomena through a recording device without any physical contact.



Biomedical Signal Processing
-----------




Description:

Biomedical signals are the observations of physical activities of various human body systems. Biomedical signals have two characteristics, they are: number of points used to collect data, type of potential. And also discussed the processing of a biomedical signal.
 
Block diagram of biomedical signal processing:




Auditory Systems
-----------




Description:

The human auditory system is composed of three parts. The outer ear , the middle ear and the inner ear. Let's see how it works. 

The sound waves are picked up by the ear pavilion of the outer ear . They are then amplified and transmitted to the middle ear through the external ear canal . This movement of the sound makes this small membrane called the eardrum vibrate.  

These vibrations are transmitted to the ossicles located in the middle ear. The ossicles are the smallest bones in the human body.  They are composed of the malleus, which transmits the vibrations to the incus then to the stapes which acts as a piston that compresses the fluid of the inner ear . 

The cochlea is the main organ of auditory perception.  It contains between 15 to 20 thousand hair cells that detect vibrations of the liquid and generate nerve impulses that are sent to the brain via the auditory nerve.

But this system is fragile and can suffer failures, we call this hearing loss two of which are conduction hearing loss and sensorineural hearing loss. 

Conduction hearing loss can be caused by an obstruction in the ear canal , such as ear wax, a perforated eardrum , a malfunction of the ossicles , otitis or fluid in the middle ear. This type of loss can often be resolved by medical intervention and represents only 10 % of cases of hearing loss.

The second type of loss, sensorineural hearing loss represents 90 % of cases. It results from the destruction of hair cells in the cochlea. It is often due to aging, can be genetic or the consequence of repeated exposure to very loud sound. This type of loss is irreversible, yes, it's a shame, but can often be compensated by hearing aids.


Properties Of Systems
=================

Memory
-----------

Video:
[![Watch the video](https://img.youtube.com/vi/4PUcOf0koxw/maxresdefault.jpg)](https://youtu.be/4PUcOf0koxw)

Description:

Memoryless system: The system is said to be memoryless (in both continuous-time and discrete-time) if its output signal only depends on the present value of the input signal.
The input from the past and future has no influence on the output of the system.

Ex: A resistor is memoryless, since the current i(t) flowing through it in response to the applied voltage v(t) is defined by


     
where R is resistance of the resistor.


Stability
-----------

Linearity
-----------

Causality
-----------

Invertibility
-----------

Time Invariance
-----------

LTI Systems
=================

Introduction
-----------

Impulse response of LTI
-----------

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




Description:

In this video, we learn about laplace transform conditions for a system to be causal. 
For a system h(t) to be causal h(t) = 0, t < 0
For a system h(t) to be stable it needs to satisfy BIBO condition,  -∞∞ h(t)dt < ∞ 
Causal systems are regions of convergence in s domain that are right sided including infinity conditions.
	I.e, laplace transform X(s) =  
  		=0∞ h(t)e-stdt;


Z transform and causality, stability
-----------




Description:

In this video, we learn that a discrete time LTI system with function H(z) is causal if and only if the ROC is the exterior of a circle outside the outermost pole. 

A causal LTI system with function H(z) is stable if and only if 
all the poles of H(z) lie inside the unit circle, i.e, they all must have magnitude smaller than 1. 
An LTI system is stable if and only if the ROC of its system function H(z) includes the unit circle |z| = 1.



Integration of Systems
=================

Cascading
-----------




Description:

A cascaded system is a series or sequential arrangement of objects. In the video, measuring the resultant response of the system in a general cascaded system. 
H(z) = H1(z) x H2(z) x ….. x Hn(z).


Parallel
-----------




Description:

A Parallel system is a parallel arrangement of objects. In the video, measuring the resultant response of the system in a general cascaded system.
H(z) = H1(z) + H2(z) + H3(z) +...... + Hn(z).


Feedback
-----------




Description:

Back in 1920, Bell Labs proposed the theory of feedback where the output is given as a limiter or remainder for the flow of input so that we can control the input and system. 
Feedback is the design technique where a portion of the amplifier output "feeds back" to the input of the amplifier. The overall effect creates a very stable gain factor determined by resistor ratios.



