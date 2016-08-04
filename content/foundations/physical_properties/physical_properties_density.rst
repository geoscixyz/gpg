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
| Specific Gravity | :math:`S.G.` | *Unitless                              |
+------------------+--------------+----------------------------------------+



Density Measurements
====================

Acquiring the density of a material requires an appropriate method of measurement.
Below are four common ways to measure density ordered from more basic to more sophisticated.

**Basic Method**

The most basic method for measuring a rock's bulk density can be performed in two steps.
First, the mass of the rock is obtained using a scale.
Next, the rock is fully immersed into a volume of water contained in a graduated cylinder.
The amount of water which is displaced by the rock is equal to its volume.
Therefore, the volume of the rock is equal to the change in volume (:math:`\Delta V`) measured from the graduated cylinder:

.. math::
	\rho = \frac{m}{\Delta V}

Although it is simple, this method is not particularly accurate and is rarely used for practical purposes.

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
Bulk density is not recovered using this method, as we are not accounting for the rock's pore space.

Pycnometers typically have a chamber of known volume (:math:`V_c`).
Once a rock has been placed in the chamber, the initial volume of the chamber is changed, thus changing the pressure.
The change in gas pressure is used to determine how much of the chamber is comprised of gas.
This can be used to determine the volume of solid material within the chamber (denoted by :math:`V_s`).
The difference between :math:`V_c` and :math:`V_s` represents the volume of solid material comprising the rock.
The skeletal density of the rock is therefore:

.. math::
	\rho_{sk} = \frac{m}{V_c - V_s}
	

**Gamma-Gamma Density Logging**

Gamma-gamma density logging is used to continuously record the bulk density of rock formation along a borehole.
For these measurements, gamma rays are emmitted by a radioactive source.
While transmitting through the adjacent rock, the gamma rays interact with electrons and undergo Compton scattering.
A detector within the borehole measures the intensity of the scattered gamma rays.
Gamma rays experience a higher level of Compton scattering in denser materials.
Therefore, the intensity scattered signal can be used to obtain the bulk density of the rocks within the borehole. 


Density of Common Rocks
=======================

Below, we have summarized the density ranges for common rock types (Telford et al., 1990).
Although certain rock types are generally less dense than others, it is important to recognize that density values for certain rock types may overlap.


+-----------------------+-----------------------------------+
| Rock Type             | Density Range (g/cm :math:`\!^3`) |
+=======================+===================================+
| **Sedimentary Rocks** |                                   |
+-----------------------+-----------------------------------+
| Clay                  |           1.63 - 2.60             |
+-----------------------+-----------------------------------+
| Silt                  |           1.80 - 2.20             |
+-----------------------+-----------------------------------+
| Soil                  |           1.20 - 2.40             |
+-----------------------+-----------------------------------+
| Sand                  |           1.70 - 2.30             |
+-----------------------+-----------------------------------+
| Sandstone             |           1.61 - 2.76             |
+-----------------------+-----------------------------------+
| Shale                 |           1.77 - 3.30             |
+-----------------------+-----------------------------------+
| Limestone             |           1.93 - 2.90             |
+-----------------------+-----------------------------------+
| Dolomite              |           2.28 - 2.90             |
+-----------------------+-----------------------------------+
| Chalk                 |           1.52 - 2.60             |
+-----------------------+-----------------------------------+
| Halite                |           2.10 - 2.60             |
+-----------------------+-----------------------------------+
| Gypsum                |           2.20 - 2.60             |
+-----------------------+-----------------------------------+
| **Igneous Rocks**     |                                   |
+-----------------------+-----------------------------------+
| Rhyolite              |           2.35 - 2.70             |
+-----------------------+-----------------------------------+
| Granite               |           2.50 - 2.81             |
+-----------------------+-----------------------------------+
| Andesite              |           2.40 - 2.80             |
+-----------------------+-----------------------------------+
| Basalt                |           2.70 - 3.30             |
+-----------------------+-----------------------------------+
| Gabbro                |           2.70 - 3.50             |
+-----------------------+-----------------------------------+
| **Metamorphic Rocks** |                                   |
+-----------------------+-----------------------------------+
| Slate                 |           2.70 - 2.90             |
+-----------------------+-----------------------------------+
| Phyllite              |           2.68 - 2.80             |
+-----------------------+-----------------------------------+
| Schist                |           2.39 - 2.80             |
+-----------------------+-----------------------------------+
| Gneiss                |           2.59 - 3.00             |
+-----------------------+-----------------------------------+
| Granulite             |           2.52 - 2.73             |
+-----------------------+-----------------------------------+
| Amphibolite           |           2.90 - 3.04             |
+-----------------------+-----------------------------------+
| Eclogite              |           3.20 - 3.54             |
+-----------------------+-----------------------------------+
| **Ore-Bearing Rocks** |                                   |
+-----------------------+-----------------------------------+
| Bauxite               |           2.30 - 2.55             |
+-----------------------+-----------------------------------+
| Pyrite and Pyrrhotite |           4.50 - 5.20             |
+-----------------------+-----------------------------------+
| Magnetite             |           4.90 - 5.20             |
+-----------------------+-----------------------------------+
| Hematite              |           4.90 - 5.30             |
+-----------------------+-----------------------------------+
| Cobaltite             |           5.80 - 6.30             |
+-----------------------+-----------------------------------+
| Galena (Lead-Sulphide)|           7.40 - 7.60             |
+-----------------------+-----------------------------------+
| **Other**             |                                   |
+-----------------------+-----------------------------------+
| Water                 |              1.00                 |
+-----------------------+-----------------------------------+
| Petroleum             |           0.60 - 0.90             |
+-----------------------+-----------------------------------+



Factors Impacting Rock Density
==============================

There are many factors which impact the bulk density of a rock.
Below are several important factors which you should be familiar with.

**Composition**

Composition impacts the density of all rock types.
Most common rocks are made up of sillicate minerals due to the abundance of silicon and oxygen in the Earth's crust.
The distinct densities of these rocks, however, are dictated by the abundances of other elements such as: aluminum, iron, calcium, sodium, potassium and magnesium.

In igeneous rocks, density generally decreases with respect to the \% abundance of silica (Si0 :math:`\!_2`) contained within the rock.
Using this relationship, igeneous rocks are classified as being felsic, intermediate, mafic or ultramafic.
Rocks with lower silica content (mafic) tend to contain higher abundances of heavier elements like magnesium and iron; making them denser than rocks with a higher silica content (felsic).
This explains why the oceanic crust (mafic) is typically more dense than the continental crust (felsic).
The classification of igeneous rocks based on \% silica content can be seen below:


+-------------------+------------------------------+----------+
| Igneous Rock Type | \% Silica (SiO :math:`\!_2`) | Density  |
+===================+==============================+==========+
| Felsic            | 65\% <                       | Lowest   |
+-------------------+------------------------------+----------+
| Indermediate      | 55\% - 65\%                  | Moderate |
+-------------------+------------------------------+----------+
| Mafic             | 45\% - 55\%                  | High     |
+-------------------+------------------------------+----------+
| Ultramafic        | < 45\%                       | Highest  |
+-------------------+------------------------------+----------+

Similar relationships between composition and density are much harder to obtain for sedimentary and metamorphic rocks.
For sedimentary rocks, the density depends on the rock's parent material, which can be highly variable.
For metamorphic rocks, the density depends on the parent rock and the metamorphic alteration it has experienced.

The oxide and sulphide minerals contained in ore-bearing rocks are much denser than typical rock forming minerals.
This is because ore-bearing rocks contain large quantities of heavy elements such as gold, silver, copper, lead and iron.



**Porosity**

Porosity primarily impacts the density of sedimentary and extrusive volcanic rocks, as the porosity of other rock types is generally very small.
Pore fluids, whether it be air, water, brine or petroleum, have much less density than rock forming minerals.
As a result, rock density decreases as porosity increases.
Because air, water, brine and petroleum have measureably different densities, the type of pore fluid also impacts the density of the rock.


**Pressure**

Sedimentary rocks can experience significant pressure from overlying geological units.
In sedimentary rocks, compressional forces are responsible for reducing the pore space.
The reduction in pore space ultimately results in a higher density for the rock.
This is explains why sediments at the bottom of a basin are typically denser than those at the top.





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





