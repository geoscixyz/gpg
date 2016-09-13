.. _magnetics_interpretation:

Interpretation
**************

In this we focus on various techniques used to interpret the magnetic data.
From an applied geoscientists standpoint, this is where most of the data integration and decision making steps are made.

Inferences from data maps
=========================

.. figure:: ./images/earth-strength-s.gif
  :figclass: float-right-360
  :align: right
  :scale: 100%

2D plots of magnetic data, often referred to as maps, can provide insight
about the geologic units, contacts, and the horizontal location of structures.
What is presented, and how it is presented can greatly alter interpretations
obtained by visually analyzing the maps. Raw data are not usually presented
directly. Choices of contour plotting parameters must be made; features not
related to targets might be removed; and data or image enhancement processing
might be employed. Here we introduce some aspects of these topics.

The most common form of magnetic survey data involves "total field"
measurements. This means that the field's magnitude along the direction of the
earth's field is measured at every location. To the right is a total field
strength map for the whole world (a full size version is in the sidebar_).

.. _sidebar: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/sidebar-fields.html

At the scale of most exploration or engineering surveys, a map of total field
data gathered over ground with no buried susceptible material would appear
flat. However, if there are rocks or objects that are magnetic (susceptible)
then the secondary magnetic field induced within those features will be
superimposed upon the Earth's own field. The result would be a change in total
field strength that can be plotted as a map. A small scale example is given
here:

.. raw:: html
    :file: data_plotting1.html

Large data sets are commonly gathered using airborne instruments. They may
involve :math:`10^5` to :math:`10^6` data points to show magnetic variations over many square
kilometers. An example of a large airborne data set is shown to the right,
with a larger version, including alternative colour scale schemes, `shown in a
sidebar`_.

.. _shown in a sidebar: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/sidebar-airmaps.html

.. figure:: ./images/map-cust.gif
  :figclass: float-right-360
  :align: right
  :scale: 40%

Such data sets were once too large to invert directly, but they still provide
extremely valuable information about geology and structure, especially if some
processing is applied to enhance desirable features and/or suppress noise or
unwanted features. With recent advancements in computational power and
inversion methodologies these large scale problems are becoming easier to
invert.


Derivative Map
--------------

There are numerous options for processing potential fields data in general,
and magnetics data specifically. One example is shown below. The processing was applied in
this case in order to emphasize geologic structural trends.

.. raw:: html
  :file: Airborne_magnetics_example.html


Other examples of magnetic data processing techniques include:

- Upward continuation is commonly used to remove the effects of very nearby
  (or shallow) susceptible material.

- Second vertical derivative of total field anomaly is sometimes used to
  emphasize the edges of anomalous zones.

- Reduction to the pole rotates the data set so that it appears as if the
  geology existed at the north magnetic pole. This removes the asymmetry
  associated with mid-latitude anomalies.

- Calculating the pseudo-gravity anomaly converts the magnetic data into a
  form that would appear if buried sources were simply density anomalies
  rather than dipolar sources.

- Horizontal gradient of pseudo-gravity anomaly: gravity anomaly inflection
  points (horizontal gradient peaks) align with vertical body boundaries;
  therefore, mapping peaks of horizontal gradient of pseudo-gravity can help
  map geologic contacts.

The effects of these five processing options are illustrated in a `separate
sidebar`_ on processing of magnetics data.

.. _separate sidebar: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/blakely/blakely.html


Parametric Simulation
=====================


Inversion
=========

Case Study
==========
