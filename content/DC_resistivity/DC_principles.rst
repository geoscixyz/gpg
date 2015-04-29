.. _DC_principles:

Physical principles of DC resistivity
*************************************

Introduction
============

This chapter presents the important physical principles upon which DC resistivity methods are based. The relations between current flow, potentials and resistivity in uniform ground are explained. This forms the basis for the concept of apparent resistivity derived from practical survey arrangements (two current and two potential electrodes planted at the surface). The effect of anisotropic ground upon measured potentials is then described. Finally, charge distribution is explained because it is a useful way of understanding how potentials arise at the surface due to variations in electrical conductivity underground. The forward modeling relations are also based upon charge distribution.

Currents and voltages in a uniform earth
========================================

In order to derive a relation between measurements (\\(I\\), \\(V\\) and geometry) and the required physical property (resistivity or  \\(\\rho\\) ), we must start by identifying how these parameters relate to electric field strength, \\(E\\) (Volts per meter), current density, \\(J\\) (Amps per unit area), and resistivity  (Ohm-m) in the three dimensional situation of a field survey (the introduction defines resistivity and conductivity).

.. figure:: ./images/currents_in_earth.gif
	:align: right
	:scale: 100 %

Consider first a uniform Earth and one electrode, which is pumping a current, \\(I\\), into the ground. We want to find the electric potential within the ground at a distance, \\(r\\), from the current source. The current density in the ground is related to source current injected, and it flows radially outward from its point source. The potential measured at a surface defined by \\(r\\) is related to the electric field that exists in the ground because of the current. These two relations will be combined with the 3D form of Ohm's law to end up with an expression for conductivity (the physical property we want) in terms of the current source, measured potential, and the distance.

First, by symmetry the current density out of the hemisphere of radius, \\(r\\), is

.. math::
		J = \frac{I}{2 \pi r^2} 	\qquad (1)

and the current is flowing in a radial direction. Since \\(J= \\sigma E\\) (Ohm's Law), the electric field must also be pointing radially outward. The relationship between the electric field and the potential is

.. math::
		E = -\frac{dV(r)}{dr}

Combining the expression for \\(E\\), Ohm's Law and equation 1, we have

.. math::
		J = -\sigma \frac{dV(r)}{dr} &= \frac{I}{2 \pi r^2}

		\frac{dV(r)}{dr} &= \frac{-I}{2\pi \sigma r^2}

If we integrate,

.. math::
		V(r) = \frac{I}{2 \pi \sigma r} + C

chose

.. math::
		V(\infty) \longrightarrow C = 0

So the potential due to a point current electrode at the surface is:

.. math::
		V(r) = \frac{I}{2 \pi \sigma r}

The electric potential inside the earth caused by the radial flow of current is illustrated in the diagram below.


.. figure:: ./images/radial_flow.gif
	:align: center
	:scale: 100 

.. figure:: ./images/pot_decay.gif
	:align: right
	:scale: 100 

At the surface, where measurements are made, the potential is infinite at the current electrode because \\(r=0\\), and it decays with distance.


.. math::
	V(r) = \frac{I}{2 \pi \sigma r} = \frac {I \rho} 
	{2 \pi r}




Two electrode current sources
=============================

.. figure:: ./images/two_electrodes.gif
	:align: right
	:scale: 100 

In a geophysical survey, current is injected into the ground using two electrodes. It is convenient to label the electrodes as

A. positive current electrode (carries a current \\(+I\\))		
B. negative current electrode (carries a current \\(-I\\))

.. figure:: ./images/fieldlines.gif
	:align: right
	:scale: 100 

For a uniform Earth, lines of current flow are shown in red in the figure to the right, and corresponding lines of equal potential (equipotential lines) are shown in black. Instead of the current flowing radially out from the current electrodes, it now flows along curved paths connecting the two current electrodes. Six current paths are shown. Between the surface of the earth and any current path we can compute the total proportion of current encompassed. The table below shows the proportion for the six paths shown (current path 1 is the top-most path and 6 is the bottom-most path).

+-----------------------+-----------------------+
|  **Current Path**     | **% of Total Current**|
+=======================+=======================+
|   1                   |    17                 | 
+-----------------------+-----------------------+
|   2                   |    32                 | 
+-----------------------+-----------------------+
|   3                   |    43                 | 
+-----------------------+-----------------------+
|   4                   |    49                 | 
+-----------------------+-----------------------+
|   5                   |    51                 | 
+-----------------------+-----------------------+
|   6                   |    57                 | 
+-----------------------+-----------------------+

From these calculations and the graph of the current flow shown above, notice that almost 50% of the current placed into the ground flows through rock at depths shallower than or equal to the current electrode spacing.

The graph shown below plots the potential that would be measured along the surface of the earth for a fixed 2-electrode source. The voltage we would observe with our voltmeter (between purple electrodes) is the **difference** in potential at the two voltage electrodes, \\(\\Delta V\\).

.. figure:: ./images/pot_difference.gif
	:align: center
	:scale: 100 

Practical surveys
=================

If there are two current (source) electrodes, the potential is the superposition of the effects from both. In a practical experiment (figure below), one electrode, \\(A\\), is the positive side of a current source, and the other electrode, \\(B\\), is the negative side. The current into each electrode is equal, but of opposite sign. For a practical survey, we need two electrodes to measure a potential difference. These are \\(M\\), the positive terminal of the voltmeter (the one closest to the \\(A\\) current electrode), and \\(N\\), the negative terminal of the voltmeter.

.. figure:: ./images/practical_experiemnt.gif
	:align: center
	:scale: 100 

The measured voltage is a potential difference \\((V_M - V_N)\\) in which each potential is the superposition of the effects from both current sources:

.. math::
	\Delta V &= V_M - V_N \textrm{, with} \\[0.8em]
	V_M &= \frac{I \rho}{2 \pi} \left \{ \frac{1}{r_{AM}}  -  \frac{1}{r_{BM}} \right \} \textrm{ and}  \\[0.8em]
	V_N &= \frac{I \rho}{2 \pi} \left \{ \frac{1}{r_{AN}}  -  \frac{1}{r_{BN}} \right \} \textrm{, so} \\[0.8em]
	\Delta V &= \frac{I \rho}{2 \pi} \left \{ \frac{1}{r_{AM}} - \frac{1}{r_{BM}} - \frac{1}{r_{AN}} + \frac{1}{r_{BN}}  	 \right \}\\[0.8em]
	\Delta V &=I \rho G

Apparent resistivity
====================

In the final relation, \\(G\\) is a geometric factor which depends upon the geometry of all four electrodes. Finally, we can define apparent resistivity (discussed in the measurements section) by rearranging the last expression to give:

.. math::
		\rho_a = \frac{\Delta V}{IG}

Similarly, the apparent conductivity is

.. math::
		\sigma_a = \frac{1}{\rho_a} = \frac{IG}{\Delta V}


We use the term *apparent resistivity* \\(\\) because it is a true resistivity of materials, only if the Earth is a uniform halfspace within range of the survey. Otherwise, this number represents some complicated averaging of the resistivities of all materials encountered by the current field.

Anisotropic ground
==================

Structural anisotropy (for example, layering or fracturing) causes the simple form of Ohm's law to break down because current flow is not necessarily parallel to the forcing electric field. Instead of simply writing \\(J = \\sigma E = - \\sigma \\Delta V \\), we have to write

.. math::
		J_i = -\sigma_{ik} \frac{\partial V}{\partial  x_k} \quad i,k = 1,2,3


In homogeneous ground with a single current and potential electrodes, the expression for \\(V\\) (voltage) in terms of resistivity and distance from the current source is \\(V=-I \\rho / 2 \\pi r \\) (which was shown above). In anisotropic ground, there are different values of resistivity for the horizontal and a vertical directions. The expression for voltage in terms of the two resistivities and distance is

.. math::
		V=-I \frac{\sqrt{\rho_h \rho_v}}{2 \pi r} = - \frac{I \rho_h \lambda}{2 \pi r}

where \\(\\lambda = (\\rho_i / \\rho_h)^{1/2}\\) is called the coefficient of anisotropy. See the table below for some values of \\(\\lambda\\) encountered in common geological materials.

.. figure:: ./images/layers.gif
	:align: left
	:scale: 100 %

.. figure:: ./images/table13.gif
	:figclass: center
	:align: left
	:scale: 100 %


Charge distribution
===================


.. figure:: ./images/sig1_sig0.gif
	:align: right
	:scale: 100 %

One of the fundamental principles regarding current flow is that away from the current electrode, all the current that goes into a body must come out. There are no sources or sinks of current anywhere, except at the current electrode itself.

Because there are no sources or sinks of current in the earth (conservation of charge), the normal component of current density is constant across any boundary where conductivity changes. That is, all of the current that flows into one side of the boundary must flow out the other side. Also, since lines of equal potential in an electric field are perpendicular to current flow, the electric field perpendicular to the normal component of current at the boundaries must also be constant across the boundary. Therefore there are two boundary conditions that must hold across interfaces where conductivity changes:

	- the *normal* \\( \\)component of current density, \\(J\\), must be continuous, and
	- *tangential* \\( \\)components of electric field, \\(E\\), must be continuous.

Recall that Ohm's law is \\(J = \\sigma E\\). Since the normal component of \\(J\\) is continuous across a boundary where conductivity changes, the normal component of the \\(E\\)-field must NOT be equal. If \\(\\sigma_2 > \\sigma_1\\) then \\(E_2 < E_1 \\). The following figure should clarify:


.. figure:: ./images/sigma_E_relation.gif
	:align: center
	:scale: 120 %

The only way an electric field can change at a boundary is if there is a charge on the boundary. If the current is flowing from a resistive medium to a conductive medium, then the charge buildup will be negative. If the current flows from a conductive medium to a resistive medium, then the charge will be positive. This is illustrated in the diagram below-left, where the anomalous body (blue) is more conductive than the host (yellow). In the figure below-right, the change in \\(E\\)-field is illustrated for a field crossing from a resistive medium (yellow) into a more conductive zone (blue). Tangential components are unchanged, but normal components of \\(E\\) are different so that normal components of \\(J\\) can remain unchanged. This change in direction is the origin of the concept that current lines "converge" upon entering a conductor, and "diverge" upon entering a resistor (illustrated with cartoons of the ore body in :doc:`DC_resistivity_surveys`).


.. figure:: ./images/conductive_body.gif
	:align: left
	:scale: 135 %

.. figure:: ./images/E_field.gif
	:figclass: center
	:align: left
	:scale: 120 %


In fact, the charge density that accumulates will be related to the ratio of the two conductivities:


.. figure:: ./images/conductivity_ratio.gif
	:align: center
	:scale: 100 %

.. figure:: ./images/Q_r_vector.gif
	:align: right
	:scale: 100 %

How are charges on boundaries related to DC resistivity surveying? Any electric charge produces an electric potential. The Coulomb electrostatic potential is given by

.. math::
		V(r) = \frac{1}{4 \pi \epsilon_0} \frac{Q}{r}

All charge on the edges of a body produce their own electric potentials, and at the surface (or anywhere else), the total potential is the sum of the potentials due to the individual charges (principal of superposition). These potentials are what we measure as voltages, and they are caused by charges building up on boundaries where conductivity changes, which in turn are caused by the current being forced to flow by the transmitter. Of course we don't measure absolute potential; rather, we measure the potential difference between two locations (say \\(r_1\\) and \\(r_2\\)).

.. figure:: ./images/potential_difference.gif
	:align: center
	:scale: 100 %

Equations for calculating DC measurements
=========================================

.. figure:: ./images/principles_dcresf1.gif
	:align: right
	:scale: 100 %

Using the physics and appropriate mathematics to calculate a set of measurements is called "forward modeling." The DC resistivity forward modeling problem involves describing potentials everywhere as a function of conductivity in the ground, geometry, and input current. It requires three fundamental relations:


.. math::
	&(a) \quad \textbf{J} = \sigma \textbf{E} \quad &&\textrm{Ohm's Law}  \\[0.4em]
	&(b) \quad \textbf{E} = \nabla V \quad  &&\textrm{The electric field is the gradient of a scalar potential.}  \\[0.4em]
	&(c) \quad \nabla \cdot\ \textbf{J} = - \partial{Q} / \partial{t} \quad &&\textrm{The divergence of current density equals the rate of change of free charge density.}

We want to obtain a differential equation and boundary conditions to define the forward problem that will allow us to relate conductivity everywhere to potential everywhere. Start by combining (a) and (b) to say \\(\\textbf{J} = \\sigma \\nabla V \\), then plug this into (c) to get

.. math:: 
		\nabla \cdot\ (\sigma \nabla V) = - \partial{Q} / \partial{t} \quad (2)

This holds for steady state conditions everywhere, except at the source position \\(r = r_s\\), where it equals the input current, \\(I\\). In other words, charge does not accumulate under steady state conditions, except at the point of the source.

Equation (2) can be re-written as

.. math:: 
	\nabla \cdot\ (\sigma \nabla V) = -I \delta (r-r_s) \quad (3)

The Dirac delta function is used here to indicate that charge density is varying only at the point source of current.

**Boundary conditions** that must hold are:
	1. The change of potential across the free surface is zero (\\(\\partial{V}/\\partial{n} = 0\\) at \\(z=0\\)), and
	2. \\(V\\) approaches 0 as \\(r - r_s\\) approaches infinity.

This differential equation (3) and the two boundary conditions define the forward problem that relates conductivity everywhere in the ground to potential measured anywhere within or on the surface of the ground. This problem can be solved numerically using finite element or finite volume techniques. 

References
----------

**Dey , A. and H.F. Morrison**, 1979a, *Resistivity modelling for arbitrarily shaped two-dimensional structures*, Geophysical Prospecting, 27, 106-136.

**Dey, A. and H.F. Morrison, 1979b**, *Resistivity modeling for arbitrarily shaped three-dimensional structures*, Geophysics, 44, no. 4, 753-780.

**McGillevry, P.R.**, 1992, *Forward modelling and inversion of DC resistivity and MMR data*, unpublished PhD. thesis, UBC.