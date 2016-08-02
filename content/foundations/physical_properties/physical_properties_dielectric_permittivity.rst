.. _physical_properties_dielectric_permittivity:

Dielectric Permittivity
***********************

The dielectric permittivity (:math:`\varepsilon`) represents an important diagnostic physical property in ground-penetrating radar; as the attenuation and velocity of electromagnetic waves associated this survey method are strongly dependent on the dielectric permittivity.
Dielectric permittivity is defined as the ratio between the electric field (:math:`\vec E`) within a dielectric material and the corresponding electric displacement (:math:`\vec D`):

.. math::
	\vec D = \varepsilon \vec E

When exposed to an electric field, the average position of positive and negative charges within most materials become slightly separated.
This separation results in a net electric polarization (:math:`\vec P`) within the material.
The electric field, electric displacement and electric polarization are related by the following expression:

.. math::
	\vec D = \varepsilon_0 \vec E + \vec P
	

where the permeability of free-space (:math:`\varepsilon_0 = 8.8541878176 \times 10^{-12}` F/m) defines the relationship between :math:`\vec D` and :math:`\vec E` if the electric polarization were zero.
Therefore, the dielectric permittivity and the electric displacement define how strongly a material becomes electrically polarized under the influence of an electric field.

**Relative Permittivity**: The dielectric properties of a material are frequently expressed using the relative permittivity (:math:`\varepsilon_r`), where:

.. math::
	\varepsilon_r = \frac{\varepsilon}{\varepsilon_0}
	

**Dielectric Permittivity and Frequency-Dependence**: The electric polarization which is generated within dielectric materials does not occur instantaneously and depends on the frequency of the electric field.
Therefore, the dielectric permittivity must be expressed as a frequency-dependent quantity with both a real part (:math:`\varepsilon^\prime`) and an imaginary part (:math:`\varepsilon^{\prime\prime}`):

.. math::
	\varepsilon (\omega) = \varepsilon^\prime (\omega) + i \varepsilon^{\prime\prime} (\omega)


where :math:`i = \sqrt{-1}`.

- Significance of Re and Im to energy storage and dissipation

- That generally, permittivity decreases as frequency increases



.. math::
	\vec E &: \textrm{Electric Field ()} \\
	\vec D &: \textrm{Electric Displacement ()} \\
	\vec P &: \textrm{Electric Polarization ()} \\
	\varepsilon &:\textrm{ Dielectric permittivity (F/m)} \\
	\varepsilon_0 &:\textrm{ Permittivity of free-space ( = 8.8541878176 10}^{-12}\textrm{ F/m)} \\
	\varepsilon_r &:\textrm{ Relative permittivity ((F/m)/(F/m))} \\
	\varepsilon^\prime &:\textrm{ Real permittivity} \\
	\varepsilon^{\prime\prime} &:\textrm{ Imaginary permittivity} 
	



Measurements for Dielectric Permittivity
========================================

- Experiment by using the material to fill a parallel plate capacitor





Electrical Permittivity for Common Rocks
========================================

- Really need to define specifically what the numbers mean.

- Usually, the numbers represent the real component at a particularly relevant frequency




Factors Impacting Electric Permittivity
=======================================



**Water**:





xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

**Dielectric permittivity  :math:`(\epsilon)`:** This physical property
quantifies how easily material becomes polarized in the presence of an
electric field. The permittivity of free space is :math:`\epsilon_0 =
8.8541878176 10^{-12} F/m`, a "Farad" (F) is the unit of capacitance,
named after Michael Faraday. If free space did not have finite permittivity,
electromagnetic waves (light, radio, etc) could not propagate in free space.

**Relative dielectric permittivity :math:`(\epsilon_R)`:** Relative dielectric
permittivity is a ratio: since dielectric permittivity :math:`\epsilon =
\epsilon_R \epsilon_0`, relative dielectric permittivity :math:`\epsilon_R
= \epsilon / \epsilon_0`.

 
Relative dielectric permittivity is the parameter usually referred to in GPR
work. It is 1 (one) for free space or air, and 80 for water. Because it is a
number that compares true value to free space value, it has no units.

Dielectric permittivity is in fact a complex value, often written :math:`
\epsilon_R = \epsilon_R^{\prime} - i\epsilon_R^{\prime\prime}` . It can
be considered as a measure of the extent to which charge distribution can be
distorted or polarized by an applied electric field.


The so-called "real" part, :math:`\epsilon_r^{\prime}` , is the *relative
dielectric constant* , often introduced in electronics or physics
courses in the context of capacitors. It is a storage component measured as
capacitance per unit length. (Capacitance is "the amount of charge a material
can hold" for a given applied voltage.) At different frequencies, polarization
occurs at different scales: at very high frequencies, only subatomic particles
can be polarized. At GPR frequencies, the reorientation of dipolar molecules
is the largest contribution, hence water's importance in determining the
velocity of EM waves in a material. Note that :math:`\epsilon_R = 80` for
water, whereas :math:`\epsilon_R < 10` for most other common materials.

 .. figure:: ./images/images_duplicates/dielectric_responses.jpg
	:align: center
	:scale: 100 %

	A dielectric permittivity spectrum over a wide range of frequencies, for real (top curve) and "imaginary" (bottom curve) components. Borrowed from `Wikipedia Dielectric Permittivity Article`_.

The so-called "imaginary" part, :math:`\epsilon_r^{\prime\prime}`,  is a loss
component that generally indicates how much energy is dissipated at the
transition from one polarization mechanism to another. The behaviour of both
is shown in the figure. Values are relatively constant for GPR frequencies of
:math:`10^6` through :math:`10^9` , ensuring that wave behaviour is not
dispersive; i.e. all frequency components of a broad band signal travel at the
same speed.

The dielectric permittivity of most geological materials is closely dependent
upon the amount of water (free or otherwise) in the material. Values of
:math:`\epsilon_R` for geologic materials range from 1 to 80, as seen in the
table above.

.. _Wikipedia Dielectric Permittivity Article: https://en.wikipedia.org/wiki/Permittivity
