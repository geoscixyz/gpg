.. _GPR_survey_data

Survey and Data
***************

Here, we discuss the various survey geometries used in GPR and some of their applications.
Radargrams will be used to show the data we expect to see in each case.

Depending of the goal or the GPR survey, certain configurations may be more effective.


Furthermore, interpretation of GPR data is made significantly easier by using an appropriate survey configuration.

On this page you will learn about:

	- Commonly used GPR survey configurations and their applications
	- The data collected by GPR surveys
	- The source signal


Common Survey Geometries
========================

Introduction

Common Offset Survey
--------------------

	.. figure:: images_new/GPR_common_offset.png
		:align: right
		:figwidth: 40%

        	Common offset survey configuration.

Common offset surveys are the most frequently used configuration for GPR surveys.
In common offset survey, the distance between the transmitter and a single receiver is fixed.
Data are collected each time the transmitter-receiver pair are moved to a new position.
In some cases, the transmitter and receiver are placed at a zero-offset; otherwise known as a coincident source and receiver.

Common-offset surveys are effective for locating the depths of near-horizontal interfaces.
In addition, zero-offset surveys are very affective a locating pipes, tunnels and compact buried objects; as they generate hyperbolic signatures in radargram data.
Examples of this can be seen below.




**Example: Buried Compact Object**


Below we see a radargram for a zero-offset survey, which shows an obvious hyperbola.
For this example, the hyperbola corresponds to a buried pipe.


.. figure:: images_new/GPR_example_buried_object.png
	:align: center
	:figwidth: 100%

        (Left) Radargram for a zero-offset survey showing hyperbola from a buried pipe. (Right) Geometry showing the path of the radiowave at each reading.


.. figure:: images_new/GPR_example_buried_object_2.png
	:align: right
	:figwidth: 50%

	Geometry shown how radargram can be used to find propagation velocity.


According to the geometry of the problem (above-right), the total travel time of the GPR signal is given by:

.. math::
	t = \frac{2 \big ( x^2 + d^2 \big )^{1/2}}{V}


Now examine the figure on the right.
The top of the parabola corresponds to the horizontal location of the buried object (:math:`x_0`).
The minimum travel time (when the source and receiver are directly above) is given by:

.. math::
	t_0 = 2d/V


Using this to re-write the previous expression, we see that:

.. math::
	V = \frac{4x^2}{t^2 - t_0^2}


Therefore by determining :math:`t_0`, **any point** on the hyperbola can be used to determine the propagation velocity of the top layer.
This may come in handy when a portion of the hyperbola is obstructed by other signals.
Also note that once :math:`V` is determined, the definition of :math:`t_0` can be used to determine the depth of the object.


**Example: Dipping Layers**




Common Midpoint Survey
----------------------

        .. figure:: images_new/GPR_common_midpoint.png
		:align: right
		:figwidth: 40%
	
		Common midpoint survey configuration.
		

For this configuration, the distance between the transmitter and receiver are changed for every reading.
However, the halfway point between the transmitter and the receiver is kept the same.
As we will show, common midpoint surveys are useful for determining the top-layer velocity and thickness.

From the survey schematic, we see that if the interface is approximately flat, the point of reflection is the same for all readings.
As a result, the signal from the reflected wave in the radargram should form a hyperbola.

.. figure:: images_new/GPR_example_buried_object_2.png
	:align: right
	:figwidth: 50%

	Geometry shown how radargram can be used to find propagation velocity.


Once again, the travel time for the radiowave signal is given by:

.. math::
	t = \frac{2 \big ( x^2 + d^2 \big )^{1/2}}{V}


where :math:`d` is the thickness of the top layer and :math:`x` is the distance between the mid-point and either the transmitter or the receiver.
Once again by defining :math:`t_0 = 2d/V`, the top-layer velocity is given by:

.. math::
	V = \frac{4x^2}{t^2 - t_0^2}


Thus, **any point** on the parabola can be used to determine the top-layer velocity from a common mid-point survey.
And once :math:`V` is determined, the definition of :math:`t_0` can be used to obtain the thickness of the top layer.


	.. figure:: images_new/GPR_survey_transillumination.jpg
		:align: right
		:figwidth: 40%
	
	        (A) Mine-shaft structural integrity (B) Borehole survey. (C) Concrete pillar testing.


Transillumination Survey
------------------------

When performing a transillumination GPR survey, multiple transmitters and receivers are placed on either side of an region of interest.
There are many applications for transillumination surveys, some of which are mentionned here.

In panel (A), a transillumination survey is being used to assess the structural integrity between two mine shafts.
By using GPR, we can determine if there are void spaces between the mine shafts or any potential planes of weakness.
The information collected can be used to assure the mine shaft is safe.

In panel (B), we see a transillumination borehole survey.
In some cases, a surface survey may not supply sufficient information about a particular region of interest.
Although it is more expensive and time-consuming, this type of survey may be required.

In panel (C), a GPR transmitter and receiver are placed on opposing sides of an object; in this case, a concrete pillar.
This represents a non-invasive approach for determining internal structures.






.. sidebar:: Wavelet Example

	.. figure:: images_new/GPR_wavelet_example.png
		:align: center
		:figwidth: 100%
		
		Example of a wavelet signal.
	
	.. figure:: images_new/GPR_wavelet_frequencies_example.png
		:align: center
		:figwidth: 100%
			
		Band of frequencies for a particular wavelet.


Source Signal
=============


As we have already discussed, the source attena sends a pulse of radiowaves into the ground.
This pulse however, is not made up entirely of radiowaves of a single frequency.
Instead, a set of sinusoidal waves of different frequencies are used create what is called a wavelet.
As a result, the wavelet contains information over a range of frequencies (generally between :math:`10^6` and :math:`10^9` Hz).

Before we move forward let us define a few terms:

	- **Wavelet**: A wave-like oscillation of short duration.
	- **Bandwidth**: The range of frequencies present in the source wavelet.
	- **Pulse Width**: The time duration of the wavelet.
	- **Spatial Length**: The physical length of the wavelet signal while it propagates through a medium.
	- **Central Frequency**: The central frequency corresponding to the bandwidth. In general, the central frequency defines the propagation of the GPR signal.


GPR Signals and Bandwidth
-------------------------

The figure below can be used to examine the relationships between the 5 aforementionned terms.
As we can see, the bandwidth and central frequency for the GPR signal depends on the pulse width of the wavelet.
Here are a few important relationships to keep in mind:

**1)** For a pulse width :math:`\Delta t`, the central frequency :math:`f_c` is given by:

.. math::
	f_c = \frac{1}{\Delta t}


As a result, longer wavelets generally contain lower-frequency information.
Frequencies corresponding to GPR signal are around 100 MHz to 1 GHz.
This results in pulse widths around 1 ns to 10 ns.

**2) The bandwidth increases as the pulse width decreases.**
In order to create a wavelet with a longer pulse width, only frequencies near the central frequency are needed.
However, a large range of frequencies (or bandwidth) is needed to create wavelets that have short pulse widths.

**3) The spatial length increases as the pulse with increases**.
As we can see from the figure below, the "wave envelope" is longer for wavelets that have a long pulse width.



.. figure:: images_new/GPR_pulse_bandwidth.png
		:align: center
		:figwidth: 65%

                


Survey Resolution and Probing Distance
--------------------------------------


.. sidebar:: Radargrams at Several Resolutions (Underground tunnels)

	.. figure:: images_new/GPR_resolution_low.jpg
		:align: center
	
		Low resolution radargram (50 MHz).

	.. figure:: images_new/GPR_resolution_mid.jpg
		:align: center
		
		Low resolution radargram (100 MHz).
	
	.. figure:: images_new/GPR_resolution_high.jpg
		:align: center
		
		Low resolution radargram (200 MHz).


The pulse width, and thus the frequency content contained within the GPR signal, is a very important aspect of planning a GPR survey.
Here, we will show that there is a compromise between the resolution of the radargram and the penetration depth of the signal.


