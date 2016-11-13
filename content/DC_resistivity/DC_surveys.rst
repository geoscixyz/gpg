.. _DC_surveys:

Surveys
*******

.. sidebar:: DC Resistivity

    .. figure:: ./images/icon_dc.gif
    	:align: center

In resistivity surveying, information about the subsurface distribution of
electrical conductivity is obtained by examining how currents flow in the
earth. DC (direct current) resistivity methods involve injecting a steady
state electrical current into the ground and observing the resulting
distribution of potentials (voltages) at the surface or within boreholes.

Like all geophysical processes, DC surveys can be described in terms of input
energy, the earth's physical properties, and signals or data that are
measured.

.. figure:: ./images/source_receiver.gif
	:align: center
	:scale: 100 %

Using the same colour scheme as the flow diagram above, Figure 2 shows how
this conceptual framework applies for DC methods. The energy source is a pair
of electrodes that inject a known current into the ground at known locations
(Figure 2a). The earth affects this energy because variations in the
electrical conductivity of subsurface structures will bend the current flow
lines (Figure 2b). The measured signals or data (Figure 2c) will involve
measurements of voltage at the earth's surface or within boreholes. This type
of data contains information about how charges become distributed at
boundaries where electrical conductivity changes.

.. figure:: ./images/E_source.gif
	:align: center
	:scale: 100 %

	Figure 2a. The energy source is a controlled DC electrical current injected into the ground.

.. figure:: ./images/E_source2.gif
	:align: center
	:scale: 100 %

	Figure 2b. Increases and decreases in electrical conductivity cause current paths to converge and diverge respectively.

.. figure:: ./images/E_source3.gif
	:align: center
	:scale: 100 %

	Figure 2c. Data are voltages caused by charges accumulating due to current flow.

For each placement of the transmitting electrodes, voltages will be measured
at different locations. Therefore, the complete data set includes measured
voltages with known currents and electrode geometries. In order to create maps
or graphs of raw data for quality assessment, it is usual to convert the data
into a form that has units of resistivity. The data are the input for DC
resistivity inversions, and the results will be 1D, 2D or 3D models of how
subsurface conductivity is distributed.

Practical surveys
=================

If there are two current (source) electrodes, the potential is the
superposition of the effects from both. In a practical experiment (figure
below), one electrode, :math:`A`, is the positive side of a current source, and
the other electrode, :math:`B`, is the negative side. The current into each
electrode is equal, but of opposite sign. For a practical survey, we need two
electrodes to measure a potential difference. These are :math:`M`, the positive
terminal of the voltmeter (the one closest to the :math:`A` current electrode),
and :math:`N`, the negative terminal of the voltmeter.

.. figure:: ./images/practical_experiment.gif
   :align: center
   :scale: 100 %

The measured voltage is a potential difference :math:`(V_M - V_N)` in which each
potential is the superposition of the effects from both current sources:

.. math::
	\Delta V &= V_M - V_N \textrm{, with} \\[0.8em]
	V_M &= \frac{I \rho}{2 \pi} \left \{ \frac{1}{r_{AM}}  -  \frac{1}{r_{BM}} \right \} \textrm{ and}  \\[0.8em]
	V_N &= \frac{I \rho}{2 \pi} \left \{ \frac{1}{r_{AN}}  -  \frac{1}{r_{BN}} \right \} \textrm{, so} \\[0.8em]
	\Delta V &= \frac{I \rho}{2 \pi} \left \{ \frac{1}{r_{AM}} - \frac{1}{r_{BM}} - \frac{1}{r_{AN}} + \frac{1}{r_{BN}}  	 \right \}\\[0.8em]
	\Delta V &=I \rho G

Apparent resistivity
====================

In the final relation, :math:`G` is a geometric factor which depends upon the
geometry of all four electrodes. Finally, we can define apparent resistivity
(discussed in the measurements section) by rearranging the last expression to
give:

.. math::
   \rho_a = \frac{\Delta V}{IG}

Similarly, the apparent conductivity is

.. math::
   \sigma_a = \frac{1}{\rho_a} = \frac{IG}{\Delta V}


We use the term *apparent resistivity* :math:`\rho_{app}` because it is a true resistivity
of materials, only if the Earth is a uniform halfspace within range of the
survey. Otherwise, this number represents some complicated averaging of the
resistivities of all materials encountered by the current field.
	
