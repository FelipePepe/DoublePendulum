# DoublePendulum
## Lagrange Equations

In Lagrangian mechanics, evolution of a system is described in terms of the generalized coordinates and generalized velocities. In our case, the deflection angles of the pendulums <math xmlns="http://www.w3.org/1998/Math/MathML" data-semantic-type="punctuated" data-semantic-role="sequence" data-semantic-id="7" data-semantic-children="2,3,6" data-semantic-content="3" data-semantic-speech="alpha 1 comma alpha 2">
  <mrow data-mjx-texclass="ORD">
    <msub data-semantic-type="subscript" data-semantic-role="greekletter" data-semantic-id="2" data-semantic-children="0,1" data-semantic-parent="7">
      <mi data-semantic-type="identifier" data-semantic-role="greekletter" data-semantic-font="italic" data-semantic-annotation="clearspeak:simple" data-semantic-id="0" data-semantic-parent="2">&#x3B1;</mi>
      <mn data-semantic-type="number" data-semantic-role="integer" data-semantic-font="normal" data-semantic-annotation="clearspeak:simple" data-semantic-id="1" data-semantic-parent="2">1</mn>
    </msub>
  </mrow>
  <mo data-semantic-type="punctuation" data-semantic-role="comma" data-semantic-id="3" data-semantic-parent="7" data-semantic-operator="punctuated">,</mo>
  <mrow data-mjx-texclass="ORD">
    <msub data-semantic-type="subscript" data-semantic-role="greekletter" data-semantic-id="6" data-semantic-children="4,5" data-semantic-parent="7">
      <mi data-semantic-type="identifier" data-semantic-role="greekletter" data-semantic-font="italic" data-semantic-annotation="clearspeak:simple" data-semantic-id="4" data-semantic-parent="6">&#x3B1;</mi>
      <mn data-semantic-type="number" data-semantic-role="integer" data-semantic-font="normal" data-semantic-annotation="clearspeak:simple" data-semantic-id="5" data-semantic-parent="6">2</mn>
    </msub>
  </mrow>
</math> and the angular velocities <math xmlns="http://www.w3.org/1998/Math/MathML" data-semantic-type="punctuated" data-semantic-role="sequence" data-semantic-id="11" data-semantic-children="4,5,10" data-semantic-content="5" data-semantic-speech="ModifyingAbove alpha With dot Subscript 1 Baseline comma ModifyingAbove alpha With dot Subscript 2 Baseline">
  <mrow data-mjx-texclass="ORD">
    <msub data-semantic-type="subscript" data-semantic-role="greekletter" data-semantic-id="4" data-semantic-children="2,3" data-semantic-parent="11">
      <mrow data-mjx-texclass="ORD">
        <mover data-semantic-type="overscore" data-semantic-role="greekletter" data-semantic-id="2" data-semantic-children="0,1" data-semantic-parent="4">
          <mi data-semantic-type="identifier" data-semantic-role="greekletter" data-semantic-font="italic" data-semantic-annotation="clearspeak:simple" data-semantic-id="0" data-semantic-parent="2">&#x3B1;</mi>
          <mo data-semantic-type="operator" data-semantic-role="overaccent" data-semantic-annotation="accent:unknown" data-semantic-id="1" data-semantic-parent="2">&#x2D9;</mo>
        </mover>
      </mrow>
      <mn data-semantic-type="number" data-semantic-role="integer" data-semantic-font="normal" data-semantic-annotation="clearspeak:simple" data-semantic-id="3" data-semantic-parent="4">1</mn>
    </msub>
  </mrow>
  <mo data-semantic-type="punctuation" data-semantic-role="comma" data-semantic-id="5" data-semantic-parent="11" data-semantic-operator="punctuated">,</mo>
  <mrow data-mjx-texclass="ORD">
    <msub data-semantic-type="subscript" data-semantic-role="greekletter" data-semantic-id="10" data-semantic-children="8,9" data-semantic-parent="11">
      <mrow data-mjx-texclass="ORD">
        <mover data-semantic-type="overscore" data-semantic-role="greekletter" data-semantic-id="8" data-semantic-children="6,7" data-semantic-parent="10">
          <mi data-semantic-type="identifier" data-semantic-role="greekletter" data-semantic-font="italic" data-semantic-annotation="clearspeak:simple" data-semantic-id="6" data-semantic-parent="8">&#x3B1;</mi>
          <mo data-semantic-type="operator" data-semantic-role="overaccent" data-semantic-annotation="accent:unknown" data-semantic-id="7" data-semantic-parent="8">&#x2D9;</mo>
        </mover>
      </mrow>
      <mn data-semantic-type="number" data-semantic-role="integer" data-semantic-font="normal" data-semantic-annotation="clearspeak:simple" data-semantic-id="9" data-semantic-parent="10">2</mn>
    </msub>
  </mrow>
</math>
 can be taken as the generalized variables. Using these variables, we construct the Lagrangian for the double pendulum and write the Lagrange differential equations.

A simplified model of the double pendulum is shown in Figure 1.

[![Alt text](https://math24.net/images/double-pendulum1.svg){ width=60%,height:30px }
https://math24.net/images/double-pendulum1.svg


