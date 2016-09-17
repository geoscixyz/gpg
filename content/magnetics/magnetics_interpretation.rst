.. _magnetics_interpretation:

Interpretation
**************

In this we focus on various techniques used to interpret the magnetic data.
From an applied geoscientists standpoint, this is where most of the data integration and decision making steps are made. We illustrate each the interpretation techniques on a mineral exploration example.

Tli Kwi Cho (TKC): *A primer*
================================================

.. figure:: ./images/TKC_Location.png
  :align: right
  :figwidth: 50%
  :name: TKC_Location

We start with a brief overview the Tli Kwi Cho kimberlite project.
Tli Kwi Cho (TKC) is a kimberlite complex in the Northwest Territories,  Canada.
The Northwest Territories have been surveyed extensively for diamondiferous kimberlites since the early 1980s. The Lac de Gras region has been particularly productive, and hosts two of the largest Canadian deposits: the Ekati and Diavik mines.


.. figure:: ./images/TKC_Kimbs.png
  :align: right
  :figwidth: 50%
  :name: TKC_Sketch

A common geophysical fingerprint for a kimberlite pipe is a circular strong magnetic anomaly, with a gravitational low and an anomalous electromagnetic (EM) response.
A generic model for kimberlite pipes found in the Lac de Gras region is presented in :numref:`TKC_Sketch`. The main rock types associated with kimberlites are summarized in :numref:`TKC_rocks`.

.. list-table:: : Common rock types associated with kimberlites found in the Lac de Gras region
   :header-rows: 1
   :widths: 1 1 1
   :stub-columns: 0
   :name: TKC_rocks

   *  - Rock Type
      - Description
      - Susceptibility
   *  - Pyroclastic Kimberlite (PK)
      - Extrusive, violent, post-eruption
      - Moderate-low
   *  - Volcaniclastic Kimberlite (VK)
      - Extrusive, fragmental, main body
      - Moderate-low
   *  - Hypabyssal Kimberlite (HK)
      - Intrusive, igneous, coherent
      - High
   *  - Glacial till
      - Sedimentary
      - Low


The TKC kimberlite complex was identified from an airborne magnetic and frequency-domain electromagnetic DIGHEM survey in 1992.
Geophysics had been used during the discovery phase of TKC, but little had been done to model the deposit prior to drilling. As we will later discover, the TKC deposit differ from the standard kimberlite model found in the region.
Consequently, the geological model used to explain the deposit underwent several revisions over the following decades.
In this section, we will attempt to extract as much information as possible about the deposit strictly from the original airborne magnetic survey.


Data interpretation
===================

The first and simplest analysis can be done directly on the :ref:`Total Field Anomaly<magnetics_field_data>` data as shown below. From the raw data, we notice a regional trend coming from the east of the survey area. In order to enhance the local anomalies, we first proceed with a :ref:`regional trend removal`<magnetics_regional_trend>`. A :math:`1^{th}` Order polynomial is subtracted from the raw data and presented below.

.. raw:: html
    :file: TKC_Data_Processing.html


Derivative Maps
---------------

While the data itself can be informative, image filtering techniques are commonly used by industry to further highlight important features present in the data.


.. raw:: html
    :file: TKC_Data_Filters.html




Parametric Simulation
=====================

From the data map, we identified at least two important features.

 - Elongated magnetic anomalies that may correspond to intrusive dykes.

 - A compact, near circular anomaly that could resemble a kimberlite pipe.

In order to test these hypothesizes, we first attempt to approximate the magnetic features with simple parametric objects.

Plate model
-----------

Using the :ref:`magnetic app<magnetics_applet>`, we first look at the elongated features. :numref:`TKC_param_dyke` compares the magnetic data over the elongated with the magnetic simulated plate. The parameter used for the plate model are presented in :numref:`Param_dyke`. This result seems to confirm the presence of thin, shallow dipping magnetic dykes.Turns out that these dykes, part of the Mackenzie dyke swarm, run through out the region and are related to major tectonic events. Although interesting scientifically, they are of little interest in diamond exploration.

.. figure:: ./images/TKC_Parametric_Dyke.png
  :align: center
  :name: TKC_param_dyke

.. list-table:: : Parameter used to model the dykes
   :header-rows: 0
   :widths: 1 1
   :stub-columns: 0
   :name: Param_dyke

   *  - Dimensions
      - 50 x 800 x 500 m
   *  - Dip
      - :math:`20^\circ`
   *  - Susceptibility
      - 0.1 SI


Pipe model
----------

Second, we look at the compact, near circular magnetic anomaly in the center of the survey area. This feature may be of interest as it resemble the typical signature of a kimberlite pipe.
:numref:`TKC_param_pipe` compares the magnetic data over the compact anomaly and the parametric pipe model (:numref:`Param_dyke`). This result seems to confirm the presence of a compact magnetic block SE dipping. The shape of the anomaly is surprisingly different than the expected shape of a vertical pipe. This result requires additional work for validation, hence the need to invert the data.

.. figure:: ./images/TKC_Parametric_Pipe.png
  :align: center
  :name: TKC_param_pipe

.. list-table:: : Parameters used to model the pipe
   :header-rows: 0
   :widths: 1 1
   :stub-columns: 0
   :name: Param_pipe

   *  - Dimensions
      - 300 x 200 x 50 m
   *  - Dip
      - :math:`20^\circ`
   *  - Susceptibility
      - 0.05 SI


Inversion
=========



Old Material
============

.. _separate sidebar: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/blakely/blakely.html


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

