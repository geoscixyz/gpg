.. _magnetics_susceptibility:

Susceptibility
**************

For magnetic surveys, the relevant physical property is *magnetic susceptibiity*, or less commonly the related property *magnetic permeability*. 


Some Definitions
================

.. math::
	&\vec{B} \quad &&\textrm{magnetic flux density, } W/m^2=T \text{ (Teslas)} \\[0.3em]
	&\vec{H} \quad &&\textrm{magnetic field intensity, } A/m  \\[0.3em]
	&\mu \quad &&\textrm{magnetic permeability, } H/m  \\[0.3em]
	&\mu_0 = 4 \pi 10^{-7} \quad &&\textrm{the permeability of free space, } H/m  \\[0.3em]
	&\vec{B} = \mu \vec{H} \quad &&\textrm{the constitutive relation between } \vec{B} \text{ and } \vec{H} \\[0.3em]
	&\mu = \mu_0(1+\kappa) \quad &&\textrm{where } \kappa \textrm{ is magnetic susceptibility} \\[0.3em]
	&\vec{M}=\kappa \vec{H} \quad &&\textrm{where } \vec{M} \textrm{ is magnetization} \\[0.3em]
	&\vec{m} \quad &&\textrm{dipole moment, } Am^2 \\[0.3em]
	& \text{1 Tesla} = 10^9 \text{nT} \\[0.3em]
	& \text{1 nT} =   \gamma

**What is susceptibility?** When there is no external magnetic field, individual magnetic zones ("magnetic domains") within rocks, soils or other materials will generally be oriented randomly. The net effect would be a zero magnetic field. However, when the material is in the presence of an external magnetic field such as Earth’s field, tBKhe individual magnetic domains become more or less aligned, resulting in a net non-zero field. This is a secondary field distinct from, but caused by, the Earth’s field. The following interactive figure illustrates:

.. raw:: html
    :file: susceptibility.html
	
	
The strength of the induced magnetisation, \\(M\\), the "dipole moment per unit volume", has units Am\ :sup:`2`\ . It is related to the causative field's strength, \\(H\\), by 

.. math::
		\vec{M}=\kappa \vec{H}

Susceptibility \\( \\kappa \\) is a dimensionless number related to the number of individual magnetic dipoles in the medium that can be aligned with the main field. Note that as the field increases the number of dipoles that align themselves with the field also increases.




Although unit-less, the value of susceptibility is different in the cgs and SI systems of measurement because of the way electromagnetic derivations proceed within the two systems. Translation between cgs and SI systems of units is done via \\(\\kappa (SI) = 4 \\pi \\kappa(cgs) \\) . The SI system is the current preferred standard among most geophysicists, but you will find cgs used in older references and texts. For more details, see the sub-section on units in the "Geophysical Surveys" chapter, "Magnetics" section.  

Susceptibility of materials
===========================


Minerals
--------

Geologically significant magnetic minerals are either in the iron-titanium-oxygen group or in the iron-sulfur group. In the iron-titanium-oxygen group there are five main minerals, and in the iron-sulfur group there are two main minerals. There is apparently much more known about the first group. Grant and West, 1965, has an excellent summary, with a great deal of information about magnetism of minerals. The following table gives a simple indication of susceptibilities for specific magnetic minerals. 


+-----------------------+--------------------------+-----------------------------------+
|  **Mineral**          | **Chemical formula**     |  Average susceptibility (SI)      |
+=======================+==========================+===================================+
| Magnetite             | \\( Fe_3 O_4 \\)         |  \\( 6000 \\times 10^{-3} \\)     |
+-----------------------+--------------------------+-----------------------------------+
| Ulvospinel            | \\( Fe_2 TiO_4 \\)       |    \\( \\sim 0\\)                 |
+-----------------------+--------------------------+-----------------------------------+
| Ilmenite              | \\( FeTiO_3 \\)          |  \\( 1800 \\times 10^{-3} \\)     |  
+-----------------------+--------------------------+-----------------------------------+
| Hematite              | \\( Fe_2O_3 \\)          |   \\( 6.5 \\times 10^{-3} \\)     | 
+-----------------------+--------------------------+-----------------------------------+
| Maghemite             | \\( Fe_2O_3 \\)          |    similar to magnetite           |
+-----------------------+--------------------------+-----------------------------------+
| Pyrite                | \\( FeS_2 \\)            |   \\( 1.5 \\times 10^{-3} \\)     | 
+-----------------------+--------------------------+-----------------------------------+
| Pyrrhotite            |\\( Fe_{1-x}S(Fe_7S_8) \\)|  \\( 1500 \\times 10^{-3} \\)     |   
+-----------------------+--------------------------+-----------------------------------+


Rocks
-----

In rocks, susceptibility is mainly dependent on the volume percent of magnetite. This mineral is common in igneous and metamorphic rocks, and is present at least in trace amounts in most sediments. The chart below shows the ranges of magnetic susceptibility and magnetite volume for common rock types. Note that the susceptibility scale is logarithmic, so there is a huge range of susceptibilities in geological materials. Some relevant remarks are:

* Magnetite is by far the most common geologic magnetic material. The magnetic properties of most rocks depend on the proportion of magnetite within the rocks. See the approximate percent of magnetite by volume, highlighted by the red lines.
* Igneous rocks tend to be more magnetic than sedimentary rocks, but there is a very wide range of overlap.
* Magnetic minerals include metallic iron, nickel, cobalt, magnetite, pyrrhotite, and ulvospinel.
* Magnetite (SG ≈ 5) is heavy and often accumulates in sediments and alluvial environments in the same way that other heavy minerals form placer deposits. So, for example, ancient or hidden stream paths can sometimes be mapped because magnetite deposition will depend upon water flow rates. 
* Maghemite, a magnetic form of hematite, is produced in highly organic soils. Surface soils can acquire a remanent magnetization that is stronger than the induced magnetization, often as a result of human interference with fires or other disturbances. Implications are important for archeology.

.. figure:: ./images/susceptibility_chart.gif
	:align: center
	:scale: 100%	


A table summarizing typical susceptibilities of common materials follows:

+-----------------------+---------------------------------------------------------+
|  **Material**         | **Susceptibility (SI units, \\( \\times 10^{-3} \\) )** |
+=======================+=========================================================+
| Air                   |       about 0                                           |
+-----------------------+---------------------------------------------------------+
| Quartz                |       -0.01                                             |
+-----------------------+---------------------------------------------------------+
| Rock Salt             |       -0.01                                             | 
+-----------------------+---------------------------------------------------------+
| Calcite               |      -0.001 to 0.01                                     |
+-----------------------+---------------------------------------------------------+
| Sphalerite            |       0.4                                               |
+-----------------------+---------------------------------------------------------+
| Pyrite                |       0.05 to 5                                         |
+-----------------------+---------------------------------------------------------+
| Hematite              |       0.5 to 35                                         |
+-----------------------+---------------------------------------------------------+
| Illmenite             |       300 to 3500                                       |
+-----------------------+---------------------------------------------------------+
| Magnetite             |       1200 to 19200                                     |
+-----------------------+---------------------------------------------------------+
| Limestones            |       0 to 3                                            |
+-----------------------+---------------------------------------------------------+
| Sandstones            |       0 to 20                                           |
+-----------------------+---------------------------------------------------------+
| Shales                |       0.01 to 15                                        |
+-----------------------+---------------------------------------------------------+
| Schist                |       0.3 to 3                                          |
+-----------------------+---------------------------------------------------------+
| Gneiss                |       0.1 to 25                                         |
+-----------------------+---------------------------------------------------------+
| Slate                 |       0 to 35                                           |
+-----------------------+---------------------------------------------------------+
| Granite               |       0 to 50                                           |
+-----------------------+---------------------------------------------------------+
| Gabbro                |       1 to 90                                           |
+-----------------------+---------------------------------------------------------+
| Basalt                |       0.2 to 175                                        |
+-----------------------+---------------------------------------------------------+
| Peridotite            |       90 to 200                                         |
+-----------------------+---------------------------------------------------------+


Bulk susceptibility of rocks depends, of course, on what magnetic minerals are present, although there is no simple relationship. For example anisotropy is often present in metamorphic rocks, with smaller susceptibility in the direction normal to the textural trends (schistosity or gneissosity) than in a direction parallel to it. Banded magnetite or pyrrhotite are the most significant examples of rocks with anisotropic susceptibility. Magnetite is by far the most significant contributor to a rock's magnetic properties. There are several empirical relations between magnetite content and bulk susceptibility. Three such relations listed below (Grant and West, 1965) represent bulk susceptibility, \\(\\kappa\\), as a function of magnetite content by percent volume, \\(V\\). 

1. \\( \\kappa = 2.89 \\times10^{-3} \\; V^{1.01} \\)
2. \\( \\kappa = 2.6 \\times10^{-3} \\; V^{1.11} \\)
3. \\( \\kappa = 1.16 \\times10^{-3} \\; V^{1.39} \\)

Differences between the three formulae are probably due to the differences in the sample sets and separation process. Separation tends to overestimate the ferrimagnetic mineral content, while visual or microscopic examination tends to underestimate it. 

Soils
-----

(Summarized from Breiner, 1973) Magnetic susceptibility of soils might be expected to be related to the magnetite content of parent rocks. However magnetite is more resistant to weathering than other minerals. It is also denser than average materials and therefore subject to dispositional concentration. In addition, organic action is thought to be responsible for the formation of maghemite from other non-magnetic forms of iron oxide. For all these reasons, soils have very variable susceptibilities, and may have higher susceptibilities than suggested by the parent rocks. In any case, soil susceptibility can significantly impact ground-based surveys, creating noisy results that are often difficult to explain, or mitigate. 

Buried metal
------------

(Summarized from Breiner, 1973) For most iron or steel objects, the susceptibility, k, falls between 10 and 200 in SI units. However, predicting the response of a magnetometer survey over metal is complicated for several reasons. Remanent magnetisation is likely to be strong, and pointing in different directions in the various components of a buried object. For example, a buried pipe will often show up as a linear set of anomalies with variable character because each segment will have it's own magnetic signature. It should also be remembered that stainless steel is not magnetic, and that many potential targets may not even be ferrous (for example, aircraft frame parts are often some alloy with no magnetic properties). 

The maximum induced magnetic field strength (i.e. the maximum anomaly), \\(T\\), of a 3D object can be roughly estimated using \\(T = M/r^3\\) (or \\(T = 2M/r^3\\) for latitudes greater than \\(60^\\circ\\), where \\(M\\) is the magnetic moment estimated from \\(M = \\kappa F V\\) (\\(\\kappa\\) is susceptibility, \\(F\\) is ambient field strength,\\(V\\) is volume), and \\(r\\) is the distance to the target. For a 2D object, \\(T = M/r^2\\) is appropriate. 

Organically derived susceptibility
----------------------------------

Organic chemistry can be important in understanding magnetic survey results for petroleum exploration applications. Under certain conditions magnetic anomalies caused by organic chemical activity can provide indicators of petroleum reservoir in underlying rocks. This is described in a supplementary article (Stone et al, 2004).


Field measurements of magnetic susceptibility using a KT10
----------------------------------------------------------

.. figure:: 
	../physical_properties/images/magnetic_susceptibility_measurement_kt10.jpg

References cited on this page 
-----------------------------

**Rock Physics and Phase Relations:** An AGU online reference, © by the American Geophysical Union, 1995.

**Blakely, R.J.** , *Potential Theory in Gravity and Magnetic Applications*, Cambridge University Press 1995.

**Breiner, S, 1973**, *Applications manual for portable magnetiometers*, published by Geometrics.

**Emerson, D. W., and The Australian Society Of Exploration Geophysicists**, *The Geophysics of the Elura Orebody, Cobar, New South Wales: the Proceedings of the Elura Symposium, Sydney, 1980: a Collection* ..., Australian Society of Exploration Geophysicists, 1980, ISBN: 0959413103.

	* Adams, R.L. and Schmidt, B.L. (1980), "Geology of the Elura Zn-Pb-Ag Deposit" , in Emerson, D.W., pp1-4.
	* Blackburn, G. (1980), "Gravity and Magnetic Surveys - Elura Orebody", in Emerson, D.W., pp17-24.
	* Emerson, D.W. (1980), "Discussion on exploration, geology, gravity and magnetics- Elura symposium, Sydney, 1980", in Emerson, D.W., pp188 - 193.
	* Gidley, P.R. and Stuart, D.C. (1980), "Magnetic property studies and magnetic surveys of the Elura prospect, Cobar, NSW", in Emerson, D.W., pp25-30.

**Grant, F.S. and West, G.F.**, 1965, *Interpretation Theory in Applied Geophysics*, McGraw-Hill Book Co.

**Stone, V.C.A., J. Derek Fairhead, W. Heiko Oterdoom, and Petronas Carigali**, *Micromagnetic seep detection in the Sudan*, The Leading Edge, 2004, Vol.23, #8, p. 734, The Society of Exploration Geophysicists. (See also the same authors at the Getech website under education or publications.


