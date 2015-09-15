.. _magnetics_extended_bodies:

Fields from extended bodies
***************************

Approximating targets using magnetic charges
============================================

 .. figure:: ./images/buried_bodies1.gif
	:align: right
	:figclass: float-right-360
	:scale: 100% 

If \\(L\\) denotes the scale length of a buried object and the distance from
the observer to the body, \\(R\\) is \\(\\gg\\) \\(L\\), then the magnetic
field of the body will look like that due to a simple dipole. If the buried
object has a complicated structure or the observer is very close to the
magnetized object then it can no longer be represented as a single dipole.  In
:doc:`magnetics_complex_structures`, we will present a general method for
computing the magnetic response from an arbitrary object but here we look at
objects that have a uniform magnetic susceptibility. We introduce the concept
of magnetic charge and show how this can be used to compute the response for
some simple objects like a pipe or sheet.


First we begin with the concept of magnetic charges or poles. They can't be
generated in practise. If you cut a small magnet in half, you will have two
smaller dipole magnets. Let \\(Q\\) be a magnetic charge. It has units of
Webers. The charge creates a magnetic field, \\(B\\) that is given by

 .. math:: 
	\vec{B} =  \frac{ \mu_0 Q \hat r}{4 \pi r^2}


If \\(Q\\) is positive the field lines of \\(\\vec{B}\\) extend radially
outward in all directions as indicated by the drawing. If \\(Q\\) is negative
the field lines have the same shape but they point toward the source.

 .. figure:: ./images/Positive_magnetic_pole.png
	:align: center
	:scale: 110% 

	Figure Caption

 .. figure:: ./images/Negative_magnetic_pole.png
	:align: center
	:scale: 110% 

	Figure Caption


If a positive and negative charge are put in proximity they form a dipole and
the field lines look like the diagram below.

 .. figure:: ./images/Magnetic_dipole.png
	:align: center
	:scale: 110% 


If the distance between the two charges is \\(s\\) then the dipole has a
magnetic moment \\(m=Qs\\) (units: \\(\\text{Amp m}^2\\)). The direction of
the dipole goes from the positive to negative charge. (see diagram). Formulae
for the magnetic field in cylindrical or cartesian coordinates can be found in
standard texts.

------

As an aside we notice that magnetic charges behave exactly as point electric
charges. An important distinction is that electric particles can exist by
themselves whereas magnetic charges always occur in pairs. The reason for this
is that all magnetic fields fundamentally are arise from currents.



Consider a magnetic field impinging upon a body of arbitrary shape and uniform
susceptibility. In the interior of the body, the magnetic elements align
themselves with the inducing field. The sketch below illustrates the process.
Each cell becomes a dipole which can be represented by a plus and minus
magnetic charge. At the interior boundaries, the effects of positive and
negative charges cancel and the net result is that the magnetic field away
from the body is effectively due to the negative magnetic charges on the top
surface and the positive charges on the bottom. This greatly simplifies both
computations and understanding.

.. figure:: ./images/magnetic_charges.gif
	:align: center
	:scale: 100% 

The resultant anomalous magnetic field can be thought of as being due to a
distribution of magnetic poles on the surface of the body. Conceptually, a
picture of the large scale effect can be drawn as shown here:

.. figure:: ./images/magnetic_poles.gif
	:align: center
	:scale: 100% 


Working with magnetic charges
=============================

The magnetization in a body of constant magnetic susceptibility \\(\\kappa\\)
is \\(\\vec{M} = \\kappa \\vec{H_0}\\). As illustrated in the above diagram,
the magnetic field outside the body can be represented as fields due to
charges on the surface of the body. The surface charge density is given by

.. math::
	\tau_s= \vec{M} \cdot \hat n

So the strength of the magnetic charges on the surface depends upon how the
direction of the magnetic field is aligned with the boundary of the object. In
the image above, there are charges on the top and bottom of the prism but
there are no charges on the sides where the magnetic field is parallel to the
boundary.


There are some circumstances in which the concept of magnetic charge greatly
simplifies the problem. Consider a pipe, or vertical prism, and an incident
magnetic field that is pointing down. The magnetization points vertically
downward and \\(\\vec{M} \\cdot \\hat{n}\\) is zero except at the two ends. At
the top the charge density is \\(\\left|M\\right| \\text{W/m}^2\\) and at the
bottom it is \\(-\\left|M\\right| \\text{W/m}^2\\). Suppose the pipe has a
radius \\(a\\) and thus an area \\(\\pi a^2\\). If the radius of the pipe is
small compared to the distance from the observer then the effect is the same
as if all of the charge was sitting at the top of the pipe at its center. The
total charge on the face is the area (units \\(\\text{m}^2\\)) times the
charge density \\(\\text{W/m}^2\\).

.. math::
	Q = \kappa H_0 \pi a^2

and the magnetic fields are like those given in equation XXX and diagram XXX.

The same phenomenon is happening at the bottom of the pipe but there the
charge is \\(-Q\\). At the surface the magnetic field is the sum of fields due
to the two charges, but if the pipe is very long, then the contribution from
the bottom of the pipe becomes negligible. The resultant observed field is
effectively that due to a monopole, or point charge, of strength \\(Q\\).
This handy simplification often arises in practise.

The equation xxx provides the anomalous magnetic field due to a charge of
strength \\(Q\\). This is a vector. When we measure the magnetic anomaly we
measure one or more individual components of this field. The total field
anomaly is the projection of the anomalous field onto the direction of the
earth's field \\(\\hat{z}\\) so the magnetic field anomaly over the pipe is

.. math::
	B_t= \frac{\mu_0}{4 \pi} \frac{Q z}{r^3}

where \\(z\\) is the depth of burial. Equivalently, if we substitute for the
magnetic charge and write the expression using the earth's magnetic field
\\(B_0\\) then

.. math::
	B_t = \frac{\kappa \pi a^2 B_0}{4 \pi} \frac{z}{r^3} 	


Geologic Features and representation for modeling 
=================================================

Some simplified geologic features that can be detected (and sometimes
characterized) using magnetic data are shown below. They represent models of
the true Earth, which provide useful first order understanding about
structures and rock type distributions, in spite of being simplifications of
the real earth.

.. figure:: ./images/geomods.gif
	:align: center
	:scale: 100% 

For each model, the concept of surface magnetic charges then permits
evaluation of the fields; here are examples.

.. figure:: ./images/modrep.gif
	:align: center
	:scale: 100% 

As seen in the figures, for these types of features the responses can
represented as monopoles, dipoles, lines of dipoles, sheets of charges etc.
This can help us understand what the magnetic response of such objects are.
For instance a buried cylinder or rebar can be thought of as a line of
dipoles. Sometimes field data are interpreted using these simple
approximations. There are numerous parametric inversion algorithms that have
been generated to accomplish this.

Some images on this page adapted from "Applications manual for portable
magnetometers" by S. Breiner, 1999, Geometrics 2190 Fortune Drive San Jose,
California 95131 U.S.A.
