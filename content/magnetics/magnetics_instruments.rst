.. _magnetics_instruments:

Instruments for magnetic surveys
********************************

A measurement of the magnetic field at any location will involve either recording the magnitude in one or more vectorial coordinate directions, or a magnitude in the field's direction (commonly referred to as "total field strength"). There are many manufacturers of magnetometers for ground, marine, helicopter, fixed wing, and space-borne geophysical use. Instrument types commonly used are outlined very briefly as follows:

Fluxgate Magnetometer
=====================

- This type of instrument was developed during WWII to detect submarines. It measures the magnitude in a specific direction determined by the sensor's orientation. A complete measurement of the field requires three individual (cartesian) components of the field ( such as \\(B_x\\), \\(B_y\\), \\(B_z\\) ).
- It is generally difficult to get leveling and alignment accurate. Sensor accuracy is 1 nT so orientation must be known to within .001 degrees.
- There are some fluxgates which generate a measure of the total field strength.

Proton Precession Magnetometer
==============================

- This instrument was the most common type before the mid 1990's. It measures the total field strength.
- Advantages: Sensitive to 1 nT, small, rugged & reliable, not sensitive to orientation.
- Disadvantages: Takes >1 sec to read, sensitive to high gradients. 
- The measurement process is related to nuclear magnetic resonance (NMR). A proton source (possibly as simple as a volume of water) is subjected to an artificial magnetic field, causing the protons to align with the new field. When the artificial field is removed, the protons precess back to their original orientation and their precession frequency (called the *Larmor* precession frequency) is measured. That frequency, f, is related directly to the strength of the earth's field according to the equation to the right. The parameter,p, is the ratio of the magnetic moment to spin angular momentum. It is called the gyromagnetic ratio of a proton and is known to 0.001%; \\( \\gamma_p = 2.67520 \\times 10^8 T^{-1} s^{-1} \\).

.. math::
	f= \frac{\gamma_p B_e}{2 \pi}

Cesium (or optically pumped) magnetometer:
==========================================

- The physics behind this type of sensor is related to that of the proton precession sensor, but it is more complicated. Although it is more expensive than the above two sensor types, it is now the most commonly used system for small scale work because it is 10 to 100 times more sensitive than the proton precession magnetometer.
- The measurement process makes use of the gyromagnetic ratio of electrons and of the quantum behavior of outer-shell electrons of some elements (e.g. cesium). In this case, the relevant gyromagnetic ratio is known to 1 part in 10\ :sup:`7`\ , and frequencies are near 233 khz, so these instruments are sensitive to 0.01 nT. 
- Advantages: More rapid readings, 1 or 2 orders of magnitude more sensitive, works in high gradients.
- Disadvantages: Optical pumping won't work when parallel or perpendicular to mag field direction (solved with multiple sensors), more expensive than proton precession.

**SQUIDS** (superconducting quantum interference devices): These are very sensitive, and are currently more common in laboratories that work on rock magnetism or paleomagnetic studies. However, they are beginning to be used in the field, and more applications will become evident in the coming decade (2000 - 2010). Search the internet using, for example, "squid AND magnetometer AND geophysics" as keywords.

Magnetic Gradiometer
====================
- These instruments use two sensors (any of those mentioned above) to measure vertical or horizontal gradients.
- They often employ two cesium magnetometers separated by about 1 m.






