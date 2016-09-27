.. _basic_principles:

Basic principles
*******************


Elastic model for Earth rocks
=================================

When the earth is deformed elastically, the small strains will propagate away in all directions from the site of the original stress. The easiest way to obtain intuition about this is to think about rocks as being made up of a set of connected springs. Apply a force (stress) to any part and you will eventually get motion elsewhere. This propagation of energy is a type of wave motion. Elastic waves can be divided into two categories:

.. sidebar:: Elastic model for rocks

	.. figure:: ./images/springbox.png
		:align: center

1. **Body waves** which travel through materials

2. **Surface waves** which propagate along boundaries between materials such
   as the air/earth interface.

Subtypes of these two categories are described below. Each wave type travels through a given material with a velocity that depends upon the elastic properties and density of the material.


Body Waves
==========

**Compressional waves (P waves)** propagate by compression and rarefaction and
the velocity of such waves, :math:`v_p`, in a material with bulk modulus :math:`K`, shear modulus :math:`\mu`, and density :math:`\rho` is given by the equation

.. math::
	v_p = \sqrt{ \frac{K + 4/3\mu}{\rho} }.

The figure below shows a simple animation of the motion associated with P waves.

.. figure:: ./images/pwave-animated-2.gif
	:align: center

	Animation by `L. Braile`_, from his `seismic wave demo`_, licensed for non-commercial reuse.


**Shear waves (S waves)** propagate by a pure shear strain perpendicular to the
wave propagation. The propagation speed :math:`v_s` is given by

.. math ::
	v_s = \sqrt{\frac{\mu}{\rho} }.

The below animation shows the propagation of a vertically polarized S wave. Note that an S wave could also be horizontally polarized, meaning that particle motion would be in the y direction in the coordinate system of the animation, as opposed to the z direction for vertical polarization.

.. figure:: ./images/s-wave-animated.gif
	:align: center

	Animation by `L. Braile`_, from his `seismic wave demo`_, licensed for non-commercial reuse.

Note that if :math:`\mu = 0` then :math:`v_s = 0`. This tells us that shear
waves do not travel in a liquid.

Seismic reflection and refraction surveying is usually carried out by the analysis of P waves. S-waves can also be used but they are harder to generate artificially compared to P-waves and require more complex receivers than ones designed to measure just P waves. In marine surveys (unless sources and receivers are coupled directly to the ocean bottom) it is not possible to generate or measure P waves at all. However, since :math:`v_s < v_p`, there are situations where it is beneficial to
use S-waves instead of P-waves.


Surface Waves
=============

**Rayleigh waves** propagate along a free surface or on the boundary between two
materials. Particle motion is a retrograde ellipse, and in the same plane as
wave energy propagation. The amplitude of particle motion decays
exponentially with depth. Rayleigh wave speed :math:`v_R < v_S`. Large
earthquakes can generate Rayleigh waves that circumnavigate the globe. This
provides information about the velocity structure in the upper few hundred
kilometers of the earth.

.. figure:: ./images/Rayleigh-wave-animated.gif
	:align: center

	Animation by `L. Braile`_, from his `seismic wave demo`_, licensed for non-commercial reuse.


**Love waves** exist in a surface layer when the shear wave velocity of the
upper layer is less than the shear wave velocity of the lower layer. The
waves are trapped in the upper layer and the particle motion is parallel to
the free surface and perpendicular to the direction of propagation.

.. math::
	v_{S1} < v_{Love} < v_{S2}

.. figure:: ./images/Love-wave-animated.gif
	:align: center

	Animation by `L. Braile`_, from his `seismic wave demo`_, licensed for non-commercial reuse.

Both Love waves and Rayleigh waves are **dispersive**. That is, different
frequency components travel at different speeds. So the wave changes shape as
it travels. Also, the dispersion can be used to provide information about the
velocity structure in the upper region of the earth. For shallow work, it is
possible to generate surface waves artificially, and then observe the waves at
a series of locations at increasing distances from the source. This type of
field work is sometimes called **multi-channel analysis of surface waves** or
MASW. This is usually considered an "advanced" topic in applied geophysics.


Wave Velocity and Particle Velocity
===================================

Seismic waves typically travel in the ground at 2-7 km/s. This is the velocity
at which the energy moves, not the particles themselves. For comparison, sound
travels in air at approximately 0.33 km/s. The wave energy can be recorded
many kilometers from the source even if the source is small. The velocity and
displacements of individual particles in the rocks are however very small;
typical particle speeds are :math:`10^{-8}` m/s and typical ground
displacements are :math:`10^{-10}` m. For a list of velocities of some common
earth materials and a discussion of the geological factors that affect
velocities please see the :ref:`seismic velocity <seismic_velocity_duplicate>` page on the physical properties
section of this site.


Attenuation
===========

The amplitude of seismic waves falls off with distance from the source. There
are two primary reasons:

1. Geometrical spreading - that is, energy falls off as 1/r2 and hence the amplitude falls of as 1/r.

2. Earth materials are not perfectly elastic. Some frictional heating occurs
   as the waves propagate through the earth. This is often described as
   "absorption" and the absorption coefficient expresses the proportion of energy
   lost as the wave travels a distance of one wavelength. The figure here shows
   the progressive change of shape of an original spike pulse during its
   propagation through the ground due to the effects of absorption (After Anstey
   1977.) The spike's shape changes as well as experiencing reduced amplitude.
   This is because the different frequencies making up the pulse decay at
   different rates - in fact, higher frequencies decay more rapidly than lower
   frequencies. This is easily observed on earthquake signals that have been
   recorded at different locations. As noted above in the context of surface
   waves, such frequency dependent behavior is called **dispersion**.

.. figure:: ./images/attenuation.gif
	:align: center


Waves and Rays
==============

A wave is a representation of the propagation of energy. In the case of seismic waves, energy is propagated through the compressions and expansions of the earth. Energy propagates away from source with a distinct pattern. Most seismic sources can be represented spatially as point sources. In a uniform medium, energy propagates away from the source in an expanding spherical pattern, much like ripples on a pond that's been disturbed.

.. figure:: ./images/pondwaves-noleaves.jpg
        :align: center

In the pond example, each ring forms a coherent surface where the water is disturbed from equilibrium by an equal amount. These rings propagate outward in time, in a coherent manner.
        
.. figure:: ./images/Sonar_Principle_EN-modified-from-wikipedia-radar-article.svg.png
        :align: center
        
        Adapted from `Wikipedia <https://commons.wikimedia.org/wiki/File:Sonar_Principle_EN.svg>`__, licensed under `CC BY 3.0`_.

A wavefront indicates the locations at which the phase of the wave has the same value. For example, visualize the peaks (or troughs) of water ripples after a rock has been thrown in. The direction of propagation of the energy is normal to the wavefront. **Seismic rays** are imaginary lines perpendicular to the wavefront that indicate the path along which the wavefront is traveling. Rays are not physical entities. They exist only to illustrate where the energy travels.

.. figure:: ./images/wavefront.gif
	:align: center


Reflection and transmission of plane waves
==========================================

When a wave strikes an interface between two materials with differing physical properties, some of the wave energy will be reflected and the rest will be transmitted through or along the interface. All of the processing and interpretation methods we will discuss will assume that a seismic wave striking the interface between materials of differing physical properties can be approximated as a plane wave. We define a new quantity called acoustic impedance as :math:`Z = \rho V`, the product of density and velocity. The velocity in question could be for either P or S waves. The relative amplitudes of the reflected and transmitted waves will depend on the acoustic impedances of the two materials. Let :math:`A_0`, :math:`A_1` and :math:`A_2` be the amplitudes of the incident, reflected, and transmitted waves, respectively. The ratios of :math:`A_1` and :math:`A_2` to :math:`A_0` are given by the reflection and refraction coefficients:

**Reflection Coefficient:**

.. math::
    R = \frac{A_1}{A_0} = \frac{Z_2 - Z_1}{Z_2 + Z_1} \qquad -1 \le R \le 1

**Transmission Coefficient:**

.. math::
    T = \frac{A_2}{A_0} = \frac{2 Z_1}{Z_2 + Z_1} \qquad 0 \le T \le 2

Displacement of the earth from equilibrium position must be continuous across any interface. This guarantees that :math:`A_0 = A_1 + A_2`. We make note of the values of :math:`R` and :math:`Z` in some important special cases:

1. If :math:`Z_1 = Z_2`:   :math:`R = 0`,  :math:`T = 1`

2. If   :math:`Z_1 >> Z_2`:   :math:`R = -1`,  :math:`T = 2`.  The value :math:`R
   = -1` means that the pulse will be reflected with a polarity change, for
   example at the rock-air interface, with an upward traveling wave.

3. If   :math:`Z_2 >> Z_1`   :math:`R = 1`,  :math:`T = 0` (air earth
   interface with downward traveling wave).

**Remark:**  Large amplitudes of the transmitted wave are sometimes counter-
intuitive. However, the energy transported in an acoustic wave is

.. math::
    \text{Energy} = \frac{1}{2} \rho v \omega^2 A^2 \approx ZA^2


So even though there is an enhanced amplitude of a transmitted wave in certain
situations, there is still loss of energy. The ratio of incoming to reflected
energy is :math:`E_R` and the ration of incoming to transmitted energy is :math:`
E_T`. The values of these rations are

.. math::
    E_R = \left( \frac{Z_2 - Z_1}{Z_2 + Z_1} \right)^2

.. math::
    E_T = \frac{4 Z_1 Z_1}{(Z_2 + Z_1 )^2}

.. math::
    E_R + E_T = 1    

.. Transmitted wave will be refracted, meaning it will be bent. Check out https://www.youtube.com/watch?v=FygYDmm99SA. The direction of the refracted ray can be computed from Snell's law.

.. At the critical angle, wave will travel along interface and head waves will be generated according to Huygen's principle. Head waves propagate back toward surface at the critical angle.


.. Another refraction/head wave video https://www.iris.edu/hq/inclass/animation/seismic_wave_behavior_a_single_boundary_refracts__reflects

.. Site with some head wave figures: http://www.ucl.ac.uk/EarthSci/people/lidunka/GEOL2014/Geophysics4%20-%20Seismic%20waves/SEISMOLOGY%20.htm



.. _CC BY 3.0: https://creativecommons.org/licenses/by/3.0/
.. _Subsurface Wiki: http://subsurfwiki.org/
.. _L. Braile: http://web.ics.purdue.edu/~braile/
.. _seismic wave demo: http://web.ics.purdue.edu/~braile/edumod/waves/WaveDemo.htm
