# DoublePendulum

## Kinematics of the Double Pendulum

double pendulum variables
Kinematics means the relations of the parts of the device, without regard to forces. In kinematics we are only trying to find expressions for the position, velocity, and acceleration in terms of the variables that specify the state of the device.

x = horizontal position of pendulum mass
y = vertical position of pendulum mass
θ = angle of pendulum (0 = vertical downwards, counter-clockwise is positive)
L = length of rod (constant)
We place the origin at the pivot point of the upper pendulum. We regard y as increasing upwards. We indicate the upper pendulum by subscript 1, and the lower by subscript 2. Begin by using simple trigonometry to write expressions for the positions x1, y1, x2, y2 in terms of the angles θ1, θ2 .

    x1 = L1 sin θ1
    y1 = −L1 cos θ1

    x2 = x1 + L2 sin θ2
    y2 = y1 − L2 cos θ2

The velocity is the derivative with respect to time of the position.

    x1' = θ1' L1 cos θ1
    y1' = θ1' L1 sin θ1

    x2' = x1' + θ2' L2 cos θ2
    y2' = y1' + θ2' L2 sin θ2

The acceleration is the second derivative.

x1'' = −θ1'2 L1 sin θ1 + θ1'' L1 cos θ1 (1)
y1'' = θ1'2 L1 cos θ1 + θ1'' L1 sin θ1 (2)
x2'' = x1'' − θ2'2 L2 sin θ2 + θ2'' L2 cos θ2 (3)
y2'' = y1'' + θ2'2 L2 cos θ2 + θ2'' L2 sin θ2 (4)

## Forces in the Double Pendulum

We treat the two pendulum masses as point particles. Begin by drawing the free body diagram for the upper mass and writing an expression for the net force acting on it. Define these variables:

    T = tension in the rod
    m = mass of pendulum
    g = gravitational constant

The forces on the upper pendulum mass are the tension in the upper rod T1 , the tension in the lower rod T2 , and gravity −m1 g . We write separate equations for the horizontal and vertical forces, since they can be treated independently. The net force on the mass is the sum of these. Here we show the net force and use Newton's law F = m a .

m1 x1'' = −T1 sin θ1 + T2 sin θ2 (5)
m1 y1'' = T1 cos θ1 − T2 cos θ2 − m1 g (6)
For the lower pendulum, the forces are the tension in the lower rod T2 , and gravity −m2 g .

m2 x2'' = −T2 sin θ2 (7)
m2 y2'' = T2 cos θ2 − m2 g (8)
In relating these equations to the diagrams, keep in mind that in the example diagram θ1 is positive and θ2 is negative, because of the convention that a counter-clockwise angle is positive.

## Direct Method for Finding Equations of Motion

Now we do some algebraic manipulations with the goal of finding expressions for θ1'', θ2'' in terms of θ1, θ1', θ2, θ2' . Begin by solving equations (7), (8) for T2 sin θ2 and T2 cos θ2 and then substituting into equations (5) and (6).

    m1 x1'' = −T1 sin θ1 − m2 x2''	            (9)
    m1 y1'' = T1 cos θ1 − m2 y2'' − m2 g − m1 g	(10)

Multiply equation (9) by cos θ1 and equation (10) by sin θ1 and rearrange to get

T1 sin θ1 cos θ1 = −cos θ1 (m1 x1'' + m2 x2'') (11)
T1 sin θ1 cos θ1 = sin θ1 (m1 y1'' + m2 y2'' + m2 g + m1 g) (12)
This leads to the equation

sin θ1 (m1 y1'' + m2 y2'' + m2 g + m1 g) = −cos θ1 (m1 x1'' + m2 x2'') (13)
Next, multiply equation (7) by cos θ2 and equation (8) by sin θ2 and rearrange to get

T2 sin θ2 cos θ2 = −cos θ2 (m2 x2'') (14)
T2 sin θ2 cos θ2 = sin θ2 (m2 y2'' + m2 g) (15)
which leads to

sin θ2 (m2 y2'' + m2 g) = −cos θ2 (m2 x2'') (16)
Next we need to use a computer algebra program to solve equations (13) and (16) for θ1'', θ2'' in terms of θ1, θ1', θ2, θ2' . Note that we also include the definitions given by equations (1-4), so that we have 2 equations (13, 16) and 2 unknowns ( θ1'', θ2'' ). The result is somewhat complicated, but is easy enough to program into the computer.

<table class="fraction">
    <tbody><tr>
        <td rowspan="2">
            <i>θ</i><sub>1</sub>''&nbsp;=&nbsp;
        </td><td>
            −<i>g</i> (2 <i>m</i><sub>1</sub> + <i>m</i><sub>2</sub>) sin <i>θ</i><sub>1</sub> − <i>m</i><sub>2</sub> <i>g</i> sin(<i>θ</i><sub>1</sub> − 2 <i>θ</i><sub>2</sub>) −
            2 sin(<i>θ</i><sub>1</sub> − <i>θ</i><sub>2</sub>) <i>m</i><sub>2</sub> (<i>θ</i><sub>2</sub>'<sup>2</sup> <i>L</i><sub>2</sub> + <i>θ</i><sub>1</sub>'<sup>2</sup> <i>L</i><sub>1</sub> cos(<i>θ</i><sub>1</sub> − <i>θ</i><sub>2</sub>))
        </td>
    </tr><tr>
        <td class="upper_line">
            <i>L</i><sub>1</sub> (2 <i>m</i><sub>1</sub> + <i>m</i><sub>2</sub> − <i>m</i><sub>2</sub> cos(2 <i>θ</i><sub>1</sub> − 2 <i>θ</i><sub>2</sub>))
        </td>
    </tr>
</tbody></table>

<table class="fraction">
    <tbody><tr>
        <td rowspan="2">
            <i>θ</i><sub>2</sub>''&nbsp;=&nbsp;
        </td><td>
            2 sin(<i>θ</i><sub>1</sub> − <i>θ</i><sub>2</sub>) (<i>θ</i><sub>1</sub>'<sup>2</sup> <i>L</i><sub>1</sub> (<i>m</i><sub>1</sub> + <i>m</i><sub>2</sub>) + <i>g</i>(<i>m</i><sub>1</sub> + <i>m</i><sub>2</sub>) cos <i>θ</i><sub>1</sub>
            + <i>θ</i><sub>2</sub>'<sup>2</sup> <i>L</i><sub>2</sub> <i>m</i><sub>2</sub> cos(<i>θ</i><sub>1</sub> − <i>θ</i><sub>2</sub>))
        </td>
    </tr><tr>
        <td class="upper_line">
            <i>L</i><sub>2</sub> (2 <i>m</i><sub>1</sub> + <i>m</i><sub>2</sub> − <i>m</i><sub>2</sub> cos(2 <i>θ</i><sub>1</sub> − 2 <i>θ</i><sub>2</sub>))
        </td>
    </tr>
</tbody></table>
These are the equations of motion for the double pendulum.

Text copied from https://www.myphysicslab.com/pendulum/double-pendulum-en.html
