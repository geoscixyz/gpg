.. _physical_properties_density:

Density
*******

Some Definitions
================

For gravity survey, the physical property of concern is density. A densier buried object would create an higher attraction than the background. A hole, with a density of 0, would create a lower attraction than the background. Difference of densities in the subsurface can be mapped by measuring the variations of the earth gravity field.

Density is defined as the ratio between the mass m of an object and its volume V.

.. math::											
	\rho = \frac{m}{V} \quad &&\textrm{Volumetric mass density,}\ (g/cm^3)\ or \ (kg/m^3)


Densities of geologic materials vary from \\(880 ~\\text{kg/m}^3\\) (ice) (or \\(0\\) for air) to over \\(8000 ~{\\text{kg/m}}^3\\) for some rare minerals. Rocks are generally between \\(1600 ~\\text{kg/m}^3\\) (sediments) and \\(3500 ~\\text{kg/m}^3\\) (gabbro). Table 2.1 from PV Sharma is reproduced below.

.. figure:: ./images/gravity_table.gif

It is important to recall the difference between mass, density and weight. Density is the physical property - it is mass (kilograms) per unit volume. Weight is the force experienced by that mass in the presence of a gravitational field. Your weight on the Moon is 1/6th of your weight on Earth, but your mass (and density) is the same wherever you are.

Specific gravity is also often used and is defined as a relative density in comparaison with a reference substance (usually water, whose density is approximated to \\(1 ~\\text{g/cm^3}\\).

.. math::
	SP=\frac{\rho}{\rho_{{\omega}}}


Density Measurements 
====================

There are several ways to measure the density of differents materials.

Hydrostatic wieghting for compact samples
-----------------------------------------

The idea of this measurement is too measure with a scale the apparent mass of an object in air :math:`M_{air}` and then immersed in a fluid (usually water) :math:`M_{\omega}`. (for more details, see ASTM norm C127)

.. math::	
	\rho_{\text{i}}=\frac{M_{\text{air}}}{M_{\text{air}}-M_{\omega}} \times \rho_{{\omega}}										
	
.. figure:: ./images/hydrostatic_weighting_legend.jpg


Non compact materials
---------------------

Measuring non compact materials density (as sand for example) requires a pycnometer, which is basically a glass with a known volume. By filling the pycnometer with a known mass of material and then filling the gaps with water up to the known volume marked on the pycnometer, we are able to estimate the density of the grains. (for more details, see ASTM norm D857).

However this will not inform you about the porosity and the macroscopic density on field.


Gamma-Gamma density logging
---------------------------

This type of measurement allows to record continuously the bulk density of a formation along a borehole. The probe is composed of one radioactive transmitter of gamma rays and one receiver that measures the proportion of rays scattered by the wall material by Compton effects. This proportion can then be related to the formation's density.





