.. _GPR_fundamental_principles

Fundamental Principles
**********************


The physics governing ground penetrating radar (GPR) is given by Maxwell's equations:

.. math::
	\begin{split}
	\nabla \times \vec E = -i \omega \mu \vec H \\
	\nabla \times \vec H = \big ( \sigma + i \omega \varepsilon \big ) \vec E
	\end{split}








Wave Velocity
=============

Signals corresponding to GPR propagate through different materials at different speeds.
The velocity of radiowaves depends on the physical properties of the medium.
In general, the velocity of radiowaves through a homogeneous material is given by:

.. math::
	V = \Bigg [ \frac{\mu\varepsilon}{2} \Bigg ( 2 + \bigg ( \frac{\sigma}{\omega \varepsilon} \bigg )^2 \, \Bigg ) \Bigg ]^{-1/2}


GPR signals are characterized as being high-frequency.
Thus in many cases (and for this course), it is safe to assume that :math:`\sigma \ll \omega \varepsilon`.
In this case, the velocity of radiowaves simplifies to:

.. math::
	V = \frac{1}{\sqrt{\mu \varepsilon}} = \frac{c}{\sqrt{\mu_r \varepsilon_r}}

where c is the speed of light.
If the propagation material is non-magnetic, then :math:`\mu_r` = 1 and the radiowave velocity simplifies to:

.. math::
	V = \frac{c}{\sqrt{\varepsilon_r}}
	
	
**Add table for velocities**



Reflection and Transmission of Radiowaves
=========================================

When radio come into contact with a boundary, some of the waves


.. math::
	R = \frac{\sqrt{\varepsilon_1} - \sqrt{\varepsilon_2}}{\sqrt{\varepsilon_1} + \sqrt{\varepsilon_2}}



.. math::
	T = 1 - R



Refraction of Radiowaves
========================

.. math::
	\frac{\textrm{sin}\theta_1}{V_1} = \frac{\textrm{sin}\theta_2}{V_2}



Attenuation of Radiowaves
=========================



















