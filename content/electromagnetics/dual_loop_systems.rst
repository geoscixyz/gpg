.. _dual_loop_systems:

Dual Loop Systems
*****************

EM-31
=====

Loop-loop system mounted on a 4 meter boom. The transmitting coil operates at
a frequency of 9.8 kHz and the receiving coil is located 3.66 meters from the
transmitter. The instrument measures both the in-phase and quadrature fields.
The in-phase component is diagnostic of high conductivity bodies (metal pipes,
drums, etc.) and the quadrature component can be converted into an apparent
conductivity which is read out in mS/m. Such readings arc valid only if the
ground is laterally uniform on a scale length equal to the source-receiver
separation and that \\(s << \\delta\\). The instrument and coils can be
rotated by 90° so that loops are vertical. This provides data estimating the
conductivities and thickness. The effective depth of exploration is about 6
meters for the vertical dipole mode and about 3 meters for the horizontal
dipole mode. Data can be acquired with the device held at hip level or it can
be put on the ground.

EM-34
=====

This uses two vertical or horizontal coplanar coils that are not attached to
each other. The coils and analysis system are designed so that different coil
separations operate at different frequencies:

1. 10 meters at 6.4 kHz
2. 20 meters at 1.6 kHz
3. 40 meters at 0.4 kHz

This allows greater penetration into the ground and hence is used to delineate
vertical geologic anomalies and for groundwater exploration in fractured,
faulted and weathered bedrock zones.


Depth of Investigation
======================

A maximum depth of investigation is provided by the skin depth rule, however
for controlled source surveys we also need to take into account the source and
receiver geometry. This generally reduces the depth of penetration. A rule of
thumb for loop-loop systems is that the depth of penetration is about twice
the separation of the source and receiver, but this is very approximate and is
easily violated. Also, a necessary condition for this to happen is that the
source/receiver separation \\(s << \\delta\\) (coil separation is less than
the skin depth).

Relative Response Function
==========================

The justification for the above statement is based upon the following.
Consider a homogeneous halfspace on the surface of which is located a
horizontal coplanar coil (HCP) system (e.g. EM31) or a vertical coplanar (VCP)
system (EM34). Let the depth \\(z\\) in the earth be normalized by the coil
spacing \\(s\\). (True depth in meters is \\(zs\\).) The time varying fields
in the transmitting coils will induce eddy currents in the earth. For a
homogeneous earth, these currents flow in horizontal planes. This is true even
for the vertically oriented coils. It is possible to calculate the
contribution to the secondary field as measured from the surface from any thin
layer of thickness \\(dz\\) at some depth \\(z\\). Let \\(\\phi_V(z)\\) denote
this contribution from the vertical magnetic dipole source and receiver. The
subscript \\(V\\) denotes that the magnetic fields are vertical. A horizontal
loop of current acts like a vertical magnetic dipole. A plot of this function
is shown below:

.. figure:: ./images/vertical_dipole_response.jpg
    :align: center
    :scale: 100 %

    Relative response versus depth for vertical dipoles. \\(\\phi_V(z)\\) is the relative contribution to \\(H_s\\). from material in a thin layer dz located at (normalized) depth \\(z\\).

Note that the vertical magnetic dipole has zero sensitivity at the surface,
has a maximum at about \\(z = 0.4\\) and is substantially diminished by \\(z =
2.0\\). It is this type of diagram which says that the maximum depth of
investigation is limited to about twice the coil separation. This rule of
thumb however is valid only when the coil separation is much less than the
skin depth.

The response function from the horizontal magnetic is very different. Let
\\(\\phi_H (z)\\) denote the relative contribution that arises from a
horizontal magnetic dipole source and receiver. It has a maximum at the
surface, so it is sensitive to the conductivity there, and it decreases
monotonically with depth.

 .. figure:: ./images/horizontal_dipole_response.jpg
    :align: center
    :scale: 100 %

We therefore notice how two coil configurations couple differently with the
ground and have different sensitivities with respect to the conductivity
structure.

Cumulative Response Functions
=============================

We often have a multi-layer earth (e.g. a thin resistive layer overlying a
more conductive stratum, or vice versa) and we would like to estimate the
thickness of the layer and the two conductivities. Cumulative response curves
are useful for carrying out computations. Define
 
.. math::
        R_V (z) &= \int_{z}^{\infty} \phi_V (z) dz \\[0.8em]
        R_H (z) &= \int_{z}^{\infty} \phi_H (z) dz

to be the relative contribution to the secondary magnetic field obtained from
all of the material below a depth \\(z\\). The diagrams are plotted below:

 .. figure:: ./images/cumulative_response.jpg
    :align: center
    :scale: 100 %

A depth of investigation might be defined as that depth below which only 25%
of the signal arises. According to this rule the depth of investigation for
the vertical dipole is about 2.0 s while the depth for the horizontal dipole
is only half that amount.



