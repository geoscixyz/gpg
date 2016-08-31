.. _induced_polarization_physical_properties_duplicate:

Chargeability
*************






.. math::
	V_{off} = m e^{-t/\lambda}



**Membrane Polarization**



**Electrode Polarization**




Chargeability Measurements
==========================

Chargeability measurements are very similar to conductivity/resistivity measurements.
First, a cylindrical core sample is taken from the rock.
The core sample is then placed in a sample holder between two copper/graphite electrodes where it acts as an impedence element for a circuit.


.. figure:: ./images/electrode_chargeability_measurements.png
	:align: right
	:scale: 40%


Next, a source is used to drive alternating current (:math:`I`) through the core sample.
By measuring the voltage drop (:math:`\Delta V`) accross the length of the sample, Ohm's law can be used to determine the circuit impedence (:math:`Z`) caused by the rock:

.. math::
	Z(\omega ) = \frac{\Delta V (\omega)}{I (\omega)}


In chargeable rocks, the measured voltage drop depends on the frequency of the alternating current.
So in order to characterize the resistive properties of the rock, we need to determine the impedence over a spectrum of frequencies.

The resistivity of the sample at each frequency can be obtained from the impedence, the length of the core (:math:`L`) and its cross-sectional area (:math:`A`) using Pouillet's law:

.. math::
	\rho (\omega) = \frac{Z(\omega) A}{L}


In order to determine the rock's chargeability, we fit the experimentally acquired resistivity values to a mathematical model.
This is illustrated below.
A well-established model for explaining the resistivities of chargeable rocks is the Cole-Cole model:

.. math::
	\rho (\omega) = \rho_0 \Bigg [ 1 - m \Bigg ( 1 - \frac{1}{1 + (i\omega\tau )^C} \Bigg ) \Bigg ]


where :math:`m` is the chargeability and :math:`\rho_0` is the DC resistivity.
Parameters :math:`\tau` and :math:`C` control the rate at which ionic charges accumulate when subjected to an electric field.
By setting :math:`C=1`, :math:`\tau` defines the exponential decay in voltage according to the first equation.
The conductivity of the rock can be obtained by taking the reciprocal of the complex resistivity:

.. math::
	\sigma (\omega) = \frac{1}{\rho (\omega)}


.. figure:: ./images/electrode_chargeability_curve_fit.png
	:align: center
	:scale: 40%












Chargeability is one of two diagnostic physical properties in DC/IP surveys.
Chargeability defines the magnitude of ionic charge build-up within a rock under the influence of an electric field.
For chargeable rocks, Ohm's law can still be used to relate the density of electrical current (:math:`\vec J`) to an applied electric field (:math:`\vec E`):


.. math::
	\vec E = \rho \vec J

In this case however, :math:`\sigma` is represented by a frequency-dependent conductivity:


where :math:`\rho_0` is the DC/zero-frequency resistivity and :math:`0 \leq m \leq 1` is the chargeability.
Parameters :math:`\tau` and :math:`C` define the frequency-dependent aspect of the complex conductivity.




Under a static field, a portion of the ionic charges within the rock's pore fluid will accumulate on grain boundaries.
In this case:

.. math::
	\lim_{\omega \rightarrow 0} \sigma = \sigma_0.


At high frequencies, none of the ionic charges to not have sufficient time to accumulate.
As a result, these ions contribute towards the conductive mechanism occurring within the rock.
Thus at high frequencies:

.. math::
	\lim_{\omega \rightarrow \infty} \sigma = \frac{\sigma_0}{1 - m}


and the conductivity of the rock is larger.


**Complex Resisitivity**

In many cases, the electrical properties of chargeable rocks are described using a complex resistivity:

.. math::
	\rho = \frac{1}{\sigma} = \rho_0 \Bigg [ 1 - m \Bigg ( 1 - \frac{1}{1 + (i\omega\tau )^C} \Bigg ) \Bigg ]



Chargeability Measurements
==========================







Chargeabilities of Common Rocks
===============================






Factors Impacting Chargeability
===============================





xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

Introduction
============

Chargeability is a physical property that is related to resistivity. The
module about DC resistivity shows that potentials measured in a DC resistivity
survey can be related to charges that accumulate when current is made to flow.
However, when the transmitter current is switched off, the measured voltage
may take up to several seconds to reach zero. Similarly, when the current is
switched on, there may be a finite time taken for the voltage to reach a
steady state value. In other words, current injected into the ground causes
some materials to become polarized. The phenomenon is called induced
polarization, and the physical property that is measured is usually called
chargeability, which quantifies the material's capacity to retain charges
after a forcing current is removed. The following figure illustrates the
measurable effect.

 .. figure:: ./images/images_duplicates/IP_source.gif
	:align: center
	:scale: 100 %


Induced polarization can also be measured using low frequency sinusoidal
signals, as discussed in the `induced polarization measurements data`_ section
of this chapter. The signals or data that are measured depend upon which of
the various types of source signals are used. Note that IP surveys always
include resistivity measurements because the electrical resistivity of teh
earth must be known in order to invert data to recover chargeability.



What can be detected?
=====================

The materials that are most chargeable include sulfide minerals (both massive
and disseminated), clay-rich materials, and graphite. However, the
chargeablility of materials can have a wide range within the same geographic
region. This is because chargeability depends upon many factors, including
mineral type, grain size, the ratio of internal surface area to volume, the
properties of electrolytes in pore space, and the physics of interaction
between surfaces and fluids.

Interpretation of chargeabililty models is further complicated by the fact
that there is no standard set of units for this physical property. There are
at least three ways of measuring the phenomenon and models recovered by
inversion generally take on the same units as the measurement. This could be
milli-seconds if measurements are made of the ground's response to impulsive
sources. The units could also be percent if the response at two or more source
signal frequencies is compared, or units of milliradians may be used if the
phase difference between source and received signals is recorded.

Physical Phenomenons
====================

.. _induced polarization measurements data: http://gpg.geosci.xyz/en/latest/content/induced_polarization/induced_polarization_measurements_data.html

The chargeability of earth materials is essentially an electrochemical effect
caused by many factors, not all of which are completely understood. If ground
is chargeable, it responds as if resistivity was a complex quantity - it
behaves somewhat like a leaky capacitor. Therefore the chargeability can be
measured in a number of ways using time domain or frequency domain techniques
(detailed in the section `induced polarization measurements data`_). Aspects
affecting the chargeability of a sample include:

 - the grain size of particles in the sample;
 - the type and mobility of ions within the pore fluids;
 - the details of microscopic interactions between solid surfaces and fluids;
 - the amount of surface area within a specific volume.

The surface area-to-volume ratio is an important factor. Clays tend to be
chargeable while sandstones are not, and the images here illustrate one reason
why this is true. In addition, the surface interactions between clay minerals
and fluids enhance the ability of these materials to hold charges.

 .. figure:: ./images/images_duplicates/illite.gif
	:align: center
	:scale: 120 %
 
	Illite (a clay mineral) with surface area-to-volume ratio of :math:`100m^2/g` (1000 times greater than sandstone)

 .. figure:: ./images/images_duplicates/quartz.gif
	:align: center
	:scale: 120 %
 
 	Quartz overgrowths in sandstone with surface area-to-volume ratio of :math:`0.1m^2/g`

Two microscopic effects cause macroscopic chargeability
-------------------------------------------------------

There are two primary causes of chargeability. In both cases the re-
distribution of charges takes some time to occur when an external DC electric
field is applied. Equivalently, it takes the same time to revert to a balanced
charge distribution once the electric field is removed. "Charging" is hard to
measure in practice. "Discharging" is measured using time domain IP survey
techniques. The effect of finite charging time on sinusoidal signals at
different frequencies also can be measured using frequency domain or phase IP
surveys. The two types of polarization are called "membrane polarization" and
"electrode polarization."

Membrane polarization
^^^^^^^^^^^^^^^^^^^^^

Membrane polarization occurs when pore space narrows to within several
boundary layer thicknesses (which is the thickness of ions adsorbed to a
surface).

 .. figure:: ./images/images_duplicates/memb1.gif
	:align: center
	:scale: 100 %

Charges cannot flow easily, so they accumulate when an electric field is applied.

 .. figure:: ./images/images_duplicates/memb2.gif
	:figclass: center
	:align: center
	:scale: 100 %


The result is a net charge dipole which adds to any other voltages measured at the surface.	

 .. figure:: ./images/images_duplicates/memb3.gif
	:align: center
	:scale: 100 %

A second form of membrane polarization is similar to the first:

 .. figure:: ./images/images_duplicates/memb_pol_2nd_type.gif
	:align: right
	:scale: 100	

This occurs where clay particles partially block ionic solution paths, as in
the adjacent figure. Upon application of an electric potential, positive
charge carriers pass easily, while negative carriers accumulate. There is an
"ion-selective membrane."

A surplus of both cations and anions occurs at one end of the membrane, while
a deficiency occurs at the other end. The reduction of mobility is most
obvious at frequencies slower than the diffusion time of ions between adjacent
membrane zones; i.e. slower than around 0.1 Hz. Conductivity increases at
higher frequencies.

Electrode polarization
^^^^^^^^^^^^^^^^^^^^^^

Electrode polarization occurs when pore space is blocked by metallic
particles. Again, charges accumulate when an electric field is applied.

 .. figure:: ./images/images_duplicates/elec_pol_1.gif
	:align: center
	:scale: 100

The result is two electrical double layers which add to voltages measured at the surface.

 .. figure:: ./images/images_duplicates/elec_pol_2.gif
	:align: center
	:scale: 100

Comments on electrode polarization
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

 .. figure:: ./images/images_duplicates/elec_pol_3.gif
	:align: right
	:scale: 100

Some remarks are appropriate here in order to provide some sense of the
complexity of the chargeability phenomenon.

At an interface between ionic and metallic conduction (for example, an ore
grain in pore water), there is an impedance involved in getting current to
flow across the barrier. These interfaces look like the top figure and have
the simplified circuit analogue shown in the bottom figure.

 .. figure:: ./images/images_duplicates/elec_pol_4.gif
	:align: right
	:scale: 100 %

Current can flow via charge transfer (or ion diffusion), which involves
electrochemical processes, or via a capacitive effect (no charge transfer),
involving diffusion currents.

Ion diffusion is not easy to model with circuit elements. The process is
called the Warburg impedance. Its magnitude varies as approximately
1/frequency.

Note that, while it is useful to understand simplified models of the relevant
electrical behaviour of surface-electrolyte interactions, all rocks are, in
fact, "dirty" in the sense that they are not simply pure "electrodes"
(semiconducting mineral grains) and electrolytes (pore solutions).  There are
other materials and particles affecting ionic behaviour within and outside the
diffuse layer, and some of the sample's constituents will affect the behaviour
of the fixed layer near and on the liquid-solid interfaces.

Summary of what affects the chargeability of material
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

	- Induced polarization is greater when there are larger regions of adsorbed anomalous charge (adjacent to an interface); i.e. when there is a large surface area-to-volume ratio.
	- Non-ionic fluids (such as contaminants) can markedly change the behaviour of surface-electrolyte interactions.
	- Changes in ion concentration (such as increased salinity) will also affect both types of polarization.
	- Both effects (membrane and electrode polarization) are related to grain size as much as material type. Therefore, discrimination of mineral type on the basis of chargeability alone is not recommended.

Spectral Induced Polarization
=============================

 .. figure:: ./images/images_duplicates/spectral_ip.gif
	:align: right
	:scale: 100 %

The Cole-Cole model for complex impedance is often used for modeling the
ground's impedance. The Cole-Cole model is written as:

 .. math::
		\rho (\omega) = \rho_0 \left[1-m \left( 1- \frac{1}{1+(j \omega \tau)^c}\right) \right] 

This relation describes a complex impedance as a function of frequency,
:math:`\omega` with three parameters. :math:`m` is intrinsic chargeability,
:math:`\tau` is a time constant (of the decay curve), and :math:`c` is a
parameter controlling the frequency dependence.

Typical chargeabilities for materials
=====================================

The following tables (from Telford et al, 1976) provides a very general guide
to possible chargeabilities of materials. One reason that in-situ
chargeabilities tend to appear lower than laboratory values is that large
volumes of mixed materials are involved in field measurements.

These examples show that a wide range of variability can be expected, implying
that it is difficult to use values of intrinsic chargeability (in models
obtained by inversion of IP data) to determine exactly what type of rock or
material is in the ground. However, this is an ongoing topic of research.

**Table 1:** Charging and integration times were about 1 minute each, which is
much longer than field survey systems; therefore, values are larger than
field measurements.

+-----------------------+--------------------------+
|  **Material type**    | **Chargeability (msec)** |
+=======================+==========================+
| 20% sulfides          | 2000-3000                |
+-----------------------+--------------------------+
| 8-20% sulfides        | 1000-2000                |  
+-----------------------+--------------------------+
| 2-8% sulfides         | 500-1000                 |  
+-----------------------+--------------------------+
| volcanic tuffs        | 300-800                  |  
+-----------------------+--------------------------+
| sandstone, siltstone  | 100-500                  |  
+-----------------------+--------------------------+
| dense volcanic rocks 	| 100-500                  |  
+-----------------------+--------------------------+
| shale                 | 50-100                   |  
+-----------------------+--------------------------+
| granite, granodiorite | 10-50                    |  
+-----------------------+--------------------------+
| limestone, dolomite   | 10-20                    |  
+-----------------------+--------------------------+

**Table 2:** The values below involved more realistic charging and integration
times of 3 seconds and 0.02-1.0 seconds respectively.

+-----------------------+--------------------------+
|  **Material type**    | **Chargeability (msec)** |
+=======================+==========================+
| ground water          | 0                        |
+-----------------------+--------------------------+
| alluvium              | 1-4                      |  
+-----------------------+--------------------------+
| gravels               | 3-9                      |  
+-----------------------+--------------------------+
| precambrian volcanics | 8-20                     |  
+-----------------------+--------------------------+
| precambrian gneisses  | 6-30                     |  
+-----------------------+--------------------------+
| schists           	| 5-20                     |  
+-----------------------+--------------------------+
| sandstones            | 3-12                     |  
+-----------------------+--------------------------+
| argilites             | 3-10                     |  
+-----------------------+--------------------------+
| quartzites            | 5-12                     |  
+-----------------------+--------------------------+

**Table 3:** Chargeability of minerals at 1% concentration in the samples (charging and integration times as per Table 2 above)

+-----------------------+--------------------------+
|  **Material type**    | **Chargeability (msec)** |
+=======================+==========================+
| pyrite                | 13.4                     |
+-----------------------+--------------------------+
| chalcocite            | 13.2                     |  
+-----------------------+--------------------------+
| copper                | 12.3                     |  
+-----------------------+--------------------------+
| graphite              | 11.2                     |  
+-----------------------+--------------------------+
| chalcopyrite          | 9.4                      |  
+-----------------------+--------------------------+
| bornite            	| 6.3                      |  
+-----------------------+--------------------------+
| galena                | 3.7                      |  
+-----------------------+--------------------------+
| magnetite             | 2.2                      |  
+-----------------------+--------------------------+
| malachite             | 0.2                      |  
+-----------------------+--------------------------+
| hematite              | 0.0                      |  
+-----------------------+--------------------------+

Typical problems where chargeability is useful
==============================================


Mineral exploration for sulfides (disseminated and massive) is unquestionably
the most common application of IP because those types of ore minerals are
often chargeable.There are also applications in hydrogeology. For example,
mapping salt water intrusions in aquifers that include clayey layers may be
difficult using resistivity alone. However, the increased chargeability
associated with clay may help differentiate between zones with more saline
water and clay, both of which have low resistivity. In addition, there is a
growing interest in the possibility of using chargeability to aid in the
detection and delineation of contaminants in the ground. There has also been
some effort to apply IP to oil and gas exploration.

