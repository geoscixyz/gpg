.. _electromagnetic_fields:

Electromagnetic Fields
**********************

Electromagnetic methods are sensitive principally to electrical conductivity
\\(\\sigma\\) (units are S/m or Siemens/meter). We sometimes work with the
inverse of conductivity which is electrical resistivity \\(\\rho\\) which has
units \\(\\Omega m\\) (ohm-meters). Electrical conductivity characterizes the
ease that current flows through the material when an electrical force is
applied. Electric current (units of Amperes) quantifies the amount of charge
that is moving by an observer in one second.

Electrical force can be generated, in two ways:

1. battery (Each terminal of the battery can be thought of as storing a
   positive or negative charge. The "voltage" of the battery is directly
   proportional to the amount of stored charge). Upon completion of the circuit
   there will be an electric field \\(\\vec{E}\\) (volts/m) set up in the body.
   The electric field is a vector: it has both direction and magnitude. The force
   that any charge \\(q\\) feels is given by \\(\\vec{F} = q \\vec{E}\\). Unit
   positive or negative charges will feel the same magnitude of force but
   directions will be opposite. Since like charges repel and unlike charges
   attract, the negative charges will be attracted to the positive terminal of
   the battery and the positive charges will be attracted to the negative
   terminal.
   
.. figure:: ./images/circuit.jpg
    :align: center
    :scale: 100 %

2. A time varying magnetic field can generate or "induce" an electric field in
   a conductor. Consider the simple example of a permanent magnetic moving toward
   a loop of wire. A current is observed and hence there must have been an
   electrical force which has caused the charges to move.

.. figure:: ./images/induced_field.jpg
    :align: center
    :scale: 100 %

In the above example the changing the magnetic field was produced by a moving
magnet. There are other ways in which we can generate a magnetic field. A
current in a wire produces a magnetic field outside the wire. It follows that
a changing magnetic field outside the wire can be achieved by changing the
current in the wire. This can be done by:

a. having the wire connected to a generator which produces a sinusoidal
   current. This leads to Frequency Domain methods.

.. figure:: ./images/sinusoidal_current.jpg
    :align: center
    :scale: 100 %

b. having a steady-state current and then switching it off. This leads to Time
   Domain methods.

.. figure:: ./images/steady_state_current.jpg
    :align: center
    :scale: 100 %

**Magnetic Flux**: In discussing the phenomena of EM induction it is important
to have a concept of magnetic flux. We had previous defined the magnetic flux
density \\(\\vec{B}\\). The magnetic flux \\(\\phi_B\\) which crosses a closed
loop is given by

.. math::
        \phi_B = \int_{area} \vec{B} \cdot \hat{n} \; d\vec{a}

where \\(\\hat{n}\\) is the outward pointing normal vector for the loop.

**Faraday's Law**: A lime varying magnetic field impinging upon a conductor
induces an electromotive force (or voltage) in the conductor.

.. math::
        V = - \frac{d \phi_B}{dt}

This would be the voltage measured in a loop of wire if \\(\\phi_B\\) is the
magnetic flux crossing the wire loop.

**Lens' Law**:The direction of the induced current in the conductor is such
that its magnetic field opposes the changing field across the conductor. That
is, nature does not like to have changing magnetic fields. This is the reason
for the minus sign in the above equation.

Comment: If the input source is a battery or generator which has electrode
terminals connected to the earth then this is called a "grounded" source. It
forms the input for many geophysical experiments (DC resistivity, IP, CSAMT).

If the source is a loop of wire then this is an "inductive source". The EM-31
experiment falls into this category. Inductive experiments are generally less
labor intensive (no electrodes need be pounded into the ground) and they can
be flown in aircraft so large amounts of data can be acquired quickly and
(fairly) cheaply.