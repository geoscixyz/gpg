.. _GPR_processing

Processing
**********

So far, we have used radargrams to represent the data collect by GPR sensors.
In order to create these images, some processing is required.
Here, we discuss how raw GPR data are used to create radargrams.
We will also talk about some source of noise which must be accounted for when attempting to generate radargrams.




	- Noise 
	- Stacking
	- Gain
	- Smoothing
	- Averaging
	- Ringing







Gain Correction
===============

.. figure:: images_new/GPR_gain_time_function.png
	:align: right
	:figwidth: 40%
	
	Example gain function which corrects for a loss in signal strength at later times.


Signals measured at earlier times are much stronger than signals which are measured at later times.
As a result, it may not be easy to distinguish important features in the data at later times.
To account for this, the raw data :math:`d_{raw}(t)` for each reading is multiplied by a gain function :math:`g(t)` as follows:

.. math::
	d(t) = g(t) \times d_{raw}(t)


where :math:`d(t)` is the data represented in the radargram.
The gain function itself is a positive function which increases in magnitude as a function of :math:`t`.
An example of the gain function is shown on the right.
As we can see, the gain function increases in value exponentially to account for the exponential loss in return signal strength over time.
However, the gain function is generally bounded by a maximum value.

.. figure:: images_new/GPR_gain_signal.png
	:align: center
	:figwidth: 100%
	
	(Left) Single trace before gain correction. (Right) Single trace after gain correction.


The strength of returning signals is also much weaker at distances further away from the source.
Because of this, gain corrections may be applied based on Tx-Rx distance.
This is not necessary for common offset surveys, but may be important in common midpoint or transillumination surveys.


Stacking
========

Generally speaking, stacking refers to the amalgamation of separate traces, in order to reduce noise and improve interpretation.


Stacking (Averaging) Individual Readings
----------------------------------------

The stacking of individual readings is used to improve the signal to noise ratio by reducing incoherent noise.
In order to apply this type of stacking:

1) Multiple traces are obtained for the same Tx-Rx location (i.e. multiple readings).

2) The traces are then averaged.

What results from this process is a clearer picture of the GPR signals we are intending to investigate.
By averaging the data in this fashion, we ultimately reduce the coherent noise relative to the signal.
An example of this is demonstrated below.


.. figure:: images_new/GPR_stacking_times.png
	:align: center
	:figwidth: 100%
	
	Example of how averaging multiple traces from the same Tx-Rx pair can improve the signal to noise ratio. This results in an improved image of the returning signal.




Stacking (Averaging) Neighbouring Traces
----------------------------------------








Smoothing
=========

Smoothing is another technique used to improve the interpretation of field collected data.
This technique has the advantage over stacking individual readings because it requires the collection of less data.




.. figure:: images_new/GPR_averaging_times.png
	:align: center
	:figwidth: 100%
	
	Example of smoothing a trace by using a moving average.









