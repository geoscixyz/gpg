.. _GPR_fundamental_principles

Fundamental Principles
**********************

Here, we present the fundamental principles which govern ground penetrating radar (GPR) signals.
As we mentionned earlier, the source of the GPR system sends a pulse of high-frequency electromagnetic waves (radiowaves) into the Earth.
And as these radiowaves propagate through the Earth, they are distorted due to the Earth's electromagnetic properties.

For radiowaves which are propagating through a homogeneous medium, the associated electric and magnetic fields behave according to the wave equation:

.. math::
	\begin{split}
	\nabla^2 \vec E + k^2 \vec E &= 0 \\
	\nabla^2 \vec H + k^2 \vec H &= 0
	\end{split}


where the properties of the wave (velocity, attenuation, wavelength etc...) are defined by the wavenumber (:math:`k`):

.. math::
	k = \sqrt{-i \omega \mu \sigma + \omega^2 \mu \varepsilon}


Notice that :math:`k` depends on the physical properties of the medium.
Therefore, so do the properties of the wave.

When radiowaves come into contact with an interface (a boundary defined by an abrupt change in the Earth's electromagnetic properties), energy associated with the incoming radiowaves can be reflected, transmitted and/or refracted.
This is illustrated in the figure below.
The reflection, transmission and refraction of radiowaves depends on the electromagnetic properties defining each side of the interface as well as the incident angle of the incoming radiowave signal.

For the purposes of GPR, the Earth may be thought of as a set of homogeneous regions separated by interfaces.
Using signals measured by the receivers, the goal of GPR is to define these interfaces and thus gain information about structures under the Earth.

.. figure:: images_new/GPR_schematic_example.jpg
		:align: center
		:figwidth: 70%

                Schematic of a zero-offset GPR setup.


Wave Velocity
=============

Radiowaves corresponding to GPR signals propagate through different materials at different speeds.
The velocity of radiowaves depends on the physical properties of the medium.
In general, the velocity of radiowaves through a homogeneous material is given by:

.. math::
	V = \sqrt{\frac{2}{\mu \varepsilon}} \Bigg [ 1 + \Bigg ( 1 + \bigg ( \frac{\sigma}{\omega \varepsilon} \bigg )^2 \, \Bigg )^{1/2} \; \Bigg ]^{-1/2}


This equation can be used to show that the velocity of electromagnetic waves is largest in free-space (i.e. when :math:`\sigma = 0`, :math:`\mu = \mu_0` and :math:`\varepsilon = \varepsilon_0`).
Therefore, electromagnetic waves in matter travel slower than the speed of light (c = 2.999 :math:`\times 10^8` m/s).

GPR signals are characterized as being high-frequency.
Thus in many cases (and for this course), it is safe to assume that :math:`\sigma \ll \omega \varepsilon`; especially if the Earth is resistive.
As a result, the velocity of radiowaves can be simplified to:

.. math::
	V = \frac{1}{\sqrt{\mu \varepsilon}} = \frac{c}{\sqrt{\mu_r \varepsilon_r}}


where :math:`\mu_r` is the relative permeability and :math:`\varepsilon_r` is the relative permittivity.
If the propagation material is non-magnetic, then :math:`\mu_r` = 1 and the radiowave velocity simplifies to:

.. math::
	V = \frac{c}{\sqrt{\varepsilon_r}}
	

From this expression, we can see that radiowaves propagate more slowly in increasingly dielectric materials.
A table showing the dielectric permittivity, conductivity and radiowave velocity for various materials can be found :ref:`here <GPR_table_velocity>`.
Notice that:
	
	- Increases water saturation decreases the propagation velocity of sediments
	- Dry rocks and igneous rocks have the high propagation velocity






Attenuation, Skin Depth and Probing Distance
============================================

Attenuation defines the continuous loss of amplitude a wave experiences as it propagates through a particular medium.
The rate at which the amplitude decreases is referred as the attenuation constant.
For an electromagnetic wave that has travelled distance :math:`z`, the attenuation constant (:math:`\alpha`) is defined as follows:

.. math::
	\frac{| \mathbf{A} |}{ | \mathbf{A_0} |} = e^{-\alpha z}

where :math:`\mathbf{A_0}` is the initial amplitude of the wave and :math:`\mathbf{A}` is the amplitude of the wave after it has travel distance :math:`z`.
We can see that as :math:`z \rightarrow \infty`, the amplitude of the wave goes to zero.
Additionally, for larger values of :math:`\alpha`, the wave attenuates more quickly.

The attenuation constant depends on the physical properties of the media.
In general, the attenuation constant can be expressed as:

.. math::
	\alpha = \omega \sqrt{\frac{\mu \varepsilon}{2}} \Bigg [ \Bigg ( 1 + \bigg ( \frac{\sigma}{\omega \varepsilon} \bigg )^2 \Bigg )^{1/2} - \; 1 \; \Bigg ]^{1/2}





**Skin Depth**

Skin depth (:math:`\delta`) defines the propagation distance at which the amplitude of an electromagnetic wave is reduced by a factor of :math:`1/e`; i.e. reduced to 37\% of its original amplitude.
In conductive environments (:math:`\omega \varepsilon \ll \sigma`), a good approximation for  the skin depth is given by:

.. math::
	\delta \approx 500 \sqrt{\dfrac{\rho}{f}}


For materials in which :math:`\omega \varepsilon \gg \sigma`, the skin depth is approximated by:

.. math::
	\delta \approx \frac{5.31 \, \sqrt{\varepsilon}}{\sigma}


**Sigma here is mS/m which to me might be confusing**




**Probing Distance**

Probing distance is used to set to limit 





Reflection and Transmission of Radiowaves
=========================================


.. sidebar:: Normal Incidence Reflection/Transmission

	.. figure:: images/normal_incidence_reflection.gif
		:align: center
		:figwidth: 100%
	
		`Link to source image <https://commons.wikimedia.org/wiki/File:Partial_transmittance.gif>`__


When a radiowave reaches an interface, some of its energy is reflected and some of it is transmitted accross the interface.
This results in both a reflected and a transmitted wave.

The amplitude of the reflected wave proportional to that of the incident wave is defined by the reflection coefficient (:math:`R`).
For radiowaves, the reflection coefficient can be expressed as a function of the dielectric permittivities on each side of the interface.
Assuming the radiowave arrives at an angle perpendicular to the interface, the reflection coefficient is given by:

.. math::
	R = \frac{\textrm{Reflected Amplitude}}{\textrm{Incident Amplitude}} = \frac{\sqrt{\varepsilon_1} - \sqrt{\varepsilon_2}}{\sqrt{\varepsilon_1} + \sqrt{\varepsilon_2}}


The transmission coefficient (the amplitude of the transmitted wave proportional to that of the incident wave) is given by:

.. math::
	T = 1 - R


The reflection coefficient can be either positive or negative and has values between :math:`-1 < R < 1`.
The magnitude of :math:`R` determines how much of the incidend wave is reflected.
The sign determines whether :math:`\varepsilon_1` is greater than or less than :math:`\varepsilon_2` (**not sure if this can be done on radiogram**).

	- :math:`R<0` indicates :math:`\varepsilon_1 < \varepsilon_2`
	- :math:`R>0` indicates :math:`\varepsilon_1 > \varepsilon_2`






**Discuss the importance for relevant senarios**



Refraction of Radiowaves
========================

.. math::
	\frac{\textrm{sin}\theta_1}{V_1} = \frac{\textrm{sin}\theta_2}{V_2}












