.. _seismic_refraction_horizontal_layers:

Refraction Interpretation for Horizontal Layers
***********************************************


The goal of a seismic refraction experiment is generally to determine depth to bedrock, depth to water table, or to delineate major sedimentary layers. In its complete generality, the seismic refraction problem is quite complicated. However, there are certain geometries for which formulae can be generated to predict the arrival times. With the aid of these formulae, measurements of the refracted arrivals can be used to determine layer parameters. We will restrict ourselves to the following situations:

1. The subsurface is composed of layers separated by planes and possibly dipping interfaces.
2. The seismic velocity in each layer is constant.
3. The layer velocities increase with depth.
4. The ray paths are in the vertical plane. That is, there is no cross-dip (which means dipping into or out of the page in the figure to the right).

.. figure:: ./images/refrac3layerintro.gif
	:align: center

With the above assumptions, there are a number of special cases to be considered.

1. A 2-layer earth with a horizontal interface.
2. A 3-layer (and multiple-layer) earth with horizontal interfaces.
3. A 2-layer earth with a dipping interface.

In all cases, the development of the travel-time curves requires only that we know the rules of propagation, i.e., energy travels in straight lines in a uniform medium and refracts according to Snell's law when it enters a medium with different velocity. We must also be able to calculate the lengths of the ray path in each layer and along the refractor. Travel-time curves are graphs showing the travel-time, \\(t\\), (length of time for a seismic signal to travel from the source to the receiver along which ever path is being considered) versus distance between the source and receiver, \\(x\\).

One layer over basement - the horizontal interface
==================================================

We need to identify specific ray paths and their associated travel times. Consider an earth composed of a uniform layer with velocity \\(v_1\\) and thickness \\(z\\) overlying a medium with velocity \\(v_2\\). Let \\(\\theta\\) be the critical angle and x denoted the distance between the source at \\(A\\) and a receiver at \\(D\\).  Let \\(x_c\\) denote the critical distance.

.. figure:: ./images/refracHzGeometry.gif
	:align: center

.. sidebar:: triangle

	.. figure:: ./images/lengthTriangle.gif
		:align: center

From elementary geometry the following relationships hold:

.. math::
	x_c = 2z\tan\theta \quad l=\frac{z}{\cos\theta}
or

.. math::
	\tan\theta = \frac{x_c}{2z} \quad \cos\theta = \frac{z}{l}

The travel time is the cumulative time for the wave to traverse the path \\(ABCD\\). This is \\(t=t_{AB}+t_{BC}+t_{CD}\\).


Generally time = distance / velocity, so we can write \\(t_{AB} = L/v_1 = (z/cos\\theta) / v1\\), (using \\(L\\) from just above).

Also, we can note that \\(t_{AB} = t_{CD}\\) and the distance \\(BC\\) is \\(x-x_c\\). So we can now state that \\(t=2t_{AB}+t_{BC}\\) , or

.. math::
	t = \frac{2z}{v_1\cos\theta} + \frac{x-2z\tan\theta}{v_2}

.. sidebar:: velocity triangle

	.. figure:: ./images/velocitytriangle.gif
		:align: center

It is convenient to rearrange this slightly differently. Using the definition for critical angle  \\(\sin\\theta=v_1/v_2\\), we can make the "velocity triangle", so expressions for the angle arise directly from simple trigonometry:

.. math::
	\cos\theta = \frac{\sqrt{v_2^2-v_1^2}}{v_2}

.. math::
	\tan\theta = \frac{v_1}{\sqrt{v_2^2-v_1^2}}


Use these two relations for \\(\\cos\\) and \\(\\tan\\) in the expression for t above to obtain a useful set of relations.

.. math ::
	t = & \frac{x}{v_2} + \frac{2z\sqrt{v_2^2-v_1^2}}{v_1v_2} \\
	  = & \frac{x}{v_2} + t_i

This simple relation says that the travel time curve is a straight line which has a slope of \\(1/v_2\\) and an intercept of \\(t_i\\). This intercept time is the time where the refraction line extends to intercept the \\(y\\)-axis **above the source position**. This is not a real "time" - it is derived from the graph.

.. figure:: ./images/interpretingArrivals.gif
	:align: center

The velocities of the seismic layers and the layer thickness are obtained in the following manner.

1. Plot the times of first arrivals on an time-offset plot ("offset" is distance between source and geophone).
2. The direct arrivals are observed to lie along a straight line joining the origin. The slope of this line is \\(1/v_1\\), giving the velocity of the upper layer.
3. The refracted arrivals appear as a straight line with smaller slope equal to \\(1/v_2\\), giving the velocity of the lower layer.
4. For the refracted wave, this intercept time is

.. math::
	t_i = \frac{2z\sqrt{v_2^2-v_1^2}}{v_1v_2}

so

.. math::
	z = \frac{t_iv_1v_2}{2\sqrt{v_2^2-v_1^2}}


We therefore can obtain all three useful parameters about the earth, \\((v_1, z, v_2)\\).

There is another useful point that is observable from the first arrival travel-time plot. We can often discern the crossover distance. Since this is the location where the direct wave and the refracted wave arrive at the same time, we can write

.. math::
	\frac{x_{\text{cross}}}{v_1} = \frac{x_{\text{cross}}}{v_2} + t_i

Thus

.. math::
	x_{\text{cross}}\left(\frac{1}{v_1} - \frac{1}{v_2}\right) = t_i

.. math::
	x_{\text{cross}} &= \left(\frac{v_1v_2}{v_2-v_1}\right)t_i \\
	&= \frac{v_1v_2}{v_2-v_1}\frac{2z}{v_1v_2}\sqrt{v_2^2-v_1^2} \\
	&= 2z\sqrt{\frac{v_2+v_1}{v_2-v_1}}
This can be used as a consistency check, or it can be used to compute one of the variables given values for two others.

Two Horizontal Layers Over a Halfspace
======================================

The extension to more layers is in principle straight forward. Snell's law holds for waves at all interfaces, so for a multi-layered medium

.. math::
	\frac{\sin\theta_1}{v_1} = \frac{\sin\theta_2}{v_2} = \frac{\sin\theta_3}{v_3} = ...

For a three layer case, the algebra is slightly more involved compared to a two layer example because we need to compute the times due to the ray path segments in the two top layers. Consider the diagrams below:

.. figure:: ./images/twoHorizontalLayers.gif
	:align: center

.. figure:: ./images/twoHorizontalLayersTime.gif
	:align: center


Using arguments that are entirely analagous to the two layer case (above) the travel time for the wave refracted at the top of layer three is given by

.. math::
	t &= \frac{x}{v_3} + \frac{2 z_1 \cos\theta_1}{v_1} + \frac{2z_2\cos\theta_2}{v_2} \\
	&= \frac{x}{v_3} + t_{i1} + t_{i2}

All quantities are defined in the diagrams, and the angles are

.. math::
	\theta_1 = \sin^{-1}\left(\frac{v_1}{v_3}\right) \quad \text{and} \quad \theta_2 = \sin^{-1}\left(\frac{v_2}{v_3}\right)

Note that \\(\\theta_2\\) is a critical angle while \\(\\theta_1\\) is not. You can prove the relation for  \\(\\theta_1\\) yourself by using Snell's law at the two interfaces, and recalling that the angle of the ray coming from point \\(B\\) is the same as the angle arriving at point \\(C\\).
The straight line that corresponds to an individual refractor provides a velocity (from its slope) and a thickness (from the intercept). Thus the information on the above travel-time plot allows us to recover all three velocities and the thickness of both layers.

The travel time curves for multi layers are obtained from obvious extension of the above formulation.
