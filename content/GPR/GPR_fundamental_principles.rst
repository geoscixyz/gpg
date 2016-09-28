.. _GPR_fundamental_principles

Fundamental Principles
**********************

Here, we present the fundamental principles which govern ground penetrating radar (GPR).
As we mentionned earlier, the source of the GPR system sends a pulse of high-frequency electromagnetic waves (radiowaves) into the Earth.


	- 


The physics which govern ground penetrating radar (GPR) can be expressed using Maxwell's equations:

.. math::
	\begin{split}
	&\nabla \times \vec E = -i \omega \mu \vec H \\
	&\nabla \times \vec H = \big ( \sigma + i \omega \varepsilon \big ) \vec E
	\end{split}


For the case where Maxwell's equations are being analyzing within a homogeneous media, the electromagnetic fields behave according to the wave equation:

.. math::
	\begin{split}
	&\nabla^2 \vec E + k^2 \vec E = 0 \\
	&\nabla^2 \vec H + k^2 \vec H = 0
	\end{split}


The behaviour of the wave (velocity, attenuation, etc...) within this media depends on the wavenumber (:math:`k`), where:


.. math::
	k = \sqrt{-i \omega \mu \sigma + \omega^2 \mu \varepsilon}










Wave Velocity
=============

Signals corresponding to GPR propagate through different materials at different speeds.
The velocity of radiowaves depends on the physical properties of the medium.
In general, the velocity of radiowaves through a homogeneous material is given by:

.. math::
	V = \Bigg [ \frac{\mu\varepsilon}{2} \Bigg ( 2 + \bigg ( \frac{\sigma}{\omega \varepsilon} \bigg )^2 \, \Bigg ) \Bigg ]^{-1/2}


This equation can be used to show that the velocity of electromagnetic waves is largest in free-space (i.e. when :math:`\sigma = 0`, :math:`\mu = \mu_0` and :math:`\varepsilon = \varepsilon_0`).
Therefore, electromagnetic waves in matter travel slower than the speed of light (c = 2.999 :math:`\times 10^8` m/s).

GPR signals are characterized as being high-frequency.
Thus in many cases (and for this course), it is safe to assume that :math:`\sigma \ll \omega \varepsilon`.
As a result, the velocity of radiowaves can be simplified to:

.. math::
	V = \frac{1}{\sqrt{\mu \varepsilon}} = \frac{c}{\sqrt{\mu_r \varepsilon_r}}


If the propagation material is non-magnetic, then :math:`\mu_r` = 1 and the radiowave velocity simplifies to:

.. math::
	V = \frac{c}{\sqrt{\varepsilon_r}}
	
	
A table showing the dielectric permittivity of materials and the approximate radiowave velocity can be found here (link to table).



Reflection and Transmission of Radiowaves
=========================================

For ground penetrating radar, physical boundaries exists where changes in the Earth's electromagnetic properties occur abruptly.
These boundaries are known as interfaces.
When radiowaves reach an interface, some of the energy is reflected and the remainder it transmitted accross the interface.


**Normal Incidence**

.. sidebar:: Normal Incidence Reflection/Transmission

	.. figure:: images/normal_incidence_reflection.gif
		:align: center
		:figwidth: 100%
	
		`Link to source image <https://commons.wikimedia.org/wiki/File:Partial_transmittance.gif>`__
	


For normal incidence reflection and transmission, the incoming wave is perpendicular to the surface of the interface.


The reflection coefficient defines the ratio of amplitudes between the reflected wave and the incident wave.
For radiowaves, the reflection coefficient can be expressed as a function of the dielectric permittivities on each side of the interface:

.. math::
	R = \frac{\textrm{Reflected Amplitude}}{\textrm{Incident Amplitude}} = \frac{\sqrt{\varepsilon_1} - \sqrt{\varepsilon_2}}{\sqrt{\varepsilon_1} + \sqrt{\varepsilon_2}}





.. math::
	T = 1 - R



Refraction of Radiowaves
========================

.. math::
	\frac{\textrm{sin}\theta_1}{V_1} = \frac{\textrm{sin}\theta_2}{V_2}



Attenuation of Radiowaves
=========================



















