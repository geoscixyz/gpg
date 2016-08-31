.. _magnetics_basic_principles:

Basic Principles
****************

.. _earth_s_field:

Earth's Field
=============

.. figure:: ./images/ironfilings.gif
	:align: right
	:figclass: float-right-360
	:scale: 110% 

Most people are familiar with the magnetic field that exists around a dipolar
or "bar" magnet (shown to the right as the pattern of iron filings on paper
over a bar magnet). To a first approximation, Earth's magnetic field looks
like that of a dipolar source within the Earth, which is tilted about 11.5
degrees from the spin axis and is slightly off center. This field has a
strength of approximately 70,000 nanoTeslas (nT) at the magnetic poles and
approximately 25,000 nT at the magnetic equator.The figure below-left
illustrates a cross-section of the field as it could be imagined from space.
Below-right is a sketch of the directions of the field at Earth's surface.

There are, in fact, three different components to Earth's field:

 - **External variations** caused by currents flowing in the ionosphere. For magnetic surveys, these *diurnal variations* and considered to be source of noise and removed from the observed data. 
 .. figure:: ./images/fig_2a.jpg
	:align: center
	:figwidth: 40%

 - **The main dipolar field** of the earth produced internally by large currents in the fluid outer core of the earth. This is also refered to as the *inducing field*, and it is the main magnetic source for the magnetic geophysical surveys.
 .. figure:: ./images/Earth_Field.png
	:align: center
	:figwidth: 40% 


 - **Secondary magnetic fields** due to rocks or buried bodies that are the objective of geophysical surveys. These fields are the *signals* we have to work with, and they may be either permanent (always present, regardless of the ambient local field) or induced (caused by Earth's field).
 .. figure:: images/magnetic_anomaly.gif
   :align: center
   :figwidth: 40%

Describing Earth's field
------------------------

.. figure:: ./images/earthfield.gif
	:align: right
	:figwidth: 40% 
	:name: earth_mag_vectors
	
	: Earth's magnetic field orientation

The convention for drawing magnetic field lines is that they flow outward from
a positive pole and inward to a negative pole. The Earth's field behaves like
there is a negative pole in the northern hemisphere and a positive pole in the
southern hemisphere as shown in :ref:`earth_mag_vectors`. 
In 2004, Earth's north magnetic pole was close to Melville Island at
(Latitude, Longitude)=(79N, 70W). At Vancouver D ~ 20° east, I ~ 70° down from
horizontal.

Using B to represent the
magnetic field of Earth as a vector in three dimensions, the field at any
location on (or above or within) Earth can be described in either of three
ways (refer to the next figure below):

 - B = (:math:`B_x`, :math:`B_y`, :math:`B_z`) = (X, Y, Z) in the figure. These are Cartesian coordinates with X pointing to true (geographic) north, Y pointing east and Z pointing vertically down.

 - B = (:math:`B_h` , :math:`B_z` , :math:`D`) = (H, Z, D) in the figure. These are horizontal and vertical components, plus declination (angle with respect to true north). 
    
 - B = (:math:`D`, :math:`I`, :math:`\mid B\mid` ). These are the commonly used polar coordinates which include two angles and a magnitude: D=declination, I=inclination, and :math:`\mid B \mid` =total field strength.

.. figure:: ./images/components.gif
	:align: center
	:scale: 100% 

	Sketch of coordinates used to describe magnetic fields.

* **B** is the vector representing Earth's magnetic field. Its length represents the magnitude of the field strength (sometimes referred to as F).
* **H** is the projection of the field, **B**, onto the surface.
* **Z** is the projection of the field, **B**, onto the vertical direction.
* **X** is the projection of the field, **B**, onto the northward direction.
* **Y** is the projection of the field, **B**, onto the eastward direction.
* **D**: declination is the angle that *H* makes with respect to geographic north.
* **I**: inclination is the angle between **B** and the horizontal. It can vary between -90° and +90°. 

The details of Earth's field at any location on Earth are described using a
formula based upon a spherical harmonic decomposition of the field called the
:ref:`IGRF<magnetics_IGRF>` or International Geomagnetic Reference Field. Details about Earth's field
can be found at government geoscience websites such as the `NOAA`_ geomagnetism home page, or the `Canadian National Geomagnetism Program`_ home
page. 

**Other resources**
 - Earth's `magnetic field calculator`_.

.. _NOAA: http://www.ngdc.noaa.gov/geomag/geomag.shtml
.. _Canadian National Geomagnetism Program: http://www.geomag.nrcan.gc.ca/index-eng.php
.. _magnetic field calculator: http://www.ngdc.noaa.gov/geomag-web/


.. _magnetics_three_figures:

Earth's magnetic field
----------------------

These three figures show how declination, inclination and field strength
varies around the world, based upon the IGRF for 2003. The images were
generated using data obtained from the NOAA National Data Center.


.. figure:: ./images/earth-decl.gif
	:align: center
	:scale: 100% 

.. figure:: ./images/earth-incl.gif
	:align: center
	:scale: 100% 

.. figure:: ./images/earth-strength.gif
	:align: center
	:scale: 100% 


Variability of Earth's field
----------------------------

The source of the main (nearly dipolar) field varies slowly, causing changes
in strength, declination and inclination over time scales of months to years.
Changes in the exact location of the magnetic north pole are caused by this
effect. See the Geological Survey of Canada's website for a conversational
history of the location of the Magnetic North pole. Declination varies very
widely in Canada. The correct value of declination can be found by entering
your latitude, longitude and year at the GSC's website.

 .. figure:: ./images/solar_wind.jpg
	:align: right
	:figclass: float-right-360
	:scale: 110% 

The second component of Earth's field involves external contributions due
primarily to currents in the ionized upper atmosphere.

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


Temporal variations are often larger than geophysical anomalies. They must be
accounted for in all surveys and this is usually done by acquiring data at a
fixed base-station. Another alternative is to acquire gradient data that use
two fixed sensors. The figure below shows an example magnetic noise that may be 
encountered as a result of a geomagnetic storm. These temporal variations have 
an impact on magnetic data measured over time scales of several days, hours, or 
minutes.

 .. figure:: ./images/pipe3_timelapse_edit.gif
	:align: center
	:scale: 110% 

	Adapted from NRC http://www.spaceweather.gc.ca/tech/se-pip-en.php

The Geological Survey of Canada has a web page, which can provide graphs of
diurnal variations observed at any of 11 magnetic observatories in Canada, for
any day in the most recent 3 years. Find this facility by starting at the`GSC
Geomagnetic data page`_. This resource is also a link to other information
about magnetics.

.. _GSC Geomagnetic data page: http://www.geomag.nrcan.gc.ca/index-eng.php

.. _magnetics_IGRF:

The IGRF
========

Here are a few remarks about the IGRF or International Geomagnetic Reference Field.

The IGRF is a mathematical model that describes the field and its secular
changes as a spherical harmonic expansion. It is updated every five years, and
**later** versions may re-define the field at **earlier** times. This is
important to remember if you are comparing old maps to new ones. The IGRF is a
product of the International Association of Geomagnetism and Aeronomy (IAGA_),
and the original version was defined in 1968.

.. _IAGA: http://www.ngdc.noaa.gov/IAGA/vmod/

Every five years, the IAGA issues a contemporary main field model that
predicts the field for the next five years. These models have names that are
prefixed with "IGRF." Each new model updates the model that was used to
predict the previous five (or more) years. Updated models are called **DGRF**
for **Definitive Geomagnetic Reference Field**. Major updates since 1980 use
data from MAGSAT, consisting of measurements of vector components and total
intensity of the geomagnetic field between 350 and 560 km altitude.

To correct data sets which had older versions of reference fields removed, add
:math:`(F_0 - F_n)` to each data point, where the two parameters are total
intensity values computed from the old and new reference fields respectively.
See Peddie N.W. 1982, 1983, and 1986 for details. Charts of many types are
available on-line, as downloadable postscript files, and for sale (less than
$5.00 each) from the USGS, NOAA, GSC, and just about any other government
geoscience agency. For example, you could use either the NOAA Geomagnetism
page_, or the Canadian National Geomagnetism Program's homepage_.

.. _page: http://www.ngdc.noaa.gov/ngdc.html
.. _homepage: http://www.geomag.nrcan.gc.ca/index-eng.php

References:

* Peddie, N. W., 1986, Report on International Geomagnetic Reference Field revision 1985 by IAGA Division I Working Group 1: *Geophysics*, 51, no. 4, 1020-1023.
* Peddie, N. W., 1983, International Geomagnetic Reference Field - its evolution and the difference in total field intensity between new and old models for 1965-1980 (short note): *Geophysics*, 48, no. 12, 1691-1696.
* Peddie, N. W., 1982, Report on International Geomagnetic Reference Field 1980 by IAGA Division I Working Group 1: *Geophysics*, 47, no. 5, 841-842.

.. _magnetics_buried_dipole:

Fields due to a magnetic dipole
===============================


The general principles of magnetic surveying are encapsulated into the following steps:

(a) An object with magnetic susceptibility :math:`\kappa` is buried in the
    earth.

(b) At the location of burial, the earth's field magnetic field is :math:`\vec{H}` and the magnetization in the object is :math:`\vec{M} = \kappa \vec{H}`.

(c) If the object is "small", that is all of the object's dimensions are several times smaller than the depth to its center, then  the object acts as a "magnetic dipole" -- that is, a little bar magnet with strength and direction caused by the inducing field. The  dipole moment of the object is :math:`\vec{m} = \text{Volume} * \vec{M}`

(d) The magnetic field of the object is referred to as the "secondary" field or sometimes the "anomalous" field :math:`\vec{B_A}`. This is what we seek to measure. 

(e) :math:`\vec{B_A}` is a vector field and hence requires three components to specify it. In the accompanying applet observations of individual components :math:`(B_x,B_y,B_z)` can be displayed. The projection of :math:`\vec{B_A}` onto the direction of Earth's field :math:`\hat{B_0}` is called the *total field* (:math:`B_t`). 


 .. figure:: ./images/TMI_anomaly.png
	:align: center
	:scale: 110% 

	When using a total field magnetometer we measure :math:`\left|\vec{B}\right|` which is equal to :math:`\left|\vec{B_0} + \vec{B_A}\right|`. Since we do not know the direction of :math:`\vec{B_A}` we assume that the anomalous field is mostly induced and that it's direction aligns with the Earth's inducing field :math:`\vec{B_0}`. This allows us to approximate the *total field* datum (:math:`B_t`) as the projection of :math:`\vec{B_A}` onto the direction of Earth's field :math:`\hat{B_0}`.


In addition the vertical gradient of the field, obtained if measurements were
acquired with a gradiometer, are listed as :math:`B_g`.  Sign conventions must
be adopted when data are plotted. For magnetic surveying the coordinate system
used is: {:math:`x` is northing, :math:`y` is easting, and :math:`z` is downward}.
The sign convention will be that horizontal fields are positive if they point
in the :math:`\hat{x}` direction for :math:`B_x`, in the :math:`\hat{y}` direction
for :math:`B_y` and vertical fields are positive if they point downward. For
:math:`B_t` the anomaly is positive if it points in the same direction as the
earth's field and negative if it is the opposite direction.

Understanding the magnetic fields of a buried dipole, and the resultant
observations, is crucial because all real scenarios can be thought of as a
combination (superposition) of dipoles (see the "Buried structures" section).
More advanced applets will be used to look at the responses of some of these
bodies.


The figures below illustrate the problem. The pattern recorded at the surface
arises by measuring the field strength everywhere on the surface, removing the
Earth's field, and then plotting the results as a contour map of anomalous
field strength. In the third figure, regions of blue anomalous field are
"negative" because at those surface locations, the **anomalous** field
crossing that surface points in the opposite direction for Earth's field.

.. raw:: html
    :file: buried_dipole.html

Magnetic dipoles: a Java applet
-------------------------------

As noted above, a real buried feature will look like a magnetic dipole if its
physical dimensions are much smaller than the depth to the feature's center.

The response that will be measured at points on a surface overlying a buried
magnetic dipole can be explored using the UBC-GIF magnetic dipole Java applet;
click here_ to start it in a separate browser window. Be sure to read the
description and instructions below the applet before using it. This tool shows
you a surface map of the total field anomaly, :math:`B_t`, after you specify
the inclination, declination, and strength of the inducing field, the depth of
the buried dipole, and the strength of the buried dipole's magnetic moment,
**m** (which is proportional to its magnetic susceptibility and the inducing
field strength). Recall from the introduction that the induced magnetization
in a material is related to its susceptibility via :math:`\vec{M} =\kappa
\vec{H}` and the magnetic moment is a volume integral of the magnetic
susceptibility.

.. _here: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/magdipole/dipoleapp.html

Note that the applet also allows you to define a line across the surface map
and observe a line profile of the anomaly. Also, there are options for
displaying the surface map of the X, Y, or Z-component, or the vertical
gradient, :math:`B_g`, as if the total field had been measured using two sensors
1 m apart.

The next figure shows three versions of the field induced in a buried object
under a survey line, which is oriented towards magnetic north. The UBC-GIF
dipole applet is also used to show the measured (i.e. anomalous) fields that
would be recorded over the surface.


On the cross section, red arrows show Earth's field's direction, blue arrows
show induced field vectors, and the sign of measurements can be determined by
comparing the directions of these two fields at each location on the Earth's
surface. On the map and profile image (which shows the dipole applet screen),
pay particular attention to the amplitudes. Also note that the profile is
approximately anti-symmetric, *not* at :math:`45^\circ` latitude but at around
:math:`30^\circ` latitude.

.. raw:: html
    :file: buried_dipole2.html

The map and profile anomaly at the surface calculated by the UBC-GIF dipole
applet is plotted to the right.
  
.. _magnetics_extended_bodies:

Fields from extended bodies
===========================

Approximating targets using magnetic charges
--------------------------------------------

 .. figure:: ./images/buried_bodies1.gif
	:align: right
	:figclass: float-right-360
	:scale: 100% 

If :math:`L` denotes the scale length of a buried object and the distance from
the observer to the body, :math:`R` is :math:`\gg` :math:`L`, then the magnetic
field of the body will look like that due to a simple dipole. If the buried
object has a complicated structure or the observer is very close to the
magnetized object then it can no longer be represented as a single dipole.  In
:ref:`magnetics_complex_structures<magnetics_complex_structures>`, we will present a general method for
computing the magnetic response from an arbitrary object but here we look at
objects that have a uniform magnetic susceptibility. We introduce the concept
of magnetic charge and show how this can be used to compute the response for
some simple objects like a pipe or sheet.


First we begin with the concept of magnetic charges or poles. They can't be
generated in practise. If you cut a small magnet in half, you will have two
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
	:scale: 110% 
	:name: Positive_magnetic_pole

	Magnetic field lines generated by a postive magnetic pole.


 .. figure:: ./images/Negative_magnetic_pole.png
	:align: center
	:scale: 110% 
	:name: Negative_magnetic_pole

	Magnetic field lines generated by a negative magnetic pole.


If a positive and negative charge are put in proximity they form a dipole and
the field lines look like the diagram below.

 .. figure:: ./images/Magnetic_dipole.png
	:align: center
	:scale: 110% 
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
=============================

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
