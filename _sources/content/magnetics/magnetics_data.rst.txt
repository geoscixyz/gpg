.. _magnetics_data:

Data
****

.. figure:: ./images/measurements.gif
    :align: right
    :figwidth: 50%
    :name: mag_measurment

    Contributions to a magnetic measurement

In this section we present a summary about the different types of magnetic data. Different assumptions are made depending on the type of :ref:`instrument<magnetics_instrumentation>` used during acquisition.

.. _magnetics_field_data:

Magnetic field data
-------------------

As demonstrated in :numref:`mag_measurment`, the magnetic field measured above the surface is a vector quantity. The *magnetic field data* measured at any location contains the signal from both the :ref:`source<earth_s_field>` (:math:`\mathbf{B}_0`), as well as the :ref:`response<magnetics_responses>` (:math:`\mathbf{B}_A`) from :ref:`magnetized<magnetics_magnetization>` material:

.. math:: \mathbf{B} = \mathbf{B}_0 + \mathbf{B}_A\;.

In ideal cases, magnetic surveys would measure all three components of the field (:ref:`fluxgate magnetometer<magnetics_fluxgate>`). The *magnetic field anomaly*, the quantity of interest, is readily available by simple subtraction of the inducing field such that:

.. math:: \mathbf{B}_A = \mathbf{B} - \mathbf{B}_0 \;.

The acquisition of three-components data remains challenging however. The orientation of each components needs to corrected in real-time in order to compensate for sensors rotation. Most surveys measure instead the total strength of the field, or *Total Magnetic Intensity* data:

.. math:: |\mathbf{B}| =   |\mathbf{B}_0 + \mathbf{B}_A| \;.

Since we do not know the direction of :math:`\mathbf{B}_A` we assume that the anomalous field is mostly induced and that it's direction aligns with the Earth's inducing field :math:`\mathbf{B}_0`. This allows us to approximate the *Total Magnetic Anomaly* datum:

.. math:: B_T = \mathbf{B}_A \cdot \mathbf{\hat B}_0 \;,

.. figure:: ./images/TMI_anomaly.png
    :align: center
    :figwidth: 50%

This assumption holds as long as :math:`\mathbf{\hat B}_0 \gg \mathbf{\hat B}_A`, which is valid in most cases considering the strength of the Earth's field.


.. _magnetics_gradient_data:

Gradient measurements
=====================

.. sidebar:: Outline of gradient magnetics

    .. figure:: images/icon_maggrad.gif
        :align: center

When buried objects are the target, geophysical surveys must usually detect
features with high magnetic susceptibility and/or high electrical
conductivity. Some objects will be magnetic, but others have negligible
magnetic susceptibility (such as aluminum or some forms of stainless steel).
When the buried targets are expected to be magnetic, measurements of
variations in the strength of Earth's magnetic field often produce excellent
results. However, because of the many ferrous objects and electrical sources
of magnetic fields under and around industrial sites, total field anomaly maps
may be too complicated to interpret, or subtle variations may be overwhelmed
by larger features. A gradient survey is often a better choice under these
conditions because the magnetic field gradient varies more rapidly than total
field strength and it, therefore, provides higher spatial resolution. This is
illustrated by the interactive figures below.

.. raw:: html
    :file: grad_mag.html

In addition to higher spacial resolution, temporal variations are
automatically eliminated because the measured parameter is a difference of two
total field measurements. Therefore, the base station measurements and
subsequent data corrections normally required for total field surveys are not
required. If the goal is to map variations in geological materials, then more
subtle trends in magnetic response must be observed.

The vertical gradient is measured using two
sensors at (typically) 2 and 3 meters above the ground. Horizontal gradient
surveys can be conducted if the sensors can be mounted some distance apart on
a frame.

.. Data acquisition
.. ================

.. Data acquisition of total field magnetics or gradient magnetics is very rapid.
.. For finding buried objects, simple anomaly detection is often adequate since
.. the depth of burial and quantitative estimates of physical properties may be
.. unimportant. Under these conditions, rapid acquisition of spatially dense data
.. sets is usually required, and results are often presented with minimal
.. processing. The most important survey design consideration is to avoid spatial
.. aliasing. For small 3D targets such as buried drums or other objects, a
.. tightly spaced grid would be required; while for 2D targets such as buried
.. utilities, data spacing along profile lines would likely be much tighter than
.. spacing between lines. This assumes that lines can be placed perpendicular to
.. the target orientation.
