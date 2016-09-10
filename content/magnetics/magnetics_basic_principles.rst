.. _magnetics_basic_principles:

Basic Principles
****************

This section provides the key components to understand the geophysical magnetic experiment. As briefly summarized in the :ref:`Introduction<magnetic_physical_property>` section, the magnetic survey requires a magnetic :ref:`source<earth_s_field>` interacting with the sub-surface creating a :ref:`magnetic response<magnetic_response>`, giving rise to measurable :ref:`anomalous magnetic field<anomalous_field>` data.  temporary corrct

.. figure:: ./images/Intro_Response.png
    :align: center
    :figwidth: 50 %
    :name: mag_response


.. _earth_s_field:

Earth's magnetic field (Source)
===============================

 .. figure:: ./images/earthfield.gif
  :align: right
  :figwidth: 40%
  :name: earth_mag_vectors

  : Earth's magnetic field orientation


Most people are familiar with the magnetic field that exists around a bar
magnet. To a first approximation, Earth's magnetic field does resemble a large
dipolar source with a negative pole in the northern hemisphere and a positive
pole in the southern hemisphere (:numref:`earth_mag_vectors`). The source of
this magnetic field is thought to originate deep within the mantle due to
convection.

The field at any location on (or above or within) the Earth are generally described in terms described of magnitude (H), declination (D) and inclination (I) as illustrated in :numref:`coord_sys`.

.. figure:: ./images/Mag_Coordinate_System.png
  :align: right
  :figwidth: 40%
  :name: coord_sys

  : Sketch of coordinates used to describe magnetic fields.

* **H**: The magnitude of the vector representing Earth's magnetic field strength.
* **D**: Declination is the angle that *H* makes with respect to geographic north (positive angle clockwise).
* **I**: Inclination is the angle between **B** and the horizontal. It can vary between -90° and +90° (positive angle down).

.. _magnetics_IGRF:

The IGRF
--------

The details of Earth's field at any location on Earth are described using a
global reference model called the :ref:`IGRF<magnetics_IGRF>` or International
Geomagnetic Reference Field. The IGRF is a mathematical model that describes
the field and its secular changes as a spherical harmonic expansion. It is
updated every five years, and **later** versions may re-define the field at
**earlier** times. This is important to remember if you are comparing old maps
to new ones.  This field has a strength of approximately 70,000 nanoTeslas
(nT) at the magnetic poles and approximately 25,000 nT at the magnetic
equator. Field orientation and strength varies around the world, as presented
in :numref:`IGRF_three_figures` based upon the IGRF from 2003 (NOAA_). The
IGRF is a product of the International Association of Geomagnetism and
Aeronomy (IAGA_), and the original version was defined in 1968.

.. _IAGA: http://www.ngdc.noaa.gov/IAGA/vmod/

.. _magnetics_three_figures:

.. list-table::
   :header-rows: 0
   :widths: 10 10
   :stub-columns: 0
   :name: IGRF_three_figures

   *  - .. figure:: ./images/earth-decl.gif


          Earth's declination.
      - .. figure:: ./images/earth-incl.gif

          Earth's inclination.

   *  - .. figure:: ./images/earth-strength.gif

          Earth's field strentgh
      -


Details about Earth's field
can be found at government geoscience websites such as the `NOAA`_ geomagnetism home page, or the `Canadian National Geomagnetism Program`_ home
page.

.. _NOAA: http://www.ngdc.noaa.gov/geomag/geomag.shtml
.. _Canadian National Geomagnetism Program: http://www.geomag.nrcan.gc.ca/index-eng.php
.. _magnetic field calculator: http://www.ngdc.noaa.gov/geomag-web/
.. _page: http://www.ngdc.noaa.gov/ngdc.html
.. _homepage: http://www.geomag.nrcan.gc.ca/index-eng.php



Noteworthy
----------

Slow changes in the exact location of the magnetic north pole occur over long
periods (months-years). These changes are thought to be caused by internal
changes in mantle convection. Knowing the acquisition date of a magnetic
survey is important in order to understand the observed magnetic anomalies. In
2004, Earth's magnetic north pole was close to Melville Island (Nunavut) at
(Latitude, Longitude)=(79N, 70W). In Vancouver (BC), the current field is
orientated at D ~ 20°N,  ~ 70° Inclination. Various governmental agencies are
actively collecting and archiving information about the parameters of the
field worldwide and can be queried with the `magnetic field calculator`_.


Magnetic Weather
----------------

The second component of Earth's field involves external contributions due
primarily to currents in the ionized upper atmosphere. These changes vary over much shorter periods (hours-day) and are due to two major phenomenon:

 .. figure:: ./images/solar_wind.jpg
  :align: right
  :figwidth: 50%

* Daily variations (on the order of 20 - 50 nT in size) are due to solar wind
  action on the ionosphere and magnetosphere. The image shows an artist's
  rendition of the charged particles interacting with Earth's magnetic field.
  An overview of Earth's magnetic field (with good images, graphs, etc.) can
  be found on the British Geological Survey's `geomagnetics website`_.

.. _geomagnetics website: http://www.geomag.bgs.ac.uk/


* Magnetic storms are correlated with sunspot activity, usually on an 11-year
  cycle. These variations can be large enough to cause damage to satellites
  and north-south oriented power distribution systems. They are also the cause
  of the Aurora Borealis or Australis (northern or southern lights
  respectively). See the GSC's "Geomagnetic Hazards" web page for more.


.. _magnetic_response:

Magnetization (Response)
========================

Having identified the source of the magnetic experiment, we now look at the
response from magnetic material. The straight of the anomalous field originating from the magnetized object depends on its shape, location and magnetization such that:

.. math:: \mathbf{B}_A = \frac{\mu_0}{4\pi}  \int_{V}   \mathbf{M} \cdot \nabla \nabla \left(\frac{1}{r}\right) \; dV
  :label: integral

where :math:`\mu_0` is the :ref:`magnetic
permeability<physprop_mag_permeability>`, :math:`\mathbf{M}` is the
magnetization per unit volume :math:`\mathbf{V}`, and :math:`r` defines the
distance between the object and the location of the observer. The magnetic
field of the object is referred to as the "secondary" field or sometimes the
"anomalous" field :math:`\mathbf{B}_A`. For geological or engineering
problems, these anomalous fields are the *data* to be interpreted, and this is
what we seek to measure. Unfortunately, the measured field data are a bit more
complicated:

.. math:: \mathbf{B}^{obs} = \mathbf{B}_0 + \mathbf{B}_A\;,

where :math:`\mathbf{B}^{obs}` is the combined signal from the Earth's field :math:`\mathbf{B}_0` and from the ground :math:`\mathbf{B}_A`. Exactly how the anomalous field is extracted from the total field is explained in the :ref:`Data<magnetics_data>` section.

.. _magnetics_induced:

Induced Magnetization
---------------------

An object with magnetic susceptibility :math:`\kappa` is buried in the
earth. At the location of burial, the earth's magnetic field is
:math:`\mathbf{H}` and the magnetization in the object is:

.. math:: \mathbf{M} = \kappa \mathbf{H}.

The magnetic response then simplifies to:

.. math:: \mathbf{B}_A = \frac{\mu_0}{4\pi}  \int_{V}   \kappa \mathbf{H}_0 \cdot \nabla \nabla \left(\frac{1}{r}\right) \; dV
  :label: integral_induced

The basic ideas behind the induced magnetization process is illustrated below.

 .. raw:: html
    :file: buried_dipole.html

From :eq:`integral_induced`, we note that the induced response of the field will vary both in magnitude and orientation with respect to the inducing magnetic field :math:`\mathbf{H}_0`. Therefore, the magnetic response of an object buried in Canada may look a lot different if buried near the equator as demonstrated in the :ref:`dipole animation<magnetics_induced_demo>` below. This is an important point to keep in mind when interpreting magnetic data.

.. .. figure:: ./images/magnetics_induced_demo.png
..   :align: center
..   :figwidth: 100%
..   :name: magnetics_induced_demo

..   : This example was generated with the :ref:`magnetic applet'<magnetics_applet>`

.. the :ref:`dipole animation<magnetics_induced_demo>`
.. _magnetics_induced_demo:

 .. list-table:: : Changing magnetic response (:math:`B_z`) of a buried magnetic prism as a function of inducing field orientation.
   :header-rows: 0
   :widths: 10
   :stub-columns: 0

   *  - .. raw:: html
            :file: ./images/induced_prism_demo.html



.. _magnetics_remanent:

Remanent Magnetization
----------------------

From :eq:`integral`, the magnetic response is function of position and magnetization per unit volume :math:`\mathbf{M}`. While in most cases the magnetization is assumed to be parallel to the inducing field direction, in some cases this doesn't hold true. The full magnetization vector should be written instead as:

.. math:: \mathbf{M} = \kappa(\mathbf{H_0} + \mathbf{H_s}) + \mathbf{M_{rem}}

where :math:`\mathbf{H_s}` are secondary fields from neighbouring magnetized objects and :math:`\mathbf{M_{rem}}` is known as the remanent component. A good example of remanently magnetized objects are bar magnets. While the outside surface of a refrigerator is susceptible, the permanent dipole moment of the magnet is used generate a strong local field, which can hold your family pictures up!

Similar to the previous animation, we added a remanent component oriented east (x-axis) as presented in the :ref:`dipole animation<magnetics_remanent_demo>` below. Note that the remanent component is independent of the inducing direction, substantially distorting the magnetic data from the purely induced response. Interpreting magnetic data affected by remanence remains a key challenge in exploration geophysics.

.. .. figure:: ./images/magnetics_remanent_demo.png
..   :align: center
..   :figwidth: 100%
..   :name: magnetics_remanent_demo

..   : This example was generated with the :ref:`magnetic applet'<magnetics_applet>`



.. _magnetics_remanent_demo:

 .. list-table:: : Changing magnetic response (:math:`B_z`) of a buried magnetic prism as a function of inducing field orientation with an added remanent component oriented along the x-axis (:math:`I:0^\circ,\; D:90^\circ`).
   :header-rows: 0
   :widths: 10
   :stub-columns: 0

   *  - .. raw:: html
            :file: ./images/remanent_prism_demo.html


.. _anomalous_field:

Anomalous field (Data)
======================

The anomalous magnetic field introduced in :eq:`integral` is a vector quantity:

.. math:: \mathbf{B}_A = [B_x \hat x, B_y \hat y, B_z \hat z ]

usually given in Cartesian coordinates. As it is covered in the :ref:`Data<magnetics_data>` section, instruments more often measure the magnitude of the field, or Total Magnetic Intensity (TMI) data.

.. math:: \mathbf{B}^{TMI} = | \mathbf{B}_T + \mathbf{B}_A |


Note about :math:`\mathbf{B}` and :math:`\mathbf{H}`
----------------------------------------------------

We often use both :math:`\mathbf{B}` and :math:`\mathbf{H}` interchangeably to describe the magnetic field. To be accurate, :math:`\mathbf{B}` should be referred to as the *magnetic flux density*, although in air, both quantities are proportional to each other (:ref:`read more<physprop_mag_permeability>`).


Approximating the response
==========================

Solving the integral in :eq:`integral` can be challenging for objects with complicated geometry, as we expected it to be when thinking of geological structures. In many cases however the magnetic response of objects can be approximated by a summation of dipole and monopoles.

.. _fields_magnetic_dipole:

Fields due to a magnetic dipole
-------------------------------

Understanding the magnetic fields of a buried dipole, and the resultant
observations, is crucial because all real scenarios can be thought of as a
combination (superposition) of dipoles (see the "Buried structures" section).

If the object is "small", that is all of the object's dimensions are several times smaller than the depth to its center, then  the object acts as a :ref:`magnetic dipole<fields_magnetic_dipole>` -- that is, a little bar magnet with strength and direction caused by the inducing field.

In addition the vertical gradient of the field, obtained if measurements were
acquired with a gradiometer, are listed as :math:`B_g`.  Sign conventions must
be adopted when data are plotted. For magnetic surveying the coordinate system
used is: {:math:`x` is northing, :math:`y` is easting, and :math:`z` is downward}.
The sign convention will be that horizontal fields are positive if they point
in the :math:`\hat{x}` direction for :math:`B_x`, in the :math:`\hat{y}` direction
for :math:`B_y` and vertical fields are positive if they point downward. For
:math:`B_t` the anomaly is positive if it points in the same direction as the
earth's field and negative if it is the opposite direction.


.. _magnetics_extended_bodies:

.. Fields from extended bodies
.. ===========================

Approximating targets using magnetic charges
--------------------------------------------

.. add depth of burial of pipe
.. screenshot of buried pipe (pole anomaly)

.. add remament


 .. figure:: ./images/buried_bodies1.gif
	:align: right
	:figclass: float-right-360
	:scale: 100%

If the buried
object has a complicated structure or the observer is very close to the
magnetized object then it can no longer be represented as a single dipole.  In
:ref:`magnetics_complex_structures<magnetics_complex_structures>`, we will present a general method for
computing the magnetic response from an arbitrary object but here we look at
objects that have a uniform magnetic susceptibility. We introduce the concept
of magnetic charge and show how this can be used to compute the response for
some simple objects like a pipe or sheet.


First we begin with the concept of magnetic charges or poles. They can't be
generated in practice. If you cut a small magnet in half, you will have two
smaller dipole magnets. Let :math:`Q` be a magnetic charge. It has units of
Webers. The charge creates a magnetic field, :math:`B` that is given by

 .. math::
	\vec{B} =  \frac{ \mu_0 Q \hat r}{4 \pi r^2}
	:label: B_from_Q


If :math:`Q` is positive the field lines of :math:`\vec{B}` extend radially
outward in all directions as indicated by the drawing. If :math:`Q` is negative
the field lines have the same shape but they point toward the source.

 .. figure:: ./images/Positive_magnetic_pole.png
	:align: center
	:scale: 75%
	:name: Positive_magnetic_pole

	Magnetic field lines generated by a positive magnetic pole.


 .. figure:: ./images/Negative_magnetic_pole.png
	:align: center
	:scale: 75%
	:name: Negative_magnetic_pole

	Magnetic field lines generated by a negative magnetic pole.


If a positive and negative charge are put in proximity they form a dipole and
the field lines look like the diagram below.

 .. figure:: ./images/Magnetic_dipole.png
	:align: center
	:scale: 75%
	:name: Magnetic_dipole

	Magnetic field lines generated by a postive and negative pole which form a dipole.


If the distance between the two charges is :math:`s` then the dipole has a
magnetic moment :math:`m=Qs` (units: :math:`\text{Amp m}^2`). As seen in the above
figure the magnetic field inside of the body points from the positive pole to the
negative pole. The dipole moment on the other hand extends from the negative(south)
pole to the positive(north) pole. Formulae for the magnetic field in cylindrical
or cartesian coordinates can be found in standard texts.

------

As an aside we notice that magnetic charges behave exactly as point electric
charges. An important distinction is that electric particles can exist by
themselves whereas magnetic charges always occur in pairs. The reason for this
is that all magnetic fields fundamentally arise from currents.


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
-----------------------------

The magnetization in a body of constant magnetic susceptibility :math:`\kappa`
is :math:`\vec{M} = \kappa \vec{H_0}`. As illustrated in the above diagram,
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
downward and :math:`\vec{M} \cdot \hat{n}` is zero except at the two ends. At
the top the charge density is :math:`\left|M\right| \text{W/m}^2` and at the
bottom it is :math:`-\left|M\right| \text{W/m}^2`. Suppose the pipe has a
radius :math:`a` and thus an area :math:`\pi a^2`. If the radius of the pipe is
small compared to the distance from the observer then the effect is the same
as if all of the charge was sitting at the top of the pipe at its center. The
total charge on the face is the area (units :math:`\text{m}^2`) times the
charge density :math:`\text{W/m}^2`.

.. math::
	Q = \kappa H_0 \pi a^2

and the magnetic fields are like those given in equation :eq:`B_from_Q` and
shown in :numref:`Positive_magnetic_pole`.

The same phenomenon is happening at the bottom of the pipe but there the
charge is :math:`-Q`. At the surface the magnetic field is the sum of fields due
to the two charges, but if the pipe is very long, then the contribution from
the bottom of the pipe becomes negligible. The resultant observed field is
effectively that due to a monopole, or point charge, of strength :math:`Q`.
This handy simplification often arises in practise.

The equation :eq:`B_from_Q` provides the anomalous magnetic field due to a charge of
strength :math:`Q`. This is a vector. When we measure the magnetic anomaly we
measure one or more individual components of this field. The total field
anomaly is the projection of the anomalous field onto the direction of the
earth's field :math:`\hat{z}` so the magnetic field anomaly over the pipe is

.. math::
	B_t= \frac{\mu_0}{4 \pi} \frac{Q z}{r^3}

where :math:`z` is the depth of burial. Equivalently, if we substitute for the
magnetic charge and write the expression using the earth's magnetic field
:math:`B_0` then

.. math::
	B_t = \frac{\kappa \pi a^2 B_0}{4 \pi} \frac{z}{r^3}


Geologic Features and representation for modeling
-------------------------------------------------

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


