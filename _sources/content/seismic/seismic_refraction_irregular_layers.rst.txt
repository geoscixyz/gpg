.. _seismic_refraction_irregular_layers:

.. <<place holder>> This section is to be put on hold for now. This .rst file is a placeholder for this section.

Irregular Surfaces and the Plus-Minus Method
********************************************


There is one more step of sophistication that is required so that the
refraction technique is useful. This occurs in environments where the
interface has  topography and is no longer approximated by a plane. If the
curvature of the interface is not too great then we can still think of the
refracted wave travelling along the interface. The wave travels at the speed
of the lower medium. Consider the sketch to the right. Formulae which
explicitly assume a plane interface (even dipping) do not work well enough. We
need a better approximation.

We would like to be able to obtain the depth of the interface beneath the
source and receiver. To do this we used the concept of *delay time*. Consider
the diagram to the right. The travel time is :math:`t = x/v_2 + t_i`  where
:math:`t_i` can be thought of as the time delay.
	

The delay time can be partitioned into two parts: (1) the "delay" associated
with the source location and (2) the "delay" associated with the receiver
location.  Consider the delay at the source.

Let the delay time be denoted by

.. math::
	a = \frac{z}{v_2 \sin\theta \cos\theta} - \frac{z}{v_2}\tan\theta = \frac{z}{v_2\tan\theta}

Finally, using the definition of the velocity triangle we can write 

.. math::
	z = \frac{av_1v_2}{(v_2^2 - v_1^2)^\frac{1}{2}} 

Thus the depth can be computed if the delay time, :math:`a`, can be measured.

We can write any general travel time so that it involves a delay at the source
:math:`a_s` and a delay at the receiver or detector :math:`a_d` . It looks like
this:

.. math::
	t = \frac{x}{v_2} + a_s + a_d.

As in the diagram at the top of this page, :math:`a_s` and :math:`a_d` might be
very different. To make progress we implement Hagedoorn's "Plus-Minus" method.
This method will also make it possible to estimate depths under every geophone
that has a refracted signal from both sources. This will yield several depths
under the survey line rather than just two depths under sources, thus allowing
more detailed image of the interface's shape.

Hagedoorn's Plus-Minus Method
-----------------------------

The geometry  illustrates the two shots occurring at locations :math:`S_1` and
:math:`S_2`. The point indicated by :math:`D` lies at any location (i.e. any
geophone) between the two shots where refractions can be received from both
shots. Let :math:`a_{S1}` and :math:`a_{S2}` denote the delay times at the two
shot locations. Although the refracting interface is not flat beneath :math:`D`,
the slope is not large an d the ray path lengths :math:`AD` and :math:`BD` are
almost identical.

Let us write all portions of the travel times for signals that would travel
between :math:`S1` and :math:`S2`, between :math:`S1` and :math:`D`, and
between :math:`S2` and :math:`D`. These travel times are:

.. (Phil, 5/10/2014: This section is marked as to be done later.)
