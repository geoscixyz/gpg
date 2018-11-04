.. _physical_properties_density:

Density
*******

Density (:math:`\rho`) is defined as the mass (:math:`m`) contained within a material per unit volume (:math:`V`):

.. math::
    \rho = \frac{m}{V}

Please note that mass (the quantity of matter within an object) should not be confused with weight (the downward force exerted by an object due to gravity).

**Specific Gravity**:

In some cases, the density of a material is represented instead by its specific gravity.
Specific gravity defines the ratio of a material's density to that of water:

.. math::
    S.G. = \frac{\rho}{\rho_w}

where the density of water :math:`\rho_w` = 1,000 kg/m :math:`\!^3` (or 1 g/cm :math:`\!^3`).
Parameters used to define density and their associated units are summarized below.


+------------------+--------------+----------------------------------------+
| Property         | Symbol       | Units                                  |
+==================+==============+========================================+
| Density          | :math:`\rho` | g/cm :math:`\!^3` or kg/m :math:`\!^3` |
+------------------+--------------+----------------------------------------+
| Mass             | :math:`m`    | g or kg                                |
+------------------+--------------+----------------------------------------+
| Volume           | :math:`V`    | cm :math:`\!^3` or m :math:`\!^3`      |
+------------------+--------------+----------------------------------------+
| Specific Gravity | :math:`S.G.` | *Unitless*                             |
+------------------+--------------+----------------------------------------+



Density Measurements
====================

Acquiring the density of a material requires an appropriate method of measurement.
Below are four common ways to measure density. These are ordered from more basic to more sophisticated.

**Basic Method**

The most basic method for measuring a rock's bulk density can be performed in two steps.
First, the mass (M) of the rock is obtained using a weight scale.
Next, the rock is fully immersed into a volume of water contained in a graduated cylinder.
The amount of water which is displaced by the rock is equal to the volume (:math:`V`) of the sample.
The density of the rock is obtained from

.. math::
    \rho = \frac{m}{V}

This method is simple but it is often not sufficiently accurate for geophysical purposes.

**Hydrostatic Weighting**

For this method, the mass of the rock (:math:`m_{a}`) is first measured using a conventional scale.
The rock is then immersed into a bath of water, where its underwater weight is measured and used to obtain an apparent mass (:math:`m_{w}`).
Where :math:`\rho_w` = 1000 kg/m :math:`\!^3` is the density of water, the density of the rock is given by:

.. figure:: ./images/hydrostatic_weighting_legend.jpg
    :scale: 50%
    :align: right

.. math::
    \rho = \frac{m_a}{m_a - m_w} \times \rho_w

This method does poorly if the rock is unconsolidated or porous.
Unconsolidated rocks tend to break apart when immersed in water.
The pore-space within porous rocks becomes partially filled, resulting in an overestimation of the rock's density.

**Pycnometer Measurements**

Pycnometer measurements are generally used on porous rocks and sediments.
Using a pycnometer, we can obtain a rock's skeletal density; that is, the average density of all solid material within the rock.
Bulk density is not recovered using this method, as we are not accounting for the rock's pore space.

Pycnometers typically consist of a hollow chamber with a known initial volume (:math:`V_c`).
Once a rock has been placed in the chamber, the volume of the chamber is changed, resulting in a change in gas pressure around the rock.
The change in gas pressure is used to determine how much of the chamber is filled with gas (:math:`V_s`).
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
Therefore, the intensity of scattered signal can be used to obtain the bulk density of the rocks within the borehole.


Density of Common Rocks
=======================

Each rock type is defined by a range of density values (not a specific value). The densities for some common rocks, minerals, and other materials are summarized below.
Note that the density ranges for different rock types can overlap.
Some general comments pertaining to densities are:

- Igneous and metamorphic rock are generally more dense than sedimentary rocks.
- Mafic igneous rocks are generally more dense than felsic igneous rocks.
- Higher metamorphic grade rocks such as eclogite and amphibolite are more dense than low grade metamorphic rocks such as slate and phyllite.
- Metal ore-bearing rocks are generally much denser than other rock types. One exception is bauxite.

To see the range of densities for specific rock types, click the links in the table.

+------------------------------------------------------+-----------------------------------+
| Material                                             | Density Range (g/cm :math:`\!^3`) |
+======================================================+===================================+
| Air                                                  |           0.001225                |
+------------------------------------------------------+-----------------------------------+
| Water                                                |           1.00                    |
+------------------------------------------------------+-----------------------------------+
| Ice                                                  |           0.917                   |
+------------------------------------------------------+-----------------------------------+
| Petroleum                                            |           0.60 - 0.90             |
+------------------------------------------------------+-----------------------------------+
| :ref:`Sedimentary  Rocks<table_density_sedimentary>` |           1.50 -3.30              |
+------------------------------------------------------+-----------------------------------+
| :ref:`Igneous Rocks<table_density_igneous>`          |           2.35 -3.50              |
+------------------------------------------------------+-----------------------------------+
| :ref:`Metamorphic Rocks<table_density_metamorphic>`  |           2.52- 3.54              |
+------------------------------------------------------+-----------------------------------+
| :ref:`Ore-Bearing Rocks<table_density_ore_bearing>`  |           2.30- 7.60              |
+------------------------------------------------------+-----------------------------------+




Factors Impacting Rock Density
==============================

There are many factors which impact the bulk density of a rock.
Below are several important factors which you should be familiar with.

**Composition**

Composition impacts the density of all rock types.
Most common rocks are made up of sillicate minerals due to the abundance of silicon and oxygen in the Earth's crust.
The distinct densities of these rocks, however, are dictated by the abundances of other elements such as: aluminum, iron, calcium, sodium, potassium and magnesium.

In igneous rocks, density generally decreases with respect to the \% abundance of silica (Si0 :math:`\!_2`) contained within the rock.
Using this relationship, igeneous rocks are classified as being felsic, intermediate, mafic or ultramafic.
Rocks with lower silica content (mafic) tend to contain higher abundances of heavier elements like magnesium and iron; making mafic rocks denser than rocks with a higher silica content (felsic).
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





