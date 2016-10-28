.. _electromagnetic_basic_principals:

Basic Principals
****************

Electromagnetic (EM) Induction
==============================

Consider the goal of using an inductive EM source to locate a conductive body
buried in a relatively non-conducting (or resistive) host material. The basic
picture is shown below

.. figure:: ./images/Tx_Rx_schematic.jpg
    :align: center
    :scale: 100 %

Transmitter
===========

The transmitter may be a loop of wire connected to a generator which outputs a
sinusoidal current. For examples, the current is :math:`I_0 \cos(\omega t)`
where :math:`\omega = 2 \pi f`.

Primary EM field
================

The current in the transmitter loop produces a magnetic field. In air
(sometimes referred to as free space) this magnetic field travels at the speed
of light :math:`c = 3.0 \times 10^8` m/s and therefore reaches the receiver
"instantaneously." The magnetic field observed at the receiver is called the
"primary field." Mathematically, the magnetic field would be written as
:math:`\vec{H}_p = \vec{H}_0 \cos(\omega t)`. The direction of the field
would depend upon the orientation of the wire. When we discussed magnetism we
showed that the magnetic field from a loop source was identical to that of a
permanent bar magnet at the center of the loop provided that the observer is
"far" from the loop. That is, this approximation holds when :math:`r\, >>\,
a` where :math:`r` is the distance from the observer to the center of the loop
and :math:`a` is the radius of the loop. The magnetic moment from a loop is
:math:`\vec{m} = IA \hat{n}`, where :math:`I` is the current in the loop,
:math:`A` is its area, and :math:`\hat{n}` is the unit vector perpendicular to
the plane of the loop.

Receiver
========

This is an instrument which measures the magnetic field. The receiver could be
a magnetometer oriented to record one component of the field or it could
possibly measure multiple components of the magnetic field. It could also be a
coil . In this case, a voltage is measured and the voltage is related to the
rate of change of magnetic flux crossing the loop.

At the Buried Body
==================

There is a time varying magnetic field impinging upon the conductor. This sets
up an electric force which causes currents to flow. The strength of the
currents is governed by Ohm's law:

.. math::
        \vec{J} = \sigma \vec{E}

where :math:`\vec{J}` is current density in :math:`A/m^2` (amperes per meter
squared) and :math:`\vec{E}` is the electric field with units of Volts/meter.

The currents in the body produce their own magnetic field (This is known as
Ampere's Law or Biot Savart Law). These currents will also vary with time and
their magnetic field can be measured at the transmitter. We refer to these
fields as the "secondary" magnetic field, :math:`\vec{H_s}`.

**Observation**: The receiver measures the sum of the primary and secondary
fields or it measures the associated voltages that are induced in a coil
caused by the time varying magnetic flux.

Summary
=======

1. A time varying current in a transmitter produces a time varying magnetic
   field which impinges upon a conductor in the ground.
2. The changing flux generates and electric field everywhere.
3. The electric field generates currents via Ohm's Law, :math:`\vec{J} = \sigma \vec{E}` .
4. The currents produce their own magnetic fields.
5. The receiver measures the sum of the primary and secondary fields,
   (or it measures associated voltages.)

Responses from a Conductor in Free Space
========================================

.. figure:: ./images/Hp_Hs_schematic.jpg
    :align: center
    :scale: 80 %

The basic understanding of the different coupling between
the source and receiver that is due to geometry, allows us to sketch the
expected responses that arise from a frequency domain horizontal loop survey
taken over a conductor which is buried in a resistive host. This is a two-
stage process.

1. Use the geometries of the source and receiver to sketch the characteristic
   curve.
2. Use the response diagram and the knowledge of whether you are
   dealing with a good conductor or poor conductor to determine the relative
   amplitude of the in-phase and out-of-phase parts.


**Part I:** Consider the basic geometry given below. For any placement of the
transmitter there will be a varying magnetic field crossing the plate and
hence induced currents. Those currents generate secondary magnetic fields.
Adopt a convention that if the secondary field is in (he same direction as
the primary field then the response will be plotted as a positive value.
Alternatively, when the two fields are in opposition the response will be
negative. The distance between the transmitter and receiver loops is held
fixed and the-datum is plotted at the midpoint between the coils. When both
loops are to the left, or to the right, of the plate then the response is
positive. The response will be zero when either coil is over the plate. When
the receiver, which is a horizontal coil, is over the plate, then no
magnetic flux is passing through the coil. There will be zero voltage
induced. When the transmitter is directly over the thin conducting plate,
there is no flux crossing the plate, hence no currents will be generated in
the plate and the secondary magnetic field is zero.


 .. figure:: ./images/source_receiver_signal.jpg
    :align: center
    :scale: 100 %

**Part II:** The basic sketch for the shape of the anomalous signal is
determined from the geometry of the coils and the relative locations of
transmitter, receiver and the conductive body. In practice we measure both an
in-phase and an out-of-phase component. Each of these curves will look like
the basic curve (given above). We need only establish relative amplitude. From
the general response curve we find that the in-phase (or real component) is
larger than the out-of-phase (imaginary) component when :math:`\omega \sigma`
(or :math:`\omega L / R`) is large.

Below we plot the responses for a horizontal loop survey taken over a vertical
conductive plate in which:

1.  strike length of the plate: S = 1.0 units
2.  width of the plate W= 0.5 units (length in vertical extent)
3.  depth of burial Z=0.13 units
4.  L=distance between source and transmitter coil L=0.76 units (Z/L=0.17)
5.  conductivity-thickness product = 1.0

Because the body is conductive and the frequency of the survey is high, the
value of :math:`\omega L / R` is large and the in-phase response is larger than
the quadrature response.

.. figure:: ./images/dipole_response.jpg
    :align: center
    :scale: 80 %


Conductive Host
===============

The sketches regarding EM responses were derived under the simplifying
assumptions that the buried body was in a very resistive medium. Consequently,
the response depended only upon the relative orientations of the source coil
and the body (the coupling effect), the conductivity of the body and the
frequency of the transmitter, and the coupling effect of the secondary
magnetic fields with the receiver.

In more realistic situations the object of interest in buried in a conductive
medium.

.. figure:: ./images/buried_object.jpg
    :align: center
    :scale: 80 %

The laws of EM induction require that there be eddy currents that are also set
up in the host. But any conductive material in which currents are flowing is a
"lossy" medium. That is, there are :math:`I^2R` losses which convert the
electromagnetic energy to heat. As a consequence the energy from the source
does not propagate to arbitrarily large depths in the earth. The amplitude of
the EM fields thus decrease due to geometrical spreading and attenuation.
