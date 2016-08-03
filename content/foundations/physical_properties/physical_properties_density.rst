.. _physical_properties_density:

Density
*******

Density (:math:`\rho`) is the diagnostic physical property used in gravity surveys.
Density is defined as the mass (:math:`m`) contained within a material per unit volume (:math:`V`):

.. math::
	\rho = \frac{m}{V}
	
Please note that mass (the quantity of matter within an object) should not be confused with weight (the downward force exerted by an object due to gravity).

**Specific Gravity**: In some cases, the density of a material is represented instead by its specific gravity.
Specific gravity defines the ratio of a material's density to that of water:

.. math::
	S.G. = \frac{\rho}{\rho_w}

where the density of water (:math:`\rho_w`) is 1,000 kg/m :math:`\!^3` (or 1 g/cm :math:`\!^3`).
Parameters used to define density and their associated units are summarized below:

+------------------+--------------+----------------------------------------+
| Property         | Symbol       | Units                                  |
+==================+==============+========================================+
| Density          | :math:`\rho` | g/cm :math:`\!^3` or kg/m :math:`\!^3` |
+------------------+--------------+----------------------------------------+
| Mass             | :math:`m`    | g or kg                                |
+------------------+--------------+----------------------------------------+
| Volume           | :math:`V`    | cm :math:`\!^3` or m :math:`\!^3`      |
+------------------+--------------+----------------------------------------+
| Specific Gravity | :math:`S.G.` | *None                                  |
+------------------+--------------+----------------------------------------+



Density Measurements
====================

Acquiring the density of a material requires an appropriate method of measurement.
Below are four common ways to measure density ordered from most basic to most sophisticated.

**Basic Method**

The most basic method for measuring a rock's bulk density can be performed in two steps.
First, the mass of the rock is obtained using a scale.
Next, the rock is fully immersed into a volume of water contained in a graduated cylinder.
The amount of water which is displaced by the rock is equal to its volume.
Now that we know the mass and the volume of the rock, we can determine the density using the first equation.
This method however, is not particularly accurate and is rarely used for practical purposes.

**Hydrostatic Weighting**

For this method, the mass of the rock (:math:`m_{a}`) is first measured using a conventional scale.
The rock is then immersed into a bath of water, where its underwater weight is measured and used to obtain an apparent mass (:math:`m_{w}`).
Where :math:`\rho_w` = 1000 kg/m :math:`\!^3` is the density of water, the density of the rock is given by:

.. figure:: ./images/hydrostatic_weighting_legend.jpg
	:scale: 50%
	:align: right

.. math::	
	\rho = \frac{m_a}{m_a - m_w} \times \rho_w									

Although this method is simple, it cannot be used effectively for rocks which are overly unconsolidated or porous.
Unconsolidated rocks have a tendency to break apart when immersed in water.
The pore-space within porous rocks becomes partially filled, resulting in an overestimation of the rock's density.

**Pycnometer Measurements**

Pycnometer measurements are generally used on porous rocks and sediments.
Using a pycnometer, we can obtain a rock's skeletal density; that is, the average density of all solid material within the rock.
As a result, bulk density is not recovered using this method, as we are neglecting the rock's pore space.

Pycnometers typically have a chamber of known volume (:math:`V_c`).
Once a rock has been placed in the chamber, the volume of the chamber is changed.
The subsequent change in gas pressure is used to determine the volume of gas both surrounding and within the pore space of the rock (denoted by :math:`V_s`).
The difference between :math:`V_c` and :math:`V_a` represents the skeletal volume of the rock.
The skeletal density of the rock is therefore:

.. math::
	\rho_{sk} = \frac{m}{V_c - V_s}
	

**Gamma-Gamma Density Logging**

Gamma-gamma density logging is used to continuously record the bulk density of rocks along a borehole.
For these measurements, gamma rays are emmitted by a radioactive source.
As the rays attempt to penetrate through the borehole, they interact with electrons within the rock and undergo Compton scattering.
On the other side of the borehole, a detector measures the intensity of scattered gamma rays.
Gamma rays experience a higher level of Compton scattering in denser materials.
Therefore, the intensity of the detected gamma ray signal can be used to obtain the bulk density of the rocks within the borehole. 


Density of Common Rocks
=======================

The densities of a rocks vary depending on their composition and structure.
However, rocks formed by similar processes


The composition and structure of each rock is unique.
Thus, the densities characterizing rocks are highly variable.





Factors Impacting Rock Density
==============================

There are many factors which impact the bulk density of a rock.
Below are several important factors which you should be familiar with.

**Mineralogy**

The bulk density of most rocks is determined by its mineralogy.



**Pore-Space and Pore Fluid**

Nearly all rocks contain pore space.
For compacted or cemented rocks, the pore space is very small.
However, the pore space contained within extrusive volcanic and sedimentary rocks can vary significantly large.
The pore space within a rock is generally filled with fluids such as air, water or brine.



**Compaction**





**Cementation**






xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

Some Definitions
================

For gravity survey, the physical property of concern is density. A densier
buried object would create an higher attraction than the background. A hole,
with a density of 0, would create a lower attraction than the background.
Difference of densities in the subsurface can be mapped by measuring the
variations of the earth gravity field.

Density is defined as the ratio between the mass m of an object and its volume
V.

.. math::											
	\rho = \frac{m}{V} \quad &&\textrm{Volumetric mass density,}\ (g/cm^3)\ or \ (kg/m^3)


Densities of geologic materials vary from :math:`880 ~\text{kg/m}^3` (ice) (or
:math:`0` for air) to over :math:`8000 ~{\text{kg/m}}^3` for some rare minerals.
Rocks are generally between :math:`1600 ~\text{kg/m}^3` (sediments) and :math:`3500
~\text{kg/m}^3` (gabbro). Table 2.1 from PV Sharma is reproduced below.

.. figure:: ./images/gravity_table.gif

It is important to recall the difference between mass, density and weight.
Density is the physical property - it is mass (kilograms) per unit volume.
Weight is the force experienced by that mass in the presence of a
gravitational field. Your weight on the Moon is 1/6th of your weight on Earth,
but your mass (and density) is the same wherever you are.

Specific gravity is also often used and is defined as a relative density in
comparaison with a reference substance (usually water, whose density is
approximated to :math:`1 ~\text{g/cm}^3`.

.. math::
	SP=\frac{\rho}{\rho_{{\omega}}}


Density Measurements 
====================

There are several ways to measure the density of differents materials.

Hydrostatic wieghting for compact samples
-----------------------------------------

The idea of this measurement is too measure with a scale the apparent mass of
an object in air :math:`M_{air}` and then immersed in a fluid (usually water)
:math:`M_{\omega}`. (for more details, see ASTM norm C127)

.. math::	
	\rho_{\text{i}}=\frac{M_{\text{air}}}{M_{\text{air}}-M_{\omega}} \times \rho_{{\omega}}										
	
.. figure:: ./images/hydrostatic_weighting_legend.jpg


Non compact materials
---------------------

Measuring non compact materials density (as sand for example) requires a
pycnometer, which is basically a glass with a known volume. By filling the
pycnometer with a known mass of material and then filling the gaps with water
up to the known volume marked on the pycnometer, we are able to estimate the
density of the grains. (for more details, see ASTM norm D857).

However this will not inform you about the porosity and the macroscopic
density on field.


Gamma-Gamma density logging
---------------------------

This type of measurement allows to record continuously the bulk density of a
formation along a borehole. The probe is composed of one radioactive
transmitter of gamma rays and one receiver that measures the proportion of
rays scattered by the wall material by Compton effects. This proportion can
then be related to the formation's density.





