.. _seismic_refraction_dipping_layers:

Interpretation when layers are dipping
**************************************

Earth layers can often be approximated as planar, but they are rarely horizontal.  The next level of complication is to assume that the layers have some dip associated with them. Consider a single interface which is dipping at an angle [theta] with respect to the horizontal. The critical angle is still defined by the angle that an incoming wave must make with respect to the **normal** of the refractor. This is shown by the left diagram below.

.. Need to put second gif side by side with this one (Phil, 04/10/2014): dip_layer_x_t_lines.gif

.. figure:: ./images/dip_layer_first_arrival.gif

Arrival times of the refracted wave will still appear as a straight line on the travel time plot. However, as the refracted wave moves updip the waves have less distance to travel to the surface. The travel time is reduced and thus the slope of the line is reduced. The velocity recovered from using this slope is called \\(v_{2u}\\), and is called the updip "apparent" velocity. This will be larger than the true velocity of the layer.

Conversely, if you are downdip then the distance travelled by the refracted wave increases with distance and it takes longer for the waves to reach you. The slope of the refracted arrival on the travel time plot will increase and the apparent downdip velocity \\(v_{2d}\\) estimated from this slope will be smaller than the true velocity. 

.. figure:: ./images/dip_layer_S_R_schematic.gif
.. figure:: ./images/dip_layer_x_t_lines2.gif

**Therefore, having receivers only updip or downdip from the source provides only an apparent velocity and no indication that there is a dipping interface.**

Intuitively, if we want to obtain another parameter (namely the dip angle, designated \\( \\gamma\\)), then we need more data. We can achieve this by having two shots so that both updip and downdip apparent velocities can be obtained. This requires shots at both ends of the spread. 

Consider the geometry and travel time curves shown to the right.  Note that \\(h\\) is depth (vertical distance) of the interface beneath the shot at A. The distance from A to the normal of the interface is given by \\(z\\). These quantities are given by \\((h', z')\\) for the source at D. The traveltimes \\(t_{AD}\\) (time for the wave to go from A to D) and \\(t_{DA}\\) (the time for the wave to go from D to A) are called the "reciprocal times."  It is should be obvious from geometry that these time are equal. 

Note the reciprocal travel times are sometimes erroneously considered as the travel times from first to last geophones of a spread, even though these first and last geophones do not always coincide with the two shot locations. Reciprocal times are total travel times from source location to the last receiver location.

Checking for equal reciprocal times is a common test of the quality of the data. Don't forget that the reciprocal time for each shot is found as the intersection of the refraction line with the time axis above the other shot (not at the "arbitrary" time axis). Extending the line with a ruler is an acceptable way of finding these times.

The traveltime for receivers in the downdip direction is 


.. math::
	t_2 = \frac{x\sin(\theta + \gamma)}{v_1} + \frac{2z\cos\theta}{v_1} = \frac{x}{v_{2d}}+{t_i} \quad (1)

The traveltime in the updip direction is 

.. math::
	t^{\prime}_2 = \frac{x\sin(\theta-\gamma)}{v_1} + \frac{2z^{\prime}\cos\theta}{v_1} = \frac{x}{v_{2u}}+{t^{\prime}_i}   \quad (2)

So measurement of \\(v_{2d}\\) and \\(v_{2u}\\) can be used to obtain values for the critical angle \\(\\theta\\) and the dip \\(\\gamma\\).

.. math::
	\frac{1}{v_{2d}} = \frac{sin(\theta + \gamma)}{v_1} \rightarrow \theta + \gamma = sin^{-1}\Big( \frac{v_1}{v_{2d}}\Big)

.. math::
	\frac{1}{v_{2u}} = \frac{sin(\theta - \gamma)}{v_1} \rightarrow \theta - \gamma = sin^{-1}\Big( \frac{v_1}{v_{2u}}\Big)

There are two equations in two unknowns \\(\\theta\\) and \\(\\gamma\\), therefore we can solve for both unknowns. The result of solving for \\(\\theta\\) and \\(\\gamma\\) is  


.. math::
	\gamma = \frac{1}{2} \bigg[ sin^{-1}\bigg( \frac{v_1}{v_{2d}} \bigg) - sin^{-1}\bigg( \frac{v_1}{v_{2u}}  \bigg)     \bigg]

.. math::
	\theta = \frac{1}{2} \bigg[ sin^{-1}\bigg( \frac{v_1}{v_{2d}} \bigg) + sin^{-1}\bigg( \frac{v_1}{v_{2u}}  \bigg)     \bigg]	

Now, how do we use these relations? Start by recalling what we want: We want depths under each end of the survey line (\\(h\\) and \\(h'\\)) and two true velocities. This is as much as we will obtain from a two-shot (forward and reverse) seismic refraction survey. We have, or can measure, velocities \\(v_1\\), \\(v_{2u}\\)  and \\(v_{2d}\\)  , and two intercept times \\(t_i\\) and \\(t'_i\\). These intercepts \\(t_i\\) and \\(t'_i\\) can be used to calculate \\(z\\) and \\(z'\\) (using (1) and (2) above) because \\(x=0\\) when \\(t_2=t_i\\) or \\(t'_2=t'_i\\) and the angle \\(\\theta\\) can be found using the three velocities obtainable from the T-X plot. Finally, true depths \\(h\\) and \\(h'\\) can be found using these slant depths and the relation we found for dip, \\(\\gamma\\).

What about true refractor velocity, \\(v_2\\)? Snell's law can of course be invoked. The critical angle \\(\\theta\\) (referred to above) is obtained from the relation involving updip and downdip velocities, and the known value of \\(v_1\\). A less accurate version of \\(v_2\\) can be obtained by averaging \\(v_2\\) and \\(v_2\\) but your average value will be wrong by a factor of \\(cos(\\gamma)\\), or 2% to 3% for dips of about 12 degrees. 


.. Notes to consider for review (Phil, 04/10/2014):
.. (1) The final sentence says averaging v2 and v2 (as does GPG). Quantities need clarification. 
.. (2) Grammar/style query: earlier paragraphs use "updip velocity" and latter use "up-dip velocity." Text is modified from GPG to unhyphenated choice for consistency. But in general: hyphen or no hyphen?