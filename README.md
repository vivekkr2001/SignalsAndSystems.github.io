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
   * [Integration of Systems](#integration-of-systems)
      * [Cascading](#cascading)
      * [Parallel](#parallel)
      * [Feedback](#feedback)
<!--te-->

Introduction to Systems
=================

What is system?
-----------

<b>Video: </b> <br>
[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/fxGZ7GRQMsk/0.jpg)](http://www.youtube.com/watch?v=fxGZ7GRQMsk)

Time stamps: <br>
&nbsp;&nbsp; 0:34 - 1:55 Introduction <br>
&nbsp;&nbsp; 1:56 - 4:51 Types of Systems <br>

<b> Description: </b> <br>
<p>
In this Video, he described the system as a source which manipulates the given input signal. With a system we can perform many operations on input signals and get the desired output.
He also mentioned the types 0f systems which are continuous and discrete systems. And then he discusses them.
</p>
Block Diagram
-----------

<b>Video: </b> <br>
[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/X4hPVxZlrPU/1.jpg)](http://www.youtube.com/watch?v=X4hPVxZlrPU)

Time Stamps: <br>
&nbsp;&nbsp; 0:42 - 4:22 Introduction of the Mechanism of Block Diagrams <br>

<b>Description:</b> <br>
<p>
Lecture is about how to represent the signal transformation using a block diagram. He described every block for a particular operation. 

Block diagram consists of : 

Blocks – these represent subsystems – typically modeled by, and labeled with, a transfer function

Signals – inputs and outputs of blocks – signal direction indicated by arrows – could be voltage, velocity, force, etc.

Summing junctions – points were signals are algebraically summed –subtraction indicated by a negative sign near where the signal joins the
summing junction.
For adding signals we use summation junctions and also closed loop systems for performing iterative operations on the input signals. This lecture covers block diagrams used to represent control systems, methods of manipulation of block diagrams (including an Example) as well as covering steady state errors and their determination.
</p>


Communication Systems
-----------

<b>Video: </b> <br>
[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/qhjj6WG7Rgc/2.jpg)](http://www.youtube.com/watch?v=qhjj6WG7Rgc)

Time Stamps: <br>
&nbsp;&nbsp; 1:34 - 8:32 Basic Structure of Block Diagrams <br>

<b>Description:</b> <br>
<p>
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


</p>

Control Systems
-----------

<b>Video: </b> <br>
[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/O-OqgFE9SD4/3.jpg)](http://www.youtube.com/watch?v=O-OqgFE9SD4)

Time Stamps: <br>
&nbsp;&nbsp; 0:00 - 1:14 Open Loop
&nbsp;&nbsp; 3:38 - 4:10 Closed Loop

<b>Description:</b> <br>
<p>
This video is about the control systems and their types, A control system is a mechanical state that alters the future state of a system. 
Control system is of two types:
Open loop 
Closed loop

Open loop: 
In this system, input signal is not controlled by any feedback from output or conditions. The system is automatic. It continues to alter the input until the given time. Example: Dishwasher which  keeps on cleaning the dishes until the timer stops, it doesn't check whether the dish is clean or not. Once the timer stops it discontinues the process.

Closed loop:
	In this system, it has a regulation for the input before altering in the plant unlike open loop, closed loop system controls the input signal through feedback system.

</p>

MEMS
-----------

<b>Video: </b><br>
[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/j9y0gfN9WMg/4.jpg)](http://www.youtube.com/watch?v=j9y0gfN9WMg)

Time Stamps: <br>
&nbsp;&nbsp; 26:24 - 29:32 Characteristics of MEMS

<b>Description:</b> <br>
<p>
Micro Electro-Mechanical Systems are devices built with micro sensors and mechanical parts along signal processing circuits. These devices provide a channel between computing systems and the physical world. Basic I/O ’s are built using MEMS. They provide I/O to information systems like sensing and creating motion, radio waves etc. 
The distinctive features of MEMS :
1. Miniaturization 
2. Multiplicity
3. Microelectronics.

</p>


Remote Sensing
-----------

Auditory Systems
-----------

Properties Of Systems
=================

Memory
-----------

Video:
[![Watch the video](https://img.youtube.com/vi/4PUcOf0koxw/maxresdefault1.jpg)](https://youtu.be/4PUcOf0koxw)

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

Integration of Systems
=================

Cascading
-----------

Parallel
-----------

Feedback
-----------
