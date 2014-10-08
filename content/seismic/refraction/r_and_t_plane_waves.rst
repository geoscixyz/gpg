.. _seismic_reflection_refx_trans_plane_waves:

Reflection and Transmission of Plane Waves
******************************************

Energy at velocity boundaries
-----------------------------

If we are some distance away from the source, then the seismic wave will look like a plane wave. That is, the wavefront will look like a planar surface. Imagine such a plane wave which impinges at a boundary at normal incidence.

.. figure:: ./images/Attenuation.png
    :align: center

    Energy across a velocity boundary, where, \\(A_0\\) is the amplitude of the incident wave; \\(A_1\\) is the amplitude of the reflected wave; \\(A_2\\) is the amplitude of the transmitted wave

We define here the "Acoustic Impedance" \\( Z = \\rho V \\), or the product of density and velocity. Energy is reflected and transmitted at the interface. We define next expressions which describe the efficiency of reflection and transmission.

**Reflection Coefficient:**

.. math::
    R = \frac{A_1}{A_0} = \frac{Z_2 - Z_1}{Z_2 + Z_1} \qquad -1 \le R \le 1

**Transmission Coefficient:**

.. math::
    T = \frac{A_2}{A_0} = \frac{2 Z_1}{Z_2 + Z_1} \qquad 0 \le T \le 2


Note that at the interface there is continuity of displacement so that \\(A_0 = A_1 + A_2\\).

.. Move to reflection and transmission section (Phil, 02,10,2014)
Special Cases
=============

1. If \\( Z_1 = Z_2 \\):   \\( R = 0 \\),  \\( T = 1 \\)
2. If   \\( Z_1 >> Z_2 \\):   \\( R = -1 \\),  \\( T = 2 \\).  The value \\( R = -1 \\) means that the pulse will be reflected with a polarity change, for example at the rock-air interface, with an upward traveling wave.
3. If   \\( Z_2 >> Z_1 \\)   \\( R = 1 \\),  \\( T = 0 \\) (air earth interface with downward traveling wave).

**Remark**:  Large amplitudes of the transmitted wave are sometimes counter-intuitive. However, the energy transported in an acoustic wave is

.. math::
    \text{Energy} = \frac{1}{2} \rho v \omega^2 A^2 \approx ZA^2


So even though there is an enhanced amplitude of a transmitted wave in certain situations, there is still loss of energy. The ratio of incoming to reflected energy is \\( E_R \\) and the ration of incoming to transmitted energy is \\( E_T \\). The values of these rations are

.. math::
    E_R = \left( \frac{Z_2 - Z_1}{Z_2 + Z_1} \right)^2

.. math::
    E_T = \frac{4 Z_1 Z_1}{(Z_2 + Z_1 )^2}

.. math::
    E_R + E_T = 1