.. _seismic_reflection_travel_time_curves_multiple_layers:

Travel Time Curves for Multiple Layers
**************************************

 	

If there are additional layers then the seismic energy at each interface is refracted according to Snell's Law. The energy no longer travels in a straight line and hence the travel times are affected. It is observed that for small offsets, the travel time curve is still approximately hyperbolic, but the velocity, which controls the shape of the curve, is an "average" velocity determined from the velocities of all the layers above the reflector. The velocity is called the RMS (Root Mean Square) velocity, \\(v_{rms}\\).   

.. figure:: ./images/ray_in_multiple_layers.gif
	:align: left
	:scale: 140 %

.. figure:: ./images/t_x_curve_reflected_ray.gif
	:figclass: center
	:align: left
	:scale: 165 %


The complex travel path of a reflected ray through a multilayered ground. (b) The time--distance curve for reflected rays following the above type of path. Note that the divergence from the hyperbolic travel-time curve for a homogeneous overburden of velocity Vrms increases with offset. 

As outlined in the figure above, the reflection curve for small offsets is still like a hyperbola, but the associated velocity is  \\(v_{rms}\\), not a true interval velocity.

.. figure:: ./images/travel_t_hyperbolas.gif
	:align: right
	:scale: 150 %

For each hyperbola:

.. math::
 		  t &\approx \frac{\left(x^2 + 4z_n^2 \right)^2 } {v_n^{rms}} 

By fitting hyperbolas to each reflection event one can obtain  \\(t_n,v_n^{rms}\\) for n = 1, 2, ... The interval velocity and layer thickness of each layer can be found using the formulae below: 

.. math::
 		  v_n \approx \left[ \frac{(v_n^{rms})^2 t_n - (v_{n-1}^{rms})^2 t_{n-1}  }{t_n-t_{n-1}} \right] 


 		  \Delta z = z_n - z_{n-1} = v_n \left( \frac{t_n - t_{n-1}}{2} \right)


These formulae for the interval velocity and thickness of the \\(n^{th}\\) layer are directly obtainable from the definition of \\(v_n^{rms}\\) given above. The RMS velocity for the \\(n^{th}\\) layer is given by:


.. math::
 		  v_n^{rms} = \left( \frac{\sum_{i=1}^{n} v_i^2 \tau_i}{\sum_{i=1}^{n} \tau_i}	 \right)

where \\(v_i\\) is the velocity of the \\( \\) \\(i^{th}\\) layer, and \\(\\tau_i\\) is the one-way travel time through the \\( \\) \\(i^{th}\\) layer. 