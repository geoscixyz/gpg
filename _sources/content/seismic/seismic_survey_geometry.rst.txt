.. _seismic_survey_design:

.. Survey geometry
.. ***************

.. As a motivating example, consider the following two figures, showing typical reflection and refraction survey layouts.

.. .. figure:: ./images/reflect.jpg
..	:align: center

.. If seismic signals travel at higher velocity in the lower layer, then some of
.. the seismic energy travels along the interface, returning to the surface as a
.. "head wave" along a wave front similar to the bow wave of a ship (figure
.. below). These are refracted waves, and for geophones a long way from the shot
.. point, they represent the first arrival of seismic energy. In other words,
.. because head waves travel along the interface at the velocity of the "faster"
.. material, they eventually overtake the direct waves (green in the figure
.. below) traveling in the slower surficial materials.
.. 
.. .. figure:: ./images/refract.jpg
.. 	:align: center
.. 
.. Of course energy is both **reflected** and **refracted**, so ground motion
.. detected at a geophone is a caused by the combination of direct, refracted and
.. reflected energy arriving at the geophone's location. The different types of
.. energy are distinguishable only because they have traveled along different
.. pathways. Refraction surveying takes advantage of the fact that refracted
.. waves arrive before reflected energy, so long as the geophone is at a great
.. enough distance from the shot point.

Survey geometry
===============

Multichannel data collection
----------------------------

First consider the source-receiver geometry. The geometry can be "split
spread" in which case there is a central shot with receivers on both sides, or
a "single-ended spread" in which the receivers are always on one side of the
source. Split spreads are common in land surveys; single-ended spreads are
common in marine surveys.

.. figure:: ./images/split_and_single_spread.gif
	:align: center
	:scale: 110%

	Shot-detector configurations used in multichannel seismic reflection
	profiling .(a) Split spread, or straddle spread. (b) Single-ended spread
	[#f1]_

.. figure:: ./images/shot_gather_split_spread.gif
	:align: right
	:scale: 100 %   

.. <<editorial comment>> The original GPG had a "click to enlarge" feature for the shot gather. Should it be added?

A split spread seismic record is shown above. The seismic traces all belong to
a single source and hence this is referred to as a "Common Source Gather". The
first arrivals are direct or critically refracted arrivals. Reflection
hyperbolae from numerous boundaries are observed, right. The strong energy in
the triangular central portion is ground roll caused by surface waves. It
masks the reflection events.

Common MidPoints (CMP)
----------------------
  	
Multiple shots and receivers are used in seismic profiling
specifically so that some subsurface points are sampled more than once.
Ultimately the goal is to identify all the reflections due to that point on
the various seismograms and stack these to get an enhanced signal to noise
ratio. The idea is illustrated on the upper figure.

The collection of seismic traces that correspond to a particular midpoint is
called a Common Midpoint (CMP) gather. In older literature, this collection of
traces was referred to as a Common Depth Point (CDP) gather. That is not
strictly correct, as the bottom diagram illustrates.


 .. figure:: ./images/common_reflection_pt1.gif
    :align: center

    
    A series of six shots and associated receivers that would have
    reflections from a common point. When the layers are plane and horizontal
    then this common reflection point lies midway between the source and
    receiver


 .. figure:: ./images/common_reflection_pt2.gif
    :align: center

    
    Common depth point (CDP) reflection profiling. [#f1]_  (a) A set of rays
    from different shots to detectors are reflected off a common point on a
    horizontal reflector. (b) The common depth point is not achieved in the
    case of a dipping  reflector.

Refraction surveys
------------------

Seismic refraction is most useful when the velocity of seismic
signals in each layer increases with depth. Therefore, where higher velocity
(e.g. clay) layers may overlie lower velocity (e.g. sand or gravel) layers,
seismic refraction may yield incorrect results. In addition, seismic
refraction requires geophone arrays with lengths of approximately 4 to 5 times
the depth to the layer of interest (for example the top of bedrock). Therefore
seismic refraction is commonly limited to mapping layers to depths less than
30-50 meters. Greater depths are possible, but the required array lengths may
exceed site dimensions, and the shot energy required to transmit seismic
arrivals for the required distances may necessitate the use of large explosive
charges.
    
Reflection surveys
------------------

By contrast, reflection surveys are not hampered by low velocity layers but they have difficulty imaging the top 50m of the earth because reflections from such shallow depth are difficult to distinguish from direct arrivals and sound waves travelling through the air. In general, identifying a reflection event in a seismic record is more difficult than picking first arrivals for a refraction survey. Much signal processing is typically involved. In order to improve the ability to detect and image a given reflection event geophysicists typically design reflection surveys to detect a reflection from a particular point in the subsurface multiple times.

Fold
----

The fold refers to the number of times a particular subsurface point has been
sampled. It is equal to the number of traces in the CMP gather and is
numerically evaluated by

.. math::
 		fold = \frac{N (number\;of\;geophones)}{2n}

where :math:`n` is the moveup rate in units of geophone spacing. "Moveup rate"
is in fact (shot spacing)/(geophone spacing). For example, if geophones are 2
meters apart and shots are employed every 4 meters, then the moveup rate is
n=4/2=2. This can be less than one if there are shots set more often than
geophone spacing, a practice that is sometimes done in marine seismology,
especially ocean bottom profiling.

The schematic below shows a single ended spread with 8 geophones and moveup
rate of n=2.

.. figure:: ./images/fold.gif
    :align: center

We see that each point in the subsurface is sampled only twice. Notice that
the distance between the reflection points in the subsurface is half the
geophone spacing.

.. [#f1] From Kearey, Philip and Micheal Brooks, '*An Introduction to Geophysical Exploration*'. 2nd ed. Blackwell Science: 1991. 