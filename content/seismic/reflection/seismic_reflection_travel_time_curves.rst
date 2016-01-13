.. _seismic_reflection_travel_time_curves:

Travel Time Curves for a Single Layer
*************************************


.. figure:: ./images/travel_time_fig1.gif
	:figclass: float-right-360
	:align: right
	:scale: 100 %

Consider the situation to the right, in which there is a source :math:`S` and a
set of receivers on the surface of the earth. The earth is a single uniform
layer overlying a uniform halfspace. A reflection from the interface will
occur if there is a change in the acoustic impedance at the boundary.

Let :math:`x` denote the "offset" or distance from the source to the receiver.
The time taken for the seismic energy to travel from the source to the
receiver is given by


 .. math::
 		t = \frac{(x^2 + 4z^2)^\frac{1}{2}}{v}

This is the equation of a hyperbola. In seismic reflection (as in radar) we
plot time on the negative vertical axis, and so the seismic section (without
the source wavelet) would look like.


.. figure:: ./images/NMO_hyperbola.gif
	:align: center
	:scale: 130 %

Two way travel time:

.. math::
 		t_0 = \frac{2z}{v} 

Normal Moveout: 

.. math::
 		\Delta T = t(x) - t_0


In the above diagram :math:`t_0` is the 2-way vertical travel time. It is the
minimum time at which a reflection will be recorded. The additional time taken
for a signal to reach a receiver at offset :math:`x` is called the "Normal
Moveout" time, :math:`\Delta T`.  This value is required for every trace in the
common depth point data set in order to shift echoes up so they align for
stacking. How is it obtained? First let us find a way of determining velocity
and :math:`t_0`.

For this simple earth structure the velocity and layer thickness can readily
be obtained from the hyperbola. Squaring both sides yields,

.. math::
 		t^2 = t_0^2 + \frac{x^2}{v^2}

.. figure:: ./images/tsqrd_xsqrd_plot.gif
	:figclass: float-right-360
	:align: right
	:scale: 120 %

This is the equation of a straight line when :math:`t^2` is plotted against
:math:`x^2`.  Now, to find :math:`\Delta T`, we must rearrange this hyperbolic
equation relating :math:`t_0`, :math:`x`, the :math:`Tx`--:math:`Rx` offset, :math:`t`
at :math:`x`,  or :math:`t(x)`, and the ground's velocity, :math:`v`.


.. math::
 		t^2 &= \frac{x^2 + 4z^2}{v}
 			= \frac{4z^2}{v^2}\left(\frac{x^2}{4z^2} + 1 \right)\

 		  t &= \frac{2z}{v} \sqrt{ 1 + (\frac{x}{2z})^2 }
 		    = t_0 \sqrt{ 1 + \left(\frac{x}{vt_0}\right)^2 }\

Apply binomial expansion to get

.. math::
 		  t &\approx  t_0 \left(1 + \frac{1}{2} \left(\frac{x}{vt_0} \right)^2  \right)\quad if \quad \frac{x}{vt_0} << 1

Now, since normal moveout is :math:`\Delta T = t_x - t_0`

.. math::
		\Delta T \approx \left(t_0 + \frac{t_0x^2}{2v^2t_0^2} \right) - t_0 \approx \frac{x^2}{2v^2t_0}

The algebra has only one complicated step--a binomial expansion must be
applied to obtain a simple relation without square roots etc.

The approximation is valid so long as the source-receiver separation (or
offset) is "small" which means much less than the vertical depth to the
reflecting layer (i.e. :math:`x << vt_0`). The result is a simple expression for
normal moveout.

Each echo can be shifted up to align with the :math:`t_0` position, so long as
the trace position, :math:`x`, the vertical incident travel time, :math:`t_0`, and
the velocity are known. Velocity can be estimated using the slope of the
:math:`t^2`--:math:`x^2` plot, or with several other methods, which we will
discuss in pages following.


