.. _depth_of_penetration:

Depth of Penetration
********************

If we are attempting to find a conducting target then the ability to see the
target depends upon the coil orientation and coil separation. It must also
take into account the fact that the:

1. primary field is attenuated before it reaches the target
2. the secondary fields are attenuated as they travel from the target to the receiver.

Apparent Conductivity from the Quadrature Component
===================================================

If the spacing \\(s\\) between the coils is much less than the skin depth,
that is, \\(s << \\delta\\) then the ratio of secondary to primary field is
approximately

.. math::
         \left| \frac{H_s}{H_p} \right| \simeq \frac{\omega \mu_0 \sigma s^2}{4}  

The response is purely imaginary or is found in the quadrature component. The
constant conductivity which gives rise to the observed response can be found
from the above formula. It is referred to as the apparent conductivity
\\(\\sigma_a\\).

.. math::
        \sigma_a = \frac{4}{\omega \mu_0 \sigma s^2} \left| \frac{H_s}{H_p} \right| 

Further insight about the apparent conductivity is obtained by incorporating
the response curves \\(\\phi_V(z)\\) and \\(\\phi_H(z)\\). We have

.. math::
        \sigma_a &= \int_{0}^{\infty} \phi_V (z) \sigma (z) dz \\[0.8em]
        \sigma_a &= \int_{0}^{\infty} \phi_H (z) \sigma (z) dz

respectively for the vertical and horizontal dipoles.

Multilayer Earth Structures
===========================

Under the assumption that \\( s << \\delta \\)  then the above formulae can be
used to predict the apparent conductivity from a multilayered earth, or to
used measured apparent conductivities to estimate the individual layer
thickness and conductivities. For instance if we coplanar coils on the earth's
surface given below

.. figure:: ./images/coplanar_coils.jpg
    :align: center
    :scale: 100 %

The apparent conductivity would be

.. math::
        \sigma_a &= \int_{0}^{h} \sigma_1 \phi_V (z) dz + \int_{h}^{\infty} \sigma_2  \phi_V (z) dz \\[0.8em]
                 &= \sigma_1 (1-R_V(h)) + \sigma_2 R_V(h)   

Either the curves shown previously or the following formulae are therefore useful:

.. math::
        \phi_V (z) &= \frac{4z}{(4z^2 + 1)^{3/2}} \\[0.8em]
        \phi_H (z) &= 2- \frac{4z}{(4z^2 + 1)^{1/2}} \\[0.8em]  
               R_V &= \frac{1}{(4z^2 + 1)^{1/2} }\\[0.8em]
               R_H &=  (4z^2 + 1)^{1/2} - 2z \\[0.8em]