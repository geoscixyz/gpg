.. _primary_field_in_the_earth:

Primary Field in the Earth
==========================

The strength of the primary field depends upon:

#. frequency of the transmitter
#. conductivity of the host material
#. geometry of the source

Considerable insight can be obtained by first ignoring the geometry of the
source and observing how a plane electromagnetic wave decays as it propagates
into the earth. An incoming sinusoidal wave with frequency \\(\\omega = 2 \\pi
f\\) travels in the atmosphere at the speed of light \\(c = 3 \\times 10^8\\)
m/s and has a wavelength \\(\\lambda = c/f\\). When the wave enters the
conducting earth it still propagates as a sinusoid but it travels much slower
and attenuates rapidly. An example, with numbers for speed and wavelength is
given below.


.. figure:: ./images/EM_diffusion.jpg
    :align: center
    :scale: 80 %

The wave attenuates so fast that it only propagates about a wavelength into
the earth. Because the amplitude diminishes so rapidly and the waves travel so
slowly, we generally talk about the EM wave "diffusing" into the earth. The
amplitude of the field decays exponentially with depth according to the
diagram given below.

.. figure:: ./images/field_decay.jpg
    :align: center
    :scale: 100 %

.. math::
        H  &= H_0 e^\frac{-(1-i)z}{\delta}\\[0.4em]
       \mid H \mid &= H_0 e^\frac{-z}{\delta}

**Skin Depth:** This is the depth by which the amplitude has decayed to
\\(1/e\\) of its surface value. For a uniform halfspace of conductivity
\\(\\sigma\\) the skin depth \\(\\delta\\) is

.. math::
        \delta = \sqrt{\frac{2}{\mu_0 \omega \sigma} } \simeq 500 \sqrt{\frac{1}{\omega f}} = 500 \sqrt{\frac{\rho}{f}} \text{meters}