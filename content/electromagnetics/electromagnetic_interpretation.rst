.. _electromagnetic_interpretation:

Interpretation
**************



Apparent Conductivity from the Quadrature Component
===================================================

If the spacing :math:`s` between the coils is much less than the skin depth,
that is, :math:`s << \delta` then the ratio of secondary to primary field is
approximately

.. math::
         \left| \frac{H_s}{H_p} \right| \simeq \frac{\omega \mu_0 \sigma s^2}{4}

The response is purely imaginary or is found in the quadrature component. The
constant conductivity which gives rise to the observed response can be found
from the above formula. It is referred to as the apparent conductivity
:math:`\sigma_a`.

.. math::
        \sigma_a = \frac{4}{\omega \mu_0 \sigma s^2} \left| \frac{H_s}{H_p} \right|

Further insight about the apparent conductivity is obtained by incorporating
the response curves :math:`\phi_V(z)` and :math:`\phi_H(z)`. We have

.. math::
        \sigma_a &= \int_{0}^{\infty} \phi_V (z) \sigma (z) dz \\[0.8em]
        \sigma_a &= \int_{0}^{\infty} \phi_H (z) \sigma (z) dz

respectively for the vertical and horizontal dipoles.