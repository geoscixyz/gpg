.. _magnetics_introduction:

Introduction
************


The generic magnetic survey is summarized in :numref:`mag_response`.
The energy source is a magnetic field. The physical
property of interest is the magnetic susceptibility. The data
are magnetic field values.
Signals are sometimes interpreted in terms of geologic units, or
geologic structure (such as faults or dykes) but most often the
data are inverted to yield the subsurface
distribution of the magnetc susceptibility.

.. figure:: ./images/Intro_Response.png
    :align: center
    :scale: 50 %
    :name: mag_response

    A simple magnetic survey

A pictoral summary of magnetic surveying is
illustrated in :numref:`mag_survey` There are four main
elements:

The **energy source** is the Earth's magnetic field.
It has a strength and direction at every location on the Earth.

Subsurface materials can often be thought of as acting like a
small magnetics. The material therefore becomes magnetized when
a magnetic field is applied. The physical property that quantifies
this is the **magnetic susceptibiilty**.

The magnetized material creates a magnetic field (often called the
induced field).  The data from the survey
will be a superposition of Earth's field and the induced
fields caused by the magnetization of the buried materials.

The end goal of a magnetic survey is to infer information about the
sub-surface from the measured magnetic field data. The data are processed
and sometimes resultant data maps can be used to infer
geologic information. More generally, the data are inverted to
generate 2D or 3D images of the subsurface.



.. list-table:: :Principals of magnetic surveys.
   :header-rows: 0
   :widths: 10
   :stub-columns: 0
   :name: mag_survey

   *  - .. raw:: html
            :file: intro.html

Magnetic data can be used in a variety of ways and for different purposes.
One of the most useful is to use magnetic data for geologic mapping.
The example below shows a magnetic map and a geologic  map over the
same area. There are many geologic units that have a distinct magnetic
signature but the correspondence in not one-to-one.


    .. figure:: ./images/intro_geomaping.png
        :align: center
        :scale: 100 %
        :name: intro_geomaping

        : (a) Magnetic data.  (b)  A geologic map, over the same geographical area


Magnetic data can be used for remediation  and engineering work. The
image below shows the magnetic data over an area that is contaminated by
UXO. Each UXO has a signature like that of a magnetic dipole but the
orientations are random. These data provide fairly localized information
about where to dig to find the ordnance item. However, the data can
be further analysed through a parameteric inversion to find the
location in 3D space and also the size of the object. These are
valuable pieces of information when the area is being reclaimed.

    .. figure:: ./images/intro_paramEstim.png
        :align: center
        :scale: 100 %
        :name: mag_paramEstim

        : (a) A typical UXO site.  There is no surface indications of ordnance items. (b) Typical ordance items (c) Magnetic field data over a  site contaminated with UXO.


Magnetic data are also routinely used in mineral exploration.
In this application however, the data must be inverted to recover
information about the structure of the deposit at depth. The ability
to extend surface information into depth is one of the most
valuable results to be obtained from geophysical data.


    .. figure:: ./images/intro_exploration.png
        :align: center
        :scale: 100 %
        :name: mag_exploration

        : (a) Magnetic data map with the earth's field removed. (b) A volume rendered image of the 3D magnetic susceptibility obtained by inverting the data in (a).
