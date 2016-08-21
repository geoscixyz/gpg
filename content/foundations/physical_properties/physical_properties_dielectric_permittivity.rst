.. _physical_properties_dielectric_permittivity:

Dielectric Permittivity
***********************

The dielectric permittivity (:math:`\varepsilon`) represents an important diagnostic physical property in ground-penetrating radar; as the attenuation, wavelength and velocity of electromagnetic waves associated with this survey method are strongly dependent on the dielectric permittivity.
Dielectric permittivity is defined as the ratio between the electric field (:math:`\vec E`) within a material and the corresponding electric displacement (:math:`\vec D`):


.. figure:: ./images/electric_polarization_physics_diagram.png
	:align: right
	:scale: 40%

.. math::
	\vec D = \varepsilon \vec E

When exposed to an electric field, the average position of positive and negative charges within most materials become slightly separated on an atomic level.
This separation results in a net electric polarization (:math:`\vec P`) within the material.
The electric field, electric displacement and electric polarization are related by the following expression:

.. math::
	\vec D = \varepsilon_0 \vec E + \vec P
	

where the permittivity of free-space (:math:`\varepsilon_0 = 8.8541878176 \times 10^{-12}` F/m) defines the relationship between :math:`\vec D` and :math:`\vec E` if the material is non-polarizable.
Therefore, the dielectric permittivity and the electric displacement define how strongly a material becomes electrically polarized under the influence of an electric field.
The electrical polarization within the material can be defined in terms of the electric field as follows:

.. math::
	\vec P = (\varepsilon - \varepsilon_0 ) \vec E = \chi_e \varepsilon_0 \vec E

where :math:`\chi_e` is known as the electric susceptibility.
The electric susceptibility should not be confused with the magnetic susceptibility, as they describe different physical processes.


**Relative Permittivity**: The dielectric properties of a material are frequently expressed using the relative permittivity (:math:`\varepsilon_r`), where:

.. math::
	\varepsilon_r = \frac{\varepsilon}{\varepsilon_0}
	
	
	
	

**Dielectric Permittivity and Frequency-Dependence**: Electrical polarization mechanisms relevant to ground-penetrating radar depend on the frequency of the electric field.
Therefore, the dielectric permittivity must be expressed as a frequency-dependent quantity with both a real part (:math:`\varepsilon^\prime`) and an imaginary part (:math:`\varepsilon^{\prime\prime}`):


.. math::
	\varepsilon (\omega) = \varepsilon^\prime (\omega) + i \varepsilon^{\prime\prime} (\omega)


where :math:`i = \sqrt{-1}`.
The real component of the dielectric permittivity represents energy stored through electrical polarization whereas the imaginary component represents a measure of energy loss.
The significance of the real and imaginary components of the dielectric permittivity will be discussed in more detail when learning about ground-penetrating radar (link).



.. figure:: ./images/cole_cole_permittivity.png
	:align: right
	:scale: 40%

A widely used model for describing the dielectric permittivity as it relates to ground-penetrating radar is the Cole-Cole model:

.. math::
	\varepsilon (\omega) = \varepsilon_\infty + \frac{\varepsilon_{DC} - \varepsilon_\infty}{1 + (i\omega \tau)^\alpha}


where :math:`\varepsilon_{DC}` is the DC or zero-frequency permittivity, and :math:`\varepsilon_\infty` represents a limit as frequency goes to infinity.
Parameters :math:`\tau` and :math:`\alpha` define the span of frequencies in which the dielectric permittivity changes with respect to frequency.
As we can see from this model:

- Frequency-dependence only occurs over a finite span of frequencies.
- The magnitude of the dielectric permittivity decreases with respect to an increase in frequency.
- At sufficiently low frequencies, the dielectric permittivity is constant and real-valued.


Parameters used to define the dielectric properties of materials and their associated units are tabulated below.



+-------------------------+-----------------------------------+------------------+
| **Property**            | **Symbol**                        | **Units**        |
+=========================+===================================+==================+
| Electric Field          | :math:`\vec E`                    | N/C or V/m       |
+-------------------------+-----------------------------------+------------------+
| Displacement Current    | :math:`\vec D`                    | A/m :math:`\!^2` |
+-------------------------+-----------------------------------+------------------+
| Electric Polarization   | :math:`\vec P`                    | A/m :math:`\!^2` |
+-------------------------+-----------------------------------+------------------+
| Dielectric Permittivity | :math:`\varepsilon`               | F/m              |
+-------------------------+-----------------------------------+------------------+
| Relative Permittivity   | :math:`\varepsilon_r`             | *Unitless        |
+-------------------------+-----------------------------------+------------------+
| Real Permittivity       | :math:`\varepsilon^\prime`        | F/m              |
+-------------------------+-----------------------------------+------------------+
| Imaginary Permittivity  | :math:`\varepsilon^{\prime\prime}`| F/m              |
+-------------------------+-----------------------------------+------------------+
| DC Permittivity         | :math:`\varepsilon_{DC}`          | F/m              |
+-------------------------+-----------------------------------+------------------+
| Infinite Permittivity   | :math:`\varepsilon_\infty`        | F/m              |
+-------------------------+-----------------------------------+------------------+
| Electric Susceptibility | :math:`\chi_e`                    | *Unitsless       |
+-------------------------+-----------------------------------+------------------+




Measurements for Dielectric Permittivity
========================================

- Experiment by using the material to fill a parallel plate capacitor





Electrical Permittivity for Common Rocks
========================================

A table with the approximate relative permittivities for common rock, soils and other materials is shown below.
In order to interpret this table correctly, it is important to understand the following:

- For hard rocks and dry soils, the dielectric permittivity is effectively constant and equal to the DC permittivity :math:`\varepsilon_{DC}` (Butler).
- The frequency-dependence of water-saturated sedimentary rocks and soils is negligible below ~100 MHz and small below ~1 GHz (Kaatze, 1989; Meissner and Wentz, 2004).

As a result, the dielectric properties of rocks are generally given as real-valued.
These constant values accurately describe the dielectric properties of most relevant materials below ~100 MHz and offer a reasonable approximation below ~1 GHz.
By examining the table, several things can be inferred:

- Water generally has a much higher dielectric permittivity than rock forming minerals.
- Water saturated rocks have much larger dielectric permittivities than dry rocks.
- Sediments generally have larger dielectric permittivities than hard rocks.



+-----------------------------+---------------------------------------------+
| **Rock/Soil Type**          |:math:`\varepsilon_r\;` **at Zero-Frequency**|
+=============================+=============================================+
| Air                         | 1                                           |
+-----------------------------+---------------------------------------------+
| Water (fresh)               | 81                                          |
+-----------------------------+---------------------------------------------+
| Water (sea)                 | 81                                          |
+-----------------------------+---------------------------------------------+
| Snow                        | 1.4 - 3                                     |
+-----------------------------+---------------------------------------------+
| Ice                         | 3 - 8                                       |
+-----------------------------+---------------------------------------------+
| Permafrost                  | 1 - 8                                       |
+-----------------------------+---------------------------------------------+
| **Sediments**               |                                             |
+-----------------------------+---------------------------------------------+
| Sand (dry)                  | 3 - 6                                       |
+-----------------------------+---------------------------------------------+
| Sand (wet)                  | 25 - 30                                     |
+-----------------------------+---------------------------------------------+
| Silt (wet)                  | 10                                          |
+-----------------------------+---------------------------------------------+
| Clay Soil (dry)             | 3                                           |
+-----------------------------+---------------------------------------------+
| Clay (wet)                  | 8 - 15                                      |
+-----------------------------+---------------------------------------------+
| Marsh                       | 12                                          |
+-----------------------------+---------------------------------------------+
| Agricultural Land           | 15                                          |
+-----------------------------+---------------------------------------------+
| Pastoral Land               | 13                                          |
+-----------------------------+---------------------------------------------+
| **Rocks**                   |                                             |
+-----------------------------+---------------------------------------------+
| Granite                     | 5 - 8                                       |
+-----------------------------+---------------------------------------------+
| Limestone                   | 7 - 9                                       |
+-----------------------------+---------------------------------------------+
| Dolomite                    | 6.8 - 8                                     |
+-----------------------------+---------------------------------------------+
| Basalt (wet)                | 8                                           |
+-----------------------------+---------------------------------------------+
| Shale (wet)                 | 7                                           |
+-----------------------------+---------------------------------------------+
| Sandstone (wet)             | 6                                           |
+-----------------------------+---------------------------------------------+
| Coal                        | 4 - 5                                       |
+-----------------------------+---------------------------------------------+
| **Minerals**                |                                             |
+-----------------------------+---------------------------------------------+
| Quartz                      | 4.2 - 5                                     |
+-----------------------------+---------------------------------------------+
| Orthoclase Feldspar         | 4.5 - 5.8                                   |
+-----------------------------+---------------------------------------------+
| Kaolinite (clay)            | 9.5 - 13.7                                  |
+-----------------------------+---------------------------------------------+
| Calcite                     | 7.8 - 8.5                                   |
+-----------------------------+---------------------------------------------+
| **Contaminents**            |                                             |
+-----------------------------+---------------------------------------------+
| Benzene                     | 2.3                                         |
+-----------------------------+---------------------------------------------+
| Toulene                     | 2.4                                         |
+-----------------------------+---------------------------------------------+
| Acetone                     | 20.7                                        |
+-----------------------------+---------------------------------------------+
| Tetrachloroethene           | 2.3                                         |
+-----------------------------+---------------------------------------------+
| Trichloroethene             | 3.4                                         |
+-----------------------------+---------------------------------------------+
| Carbon Tetrachloride        | 2.2                                         |
+-----------------------------+---------------------------------------------+
| **Other**                   |                                             |
+-----------------------------+---------------------------------------------+
| Concrete                    | 6-30                                        |
+-----------------------------+---------------------------------------------+
| Asphalt                     | 3-5                                         |
+-----------------------------+---------------------------------------------+
| PVC, Epoxy, Polyesters      | 3                                           |
+-----------------------------+---------------------------------------------+






Factors Impacting Electric Permittivity
=======================================



**Porosity and Water Saturation**:

By far the most important factors in determining a rock's dielectric permittivity are porosity and water saturation.
Air has a relative permittivity of 1 whereas common rock forming minerals have much higher relative permittivities.
This means that for dry samples, the rock's bulk dielectric permittivity decreases as the porosity increases.

When rock samples are saturated with water, their dielectric permittivities can increase drastically.
This is because water has a relative permittivity of 81, which is much higher than the relative permittivities of rock forming minerals.
As a result, the bulk dielectric permittivity of a rock increases as pore water saturation increases.

The relationship between a rock's bulk dielectric permittivity, porosity and water saturation is given by:

.. math::
	\sqrt{\varepsilon} = (1 - \phi ) \sqrt{\varepsilon_m} + \phi S_w \sqrt{\varepsilon_w} + \phi (1-S_w) \sqrt{\varepsilon_a}

where

- :math:`0 \leq \phi \leq 1` is the porosity
- :math:`0 \leq S_w \leq 1` is the factional volume of the pore space saturated by water.
- :math:`\varepsilon_m` is the dielectric permittivity of rock forming minerals.
- :math:`\varepsilon_a` is the dielectric permittivity of air (equal to free-space).
- :math:`\varepsilon_w` is the dielectric permittivity of water.


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
