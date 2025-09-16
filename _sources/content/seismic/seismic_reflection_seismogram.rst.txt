.. _seismic_reflection_seismogram:

Normal Incidence Reflection Seismogram
**************************************


The principles of the normal incidence reflection seismogram are illustrated
in the diagrams below. A source and receiver are at the surface of a layered
earth whose properties are variable. The reflection and transmission
coefficients depend upon the change in acoustic impedance, and thus on both
density and velocity. The travel time for the wave to go from the source to
the reflecting interface and back to the surface depends only upon the length
of the travel path and the velocity of each layer. The travel time formula
given below, is for a wave which travels vertically and for which the source
and receiver are coincident. (The source and receiver are offset slightly in
the diagram for visual clarity). This produces the "normal incidence"
seismogram.

The procedure for generating the ideal seismogram is as follows:

(a) Begin with a geologic section.

(b) Compute the acoustic impedance as a function of depth by taking the product of the density and velocity logs

(c) Compute the reflection (and transmission) coefficients as a function of
    depth. This yields a reflection log.

(d) Convert to time. Each layer has a defined velocity. The incremental (two-
    way) travel time on each layer is :math:`\Delta t_i = 2h_i / v_i`. This
    yields a reflection function on the two-way travel time domain.

(e) Convolve the reflectivity function with a source wavelet. This yields the
    desired ideal seismogram.

The figure below illustrates the procedure:

.. figure:: ./images/three_layer_schematic.gif
	:align: right
	:scale: 110 %


The acoustic impedance for the ith layer is given by:

.. math::
   Z_i = \rho_{i} v_{i}

If the amplitude of the incident ray is :math:`A_0` and the amplitude of
reflection is :math:`A_1`, then the reflection coefficient :math:`R` is
:math:`A_1/A_0`. Similarly, if the amplitude of the transmitted wave is 
:math:`A_2`, then the transmission coefficient :math:`T` is
:math:`A_2/A_0`. 

.. figure:: ./images/Reflection_Transmission.jpg
    :align: center
    :scale: 70 %

Using boundary conditions to ensure the continuity of
stresses and displacements at the interface between we can express the 
reflection and transmission coefficients in terms of the acoustic 
impedance. Where :math:`i` denotes the layer the wave is in and :math:`j` 
denotes the layer that the transmitted wave passes into.       

.. math::
	R_{i,j} =\frac{Z_{j} - Z_{i}}{Z_{j} + Z_{i}}

and

.. math::
   T_{i,j} = \frac{2Z_i}{Z_{j} + Z_{i}}


Given the amplitude of the incident wave :math:`A_0` you can calculate the 
amplitude of a transmitted of reflected waves in any layer. For example, 
the amplitude of the transmitted wave in the 3rd layer is equal to 
:math:`A_0 T_{1,2} T_{2,3} = A_2 T_{2,3}` and the amplitude of the reflected 
wave from the top of the 3rd layer in the 1st layer is 
:math:`A_0 T_{1,2} R_{2,3} T_{2,1}`.

We then convert the reflectivity log from reflectivity as a function of depth 
to reflectivity as a function of time. The total travel time is the sum of 
the incremental times for a particular reflection. The incremental 2 way travel 
time for layer :math:`i` is:

.. math::
	\Delta  t_i = \frac{2h_i}{v}


The normal incidence seismic trace is then obtained by the convolution of a seismic
wavelet (input pulse) with the reflectivity function. The amplitude of each
spike on the reflectivity function is determined by the value of the calculated 
reflection and transmission coefficients. The times for each reflection event are 
obtained by knowing the layer thickness and velocities. Each impulse on the 
reflection function generates a scaled replication of the seismic wavelet. The 
composite of all of the reflection events generates the seismic trace.

.. figure:: ./images/logs.gif
	:align: center
	:scale: 100%

	The reflection seismogram viewed as the convolved output of a reflectivity function with an input pulse. [#f1]_  

Notice how the negative reflection coefficients change the polarity of the
signal recorded at the receiver.

.. figure:: ./images/synthetic_seismogram.gif
	:align: center
	:scale: 100%

	A synthetic seismogram. [#f1]_

.. [#f1] From Kearey, Philip and Micheal Brooks, "An Introduction to Geophysical Exploration". 2nd ed. Blackwell Science: 1991. 

.. <<place holder>> This comment is a placeholder for the "understanding negative reflection and differences in velocities" applet.