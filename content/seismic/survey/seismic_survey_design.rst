.. _seismic_survey_design:

Survey design
*************

Energy in the ground
====================

Seismic body waves travel away from the source, into the ground. The energy
spreads in all possible directions away from the source, so wavefronts expand
as hemispheres under a source point, if the ground is uniform. The energy will
arrive at geophones at times depending upon the velocity of the waves in the
subsurface materials. When energy reaches a change in material, some energy
will be reflected from the interface, and some will pass through it. The
geometry of this situation is shown in the next figure.

.. <<place holder>> This is a place holder for active links

.. figure:: ./images/reflect.jpg
	:align: center

If seismic signals travel at higher velocity in the lower layer, then some of
the seismic energy travels along the interface, returning to the surface as a
"head wave" along a wave front similar to the bow wave of a ship (figure
below). These are refracted waves, and for geophones a long way from the shot
point, they represent the first arrival of seismic energy. In other words,
because head waves travel along the interface at the velocity of the "faster"
material, they eventually overtake the direct waves (green in the figure
below) traveling in the slower surficial materials.

.. figure:: ./images/refract.jpg
	:align: center

Of course energy is both **reflected** and **refracted**, so ground motion
detected at a geophone is a caused by the combination of direct, refracted and
reflected energy arriving at the geophone's location. The different types of
energy are distinguishable only because they have traveled along different
pathways. Refraction surveying takes advantage of the fact that refracted
waves arrive before reflected energy, so long as the geophone is at a great
enough distance from the shot point.


Signals that get recorded
=========================

Each geophone produces an electrical signal that is proportional to ground
motion (in one direction - usually vertical, but horizontal with special
geophones used for shear wave work). That signal is recorded for a short
period of time starting at the moment that the source of energy begins. We
observe these signals by plotting them as one wiggly line for each geophone's
signal. These signals are plotted next to each other so that ground motion at
each geophone can be seen as a function of time. An example showing ground
motion at 24 geophones is shown below.

.. figure:: ./images/rawdata.gif
	:align: center

On this plot, one geophone was not working properly. Geophones are labeled
with the first closest to the source. As expected, ground motion occurred
earlier at geophones closest to the source. For geophones 1 through 10, it
seems as if there was no ground motion at later times, however this is an
artifact of the "gain" (amplification) applied to these traces. Gain is lower
for geophone signals near the source because signal amplitudes are larger. If
the signals within the blue box are amplified and replotted, the adjustable
figure below results.

.. raw:: html
    :file: raw_refraction_data.html

This figure shows shorter segments of traces from 12 geophones. The signal
amplitudes have been amplified, so all ground motions are visible. There are
clear beginnings of ground motion for each trace, which appear later in time
for traces farther from the source. Finding exactly what time the ground first
moved at each geophone is called **first break picking**. It is not difficult
in this case, but it can be challenging if signals are weak. Use radio buttons
next to the figure to see the result of picking first breaks (also known as
first arrivals) on this figure. Once the picks are chosen, it becomes evident
that there is a definite pattern to the arrivals--there are straight lines
joining the first breaks of several adjacent traces. The third radio button
reveals straight line patterns emphasized by drawing red lines.

We will learn that first arrivals are either direct signals (for near
geophones) or refractions that have traveled along subsurface interfaces. The
objective of seismic refraction surveys is to determine the geometry of
subsurface interfaces, and this can be derived by analysis of the pattern of
first arrivals.

Reflections surveys
===================

In reflection seismology we record seismic pulses that are reflected from
boundaries which separate layers that have different acoustic impedances. Unlike in refraction surveying, information in
the seismogram which comes after the first arrival is important. In general the processing is considerably different than in refraction surveying. In reflection seismology, seismic records from many sets of shots and receivers are used to generate a Normal Incidence Reflection Seismogram which has reflections that correspond to a vertically traveling
wave. The reflections occur at travel times that are determined by the velocity and the length of the travel path in each
layer. The normal incidence reflection seismograms are acquired at regular distances along the surface and
are composited into a seismic section. This generates an image of the substructure that can be used in an identical manner to a radar section. The examples below illustrate how the seismic images can be interpreted in terms of geologic structure:

Two Examples
------------

.. figure:: ./images/Usgs_examples_mexicogulf.png

 Hart, Patrick et al., High-Resolution Multichannel Seismic-Reflection Data Acquired in the Northern Gulf of Mexico, 1998-99, http://geopubs.wr.usgs.gov/open-file/of02-368/, USGS Open File report 02-368, public domain, converted to PNG

.. figure:: ./images/Flat_Spot_in_Seismic.jpg

 By Joshua Doubek - Own work, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=27279591

  Flat spots are used as indicator for hydrocrbons. More Information about `flat spot`_: 

  .. _flat spot: https://en.wikipedia.org/wiki/Flat_spot_(reflection_seismology)



.. ./images/air_gun.gif
..	:align: right
..	:scale: 200 %

..	An air gun record from the Gulf of Patras, Greece, showing Holocene
..	hemipelagic (h) and deltaic (d) sediments overlying an irregular erosion
..	surface (rockhead, RH) cut into tectonized Mesozoic and Tertiary rocks of
..	the Hellenide (Alpine) orogenic belt. SB: sea bed reflection; SBM1 and
..	SBM2: first and second multiples of sea bed reflection; RHM1: first
..	multiple of rockhead reflection [#f1]_.


.. ./images/seismic_section_intro.gif
..	:align: right
..	:scale: 200 %
..
..	A seismic section from the northern Amadeus basin, central Australia,
..	illustrating a dispositional sequence bounded by major unconformities
..	[#f1]_.



Multichannel Reflection Survey
==============================

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
======================
  	

Multiple shots and receivers are used in a reflection seismic profiling
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

"Fold" in Seismic Reflection Surveying
======================================

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