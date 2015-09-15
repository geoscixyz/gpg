.. _seismic_reflection_fold:

"Fold" in Seismic Reflection Surveying
**************************************

The fold refers to the number of times a particular subsurface point has been
sampled. It is equal to the number of traces in the CMP gather and is
numerically evaluated by

.. math::
 		fold = \frac{N (number\;of\;geophones)}{2n}

where \\(n\\) is the moveup rate in units of geophone spacing. "Moveup rate"
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
