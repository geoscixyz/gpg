.. _principles_of_em_induction:

Principles of Electromagnetic (EM) Induction
********************************************

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