


--- pic\Double integrals over non-rectangular regions.pdf_01.png ---
The trouble with non-rectangular regions

Consider the function

f(x,y) = xy? Its graph looks like this:

Graph of xy42

See video transcript

We will find the volume under a portion of this graph. Unlike the last article,
this volume will not lie above a rectangular region on the xy-plane. Instead, we
will look for a volume whose base is a triangle. The triangle pictured below, to
be specific.

--- pic\Double integrals over non-rectangular regions.pdf_02.png ---
This is a right isosceles triangle, one of whose legs connects the points (0, 0)
and (2,0) on the x-axis, while the other leg connects the points (2,0) and
(2,2). The volume above this triangle and below the graph of f(z, y) = zy”
looks like this:

Volume under xy*2 bounded by triangle

4

See video transcript

This is similar to the problem | showed in the last article, which introduced the
double integral. And indeed, the way to solve it is similar. Find a formula for slices of area using an integral. Use a second integral to add those infinitely many slices of area into a
volume. What gets tricky now is the bounds. For example, consider the slices of this
volume which represent constant z values. The following animation shows
what these slices look like, as the constant z-value varies back and forth
between 0 and 2.

--- pic\Double integrals over non-rectangular regions.pdf_03.png ---
The height of one of these slices changes based the height of the graph of
f(x,y) = zy’ above its base. But the length of the base of the slice also
changes. For example, when x = 0. Alternatively, when zx = 1. This means when we set up an integral to find the area of one of these
constant-z-value slices, the upper bound is written in terms of z.

--- pic\Double integrals over non-rectangular regions.pdf_04.png ---
As far as our computations are concerned, it's perfectly fine to have one of the
bounds written in terms of x. After all, we'll end up with an expression in terms
of x anyway. Go ahead and work out the integral for yourself:

i ry” dy =
0

Check

[Hide explanation]

Remember, in the eyes of the integral, x is a constant, since it is an integral
with respect to y (as indicated by the "dy"). From here, there is nothing new. Multiply this value by dz to give it a little
depth, and hence make it an infinitesimal volume. Then when we integrate it
with respect to z, the bounds are constants, z = 0 and x = 2, since this Is
where the base of our triangle sits on the z-axis. The total volume is therefore = ~ 2. Integrating over a disk

Now let's try something a little harder: finding the volume under a graph
bounded by the unit disk.

--- pic\Double integrals over non-rectangular regions.pdf_05.png ---
For example, the volume underneath the graph

f(x,y) =3+y-2°

bound by the unit disk looks like this

Volume between 3+y-x‘2 and unit disk

4

See video transcript

Once again, consider slices of this volume which correspond to constant z-
values. Slices of area under 3+y-x*2 over unit disk

4

_ >

See video transcript

Think about what the base of each of these slices looks like on the xy-plane. Each slice corresponds with some vertical stripe in the unit disk.

--- pic\Double integrals over non-rectangular regions.pdf_06.png ---
Using the pythagorean theorem, we can find the y-values which determine the
top and bottom of this stripe as a function of the z-value that the stripe
represents. We can now find the area of one of these constant-z-value slices by
integrating f(z, y) with respect to y. Again, where this is different from the
case of rectangular regions is that the bounds are each a function of z. Concept check: Which of the following integrals represents the area of a
constant-z-value slice of the volume we are looking for?

--- pic\Double integrals over non-rectangular regions.pdf_07.png ---
Vie? V1-2? Hide explanation]

The first choice Is correct:

V1—«? In this integral, z should be thought of as a constant. The height of the slice at each point (as a function of y) is f(z, y) =3+y— 2’. The bounds for the y-value at the base of the slice are what we just found

geometrically:

y= —V1-2? Work through it: This is a heavier computation than previous examples, but if
you feel up to it, compute this integral to get a formula for the area of a
constant-z-value slice, as a function of z.

--- pic\Double integrals over non-rectangular regions.pdf_08.png ---
Vinw? J/1— 72)
= (svinws OS) Avi-#)

The x-values in the unit disk range from z = —1 to z = 1, so to find the
volume we are looking for, integrate the expression you just found with
respect to x between the value —1 and 1. As before, you can imagine this as
adding up many, many paper-thin volumes. This turns out to be a tricky integral, but for pragmatism's sake we can solve it
using any ol' computer algebra system or numerical integration tool, such as
Wolfram Alpha. Total volume: / (6 — 227)V/1-— 2? Slice the other way: Shark fin region

Sometimes it's easier to consider constant-y-value slices, which involves
cutting your region in xy-plane along horizontal stripes.

--- pic\Double integrals over non-rectangular regions.pdf_09.png ---
This region kind of looks like a shark's dorsal fin:

The upper right corner of the region is where the curve z = y* meets the line
x = y + 2. That point is (4, 2). Let's find the volume of a solid that has this region as its footprint, and whose
height is determined by a relatively simple multivariable function:

f(x,y) = a+ 2y

Here's what the volume looks like:

Volume over shark fin\fegion ©
aye

See video transcript

This time, imagine cutting constant-y-value slices of this volume.

--- pic\Double integrals over non-rectangular regions.pdf_10.png ---
Concept check: If one of these horizontal stripes corresponds to a value y,
what are the bounds on the z-value of the stripe? That is, what are the z-
coordinates of the left and right ends of this line as a function of y? Lower bound: zx =

Upper bound: xz =

Check

[Hide explanation]

Lower bound: z = y’
Upper bound: xz = y + 2

These come directly from the definition of the region given above. Concept check: Which of the following integrals represents the slice of area
above one of these stripes, and under the graph of f(z, y) = x+ 2y, asa

function of y?

--- pic\Double integrals over non-rectangular regions.pdf_11.png ---
Hide explanation]

The first choice is correct. The integration moves horizontally, as indicated by the "dz". It is also
bounded by the values found in the last question, indicated that it
stays within the shark fin region. Concept check: Solve this integral to find the area of the constant y-value
slices of our volume. Area of constant-y-value slice: |

[Hide explanation]

aut? Factor out 1 / 2

(y? By? Re

Concept check: When we integrate this function of y to get the total volume,
what bounds should we use?

--- pic\Double integrals over non-rectangular regions.pdf_12.png ---
Choose 1 answer:

® [ney

[ot

Check

[Hide explanation]

Looking at the picture of our shark fin region, y varies from 0 to 2

Therefore, the second choice is correct. The integral giving our desired
volume looks like this:

2
1
i 5 (—y* — dy? By? Bring it on home: Solve this integral to find the volume of the region defined
at the start of this section. Feel free to use a calculator).

--- pic\Double integrals over non-rectangular regions.pdf_13.png ---
Ay” + 5y" + 12y + 4) dy
0

5 3 -
=> (Ey 54 + Gy? Lip
15
Summary

When you need to perform a double integral over a non-rectangular region,
follow these steps. Start by cutting your region along slices that correspond with holding one
of the variables constant. For example, holding xz at some constant value
will give a vertical stripe of your region. Find how to express the bounds of these stripes as a function of the other
variable. For example, the top and bottom of a vertical stripe would be
expressed as some function of z. When you set up your double integral, the inner integral will correspond to
integrating along one of these stripes, and each of its bounds will be a
function of the outer variable.

--- pic\Double integrals over non-rectangular regions.pdf_14.png ---


