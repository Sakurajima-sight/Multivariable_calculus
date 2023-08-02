--- pic\Stokes' theorem examples.pdf_00.png ---
Stokes' theorem examples
因 Google Classroom
See how Stokes' theorem is used in practice.
Background
- Stokes' theorem
- Line integrals
- Flux in 3D
- $\underline{\text { Curl }}$
The formula (quick review)
Stokes' theorem is a tool to turn the surface integral of a curl vector field into a line integral around the boundary of that surface, or vice versa. Specifically, here's what it says:
Let's go through each term:




--- pic\Stokes' theorem examples.pdf_01.png ---
- $\mathbf{F}(x, y, z)$ is a three-dimensional vector field.
- $\operatorname{curl} \mathbf{F}$, also often written as $\nabla \times \mathbf{F}$. It is the three-dimensional curl of $\mathbf{F}$, which is a vector field.
- $S$ is a surface in three dimensions.
- $\hat{\mathbf{n}}$ represents a function that gives unit normal vectors to $S$.
- $C$ is the boundary of $S$.
- $C$ is oriented using the right-hand rule, meaning if you point the thumb of your right hand in the direction of a unit normal vector $\hat{n}$ near the edge of $S$ and curl your fingers, the direction they point indicates the direction you should integrate around $C$.

Example 1: From a surface integral to line integral
Problem
Let $S$ be the half of a unit sphere centered at the origin that is above the $x y$ plane, oriented with outward facing unit normal vectors. Let $\overrightarrow{\mathbf{v}}(x, y, z)$ be the vector field defined as follows:
$$
\overrightarrow{\mathbf{v}}(x, y, z)=y \hat{\mathbf{i}}
$$
Compute the following surface integral:
$$
\iint_S \overrightarrow{\mathbf{v}} \cdot d \Sigma
$$
[Hide explanation].




--- pic\Stokes' theorem examples.pdf_02.png ---

Whenever people talk about taking a surface integral of a vector field, this always means taking the dot product with the unit normal vector to that surface:
$$
\iint_S(\overrightarrow{\mathbf{v}} \cdot \hat{\mathbf{n}}) d \Sigma
$$
So really, this is a surface integral of a scalar-valued function, but that scalar value arises as the dot product between two vector-valued functions: $(\overrightarrow{\mathbf{v}} \cdot \hat{\mathbf{n}})$
This is so universal that it often goes without saying that the unit normal vector is involved, so people instead drop the $\hat{\mathbf{n}}$ and write this:
$$
\iint_S \overrightarrow{\mathbf{v}} \cdot d \Sigma
$$
Solution
Remember, Stokes' theorem relates the surface integral of the curl of a function to the line integral of that function around the boundary of the surface. This means we will do two things:
- Step 1: Find a function whose curl is the vector field $y \hat{\mathbf{i}}$



--- pic\Stokes' theorem examples.pdf_03.png ---

- Step 2: Take the line integral of that function around the unit circle in the $x y$-plane, since this circle is the boundary of our half-sphere.

Concept check: Find a vector field $\mathrm{F}(x, y, z)$ satisfying the following property:
$$
\nabla \times \mathbf{F}=y \hat{\mathbf{i}}
$$
There are multiple ways to do this, but one in particular will make our lives easiest. In the one I'm thinking of, the $\hat{\mathbf{i}}$ and $\hat{\mathbf{j}}$ components are 0 , while the $\hat{\mathbf{k}}$ component is non-zero. Can you find it?
$$
\mathbf{F}(x, y, z)=0 \hat{\mathbf{i}}+0 \hat{\mathbf{j}}+\square \hat{\mathbf{k}}
$$
Check
[Hide explanation].
First things first, let's write out how curl is computed. Suppose $F_1, F_2$, and $F_3$ represent the coordinate functions of our vector-valued function:
$$
\mathbf{F}(x, y, z)=F_1(x, y, z) \hat{\mathbf{i}}+F_2(x, y, z) \hat{\mathbf{j}}+F_3(x, y, z) \hat{\mathbf{k}}
$$
Then curl is computed with the following determinant trick:
$$
\begin{aligned}
& \left|\begin{array}{ccc}
\hat{\mathbf{i}} & \hat{\mathbf{j}} & \hat{\mathbf{k}} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
F_1 & F_2 & F_3
\end{array}\right| \\
& =\left(\frac{\partial F_3}{\partial y}-\frac{\partial F_2}{\partial z}\right) \hat{\mathbf{i}}+\left(\frac{\partial F_1}{\partial z}-\frac{\partial F_3}{\partial x}\right) \hat{\mathbf{j}}+\left(\frac{\partial F_2}{\partial x}-\frac{\partial F_1}{\partial y}\right) \hat{\mathbf{k}}
\end{aligned}
$$
We want this whole expression to equal the simple vector field $\overrightarrow{\mathbf{v}}(x, y, z)=y \hat{\mathbf{i}}$. This means we need the following equality:
$$
\left(\frac{\partial F_3}{\partial y}-\frac{\partial F_2}{\partial z}\right)=y
$$
There are many pairs of functions $F_2$ and $F_3$ that will make this equality work. Given how I phrased the question above, though, we want $F_2$ to be 0 .



--- pic\Stokes' theorem examples.pdf_04.png ---

This means the term $\frac{\partial F_3}{\partial y}$ must take care of the entire equation. To do this, take the antiderivative of $y$, the function on the right-hand-side, with respect to the variable $y$ :
$$
F_3(x, y, z)=\frac{1}{2} y^2
$$
When you set the other two components equal to 0 , you can check the original curl expression to see that $\nabla \times \mathbf{F}=y \hat{\mathbf{i}}$ as desired.
[Hide explanation].
Given that you can find many different functions satisfying the property $\nabla \times \mathbf{F}=y \hat{\mathbf{i}}$, how do you know which one to choose?
To start, we want something as simple as possible, so if you can make all but one component 0 , do it.

From the answer explanation, though, you might have noticed that we could also have chosen a function where only $F_2$ is nonzero, so why not use that? Although it would be fine to use that other function, when you consider the fact that we will ultimately be performing a line integral over the unit circle in the $x y$-plane, having a function with only a $\hat{\mathbf{k}}$-component will make things even simpler.

The surface $S$ is defined to be the portion of the unit sphere above the $x y$ plane. The boundary of this hemisphere is the unit circle on the $x y$-plane.



--- pic\Stokes' theorem examples.pdf_05.png ---

Concept check: Both of the following parameterize the unit circle on the $x y$ plane, but each with a different orientation. Which one corresponds with the orientation of the hemisphere above the $x y$-plane with outward-facing unit normal vectors? ("Correspond" in the sense that we can apply Stokes' theorem.)
Choose 1 answer:
(A) $\left[\begin{array}{c}\cos (t) \\ \sin (t) \\ 0\end{array}\right]$, where $0 \leq t \leq 2 \pi$
(B) $\left[\begin{array}{c}\cos (t) \\ -\sin (t) \\ 0\end{array}\right]$, where $0 \leq t \leq 2 \pi$
Check
[Hide explanation].
The first answer choice is correct:
$$
\left[\begin{array}{c}
\cos (t) \\
\sin (t) \\
0
\end{array}\right] \text {, where } 0 \leq t \leq 2 \pi
$$
This corresponds to a counterclockwise orientation of the circle.
Surfaces are oriented by the chosen direction for their unit normal vectors, and curves are oriented by the chosen direction for their tangent vectors. In order to apply Stokes' theorem, the orientation of a surface and its boundary must "line up" in the right way. Here are several different, but equivalent, ways to phrase how that alignment must look:



--- pic\Stokes' theorem examples.pdf_06.png ---
- If you look at the surface in such a way that the unit normal vectors are all pointed towards your face, the curve should be oriented counterclockwise.
- The curve's orientation should follow the right-hand rule, in the sense that if you stick the thumb of your right hand in the direction of a unit normal vector near the edge of the surface, and curl your fingers, the direction they point on the curve should match its orientation.
- When you are walking along the boundary curve with your body pointing out in the direction of the unit normal vector, you should be walking in such a way that the surface is to your left side.
If you apply any of these images to our specific example, you will see that a counterclockwise orientation of the unit circle "aligns" with outward facing unit normal vectors for the hemisphere.

Concept check: Let $C$ represent the boundary of the surface $S$. Use the parameterization of $C$ that you just chose, together with the definition of $\mathbf{F}$ that you found in the question before that, to solve the following line integral.
$$
\oint_C \mathbf{F} \cdot d \mathbf{r}=
$$
Check
[Hide explanation].
$$
\mathbf{F}(x, y, z)=\frac{1}{2} y^2 \hat{\mathbf{k}}
$$
[Hide explanation].




--- pic\Stokes' theorem examples.pdf_07.png ---

You actually don't need to dive into any computations once you think about what this integral means. Take a look at $\mathbf{F}(x, y, z)$ :
$$
\mathbf{F}(x, y, z)=\frac{1}{2} y^2 \hat{\mathbf{k}}
$$
Most notably, it only has a $\hat{\mathbf{k}}$-component, so all the vectors are perpendicular to the $x y$-plane. Since the curve $C$ resides completely in the $x y$-plane, all the little tangent vectors $d \mathbf{r}$ will be contained on the $x y$-plane. Therefore, the dot product $\mathbf{F} \cdot d \mathbf{r}$ in the line integral will always be 0 , so the line integral as a whole is just 0 .
Of course, this is a fact you could have recognized even earlier in the problem, before parameterizing the circle. However, I wanted an excuse to let you practice thinking about matching up the orientation of a surface's boundary with the surface itself, since that is an easy thing to accidentally mess up in a Stokes' theorem problem.
Example 2: Wind through a butterfly net
Problem
Suppose you have a butterfly net with a square-shaped rim, and the wind is blowing through the net. Think about the square rim positioned in space on the $y z$-plane such that its four corners are at the following four points:
$$
\left[\begin{array}{l}
0 \\
1 \\
1
\end{array}\right] \quad\left[\begin{array}{c}
0 \\
-1 \\
1
\end{array}\right] \quad\left[\begin{array}{c}
0 \\
-1 \\
-1
\end{array}\right] \quad\left[\begin{array}{c}
0 \\
1 \\
-1
\end{array}\right]
$$
Furthermore, let the net be some surface emerging from this rim in the positive $x$-direction.



--- pic\Stokes' theorem examples.pdf_08.png ---
Suppose the velocity vector field for the wind is given by the following function:
$$
\mathbf{F}=\left[\begin{array}{c}
y^2 \\
z^2 \\
x^2
\end{array}\right]
$$
Assuming the air has a uniform density of $1 \mathrm{~kg} / \mathrm{m}^3$, how much air passes through your net per unit time? Specifically, suppose air going from the inside of the net to the outside counts positively towards this sum, and air going from the outside to the inside counts negatively.
Step 1: Dissecting the question
Before anything, we need to compose our thoughts and piece together how this physics-sounding problem is a Stokes' theorem question.
Concept check: What is this question really asking about?
Choose 1 answer:




--- pic\Stokes' theorem examples.pdf_09.png ---

(A) The flux of $\mathrm{F}$ through the surface of the butterfly net.
(B) The line integral of $\mathbf{F}$ around the specified square in the $y z-$ plane.
Check
[Hide explanation].
This is a flux problem, since it is asking how much fluid passes through a surface, given the velocity vector field of that fluid. See this article on 3D flux if that feels unfamiliar.

Concept check: More specifically, which of the following integrals represents the answer to the question? Let $S$ denote the surface of the butterfly net, while $C$ is the square rim of that net sitting in the $y z$-plane.
Choose 1 answer:
(A) $\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) d \Sigma$, where $\hat{\mathbf{n}}$ represents outward-facing unit normal vectors.
(B) $\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) d \Sigma$, where $\hat{\mathbf{n}}$ represents inward-facing unit normal vectors.
(c) $\int_C \mathbf{F} \cdot d \mathbf{r}$, where $C$ is oriented counterclockwise.
(D) $\int_C \mathbf{F} \cdot d \mathbf{r}$, where $C$ is oriented clockwise.
Check
[Hide explanation].



--- pic\Stokes' theorem examples.pdf_10.png ---
The rate at which air passes through the net, in terms of volume per unit time, is given by the following flux integral:
$$
\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) d \Sigma
$$
Since the assumption is that air has uniform density $1 \mathrm{~kg} / \mathrm{m}^3$, this also gives the mass of air passing through the net per unit time.
To capture the idea that air going from the inside of the net to the outside counts positively toward flux, while air going from the outside counts negatively towards flux, the unit normal vectors $\hat{\mathbf{n}}$ must be outward-facing. This way, the dot product $\mathbf{F} \cdot \hat{\mathbf{n}}$ will be positive at points where the air's trajectory is outward, and negative when it is inward.
Again, if this feels unfamiliar, feel free to review the article on 3D flux.
Really, this is all just a way to give a physical interpretation to a surface integral through a vector field.
Step 2: Applying Stokes' theorem
What might feel weird about this problem, and what suggests that you will need Stokes' theorem, is that the surface of the net is never defined! All that is given is the boundary of that surface: A certain square in the $y z$-plane.

If we can find a way to express $\mathbf{F}(x, y, z)$ as the curl of some other vector field, say $\mathbf{G}(x, y, z)$, we will be able to apply Stokes' theorem to this problem as follows:
$$
\underbrace{\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) \cdot d \Sigma}_{\text {Target flux integral }}=\underbrace{\iint_S(\nabla \times \mathbf{G}) \cdot \hat{\mathbf{n}} d \Sigma=\int_C \mathbf{G} \cdot d \mathbf{r}}_{\text {Stokes' theorem }}
$$
This is analogous to performing the integral $\int f(x) d x$ in single-variable calculus, where you have to find a new function with the property $g^{\prime}(x)=f(x)$, which then lets you compute the integral based on the boundary values. In this case, we are looking for the "anti-curl" of $\mathbf{F}$, so to speak, which will let us compute the surface integral based on the values of this anti-curl function on the boundary of the surface.




--- pic\Stokes' theorem examples.pdf_11.png ---
Unlike single-variable calculus, not all vector fields $\mathbf{F}$ have such an anti-curl function. Luckily for us, this particular function is one of the special ones that do.
$$
\mathbf{F}=\left[\begin{array}{c}
y^2 \\
z^2 \\
x^2
\end{array}\right]
$$
Concept check: Find a vector field $\mathbf{G}(x, y, z)$ satisfying the property $\nabla \times \mathbf{G}=\mathbf{F}$.
$\mathbf{G}(x, y, z)=$ $\hat{\mathbf{i}}+$ $\hat{\mathbf{j}}+$ $\hat{\mathbf{k}}$
Check
[Hide explanation].
Let $G_1, G_2$ and $G_3$ be the component function of $\mathbf{G}$ :
$$
\mathbf{G}(x, y, z)=G_1(x, y, z) \hat{\mathbf{i}}+G_2(x, y, z) \hat{\mathbf{j}}+G_3(x, y, z) \hat{\mathbf{k}}
$$
Next, just write out the definition of curl:
$$
\begin{aligned}
& \left|\begin{array}{ccc}
\hat{\mathbf{i}} & \hat{\mathbf{j}} & \hat{\mathbf{k}} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
G_1 & G_2 & G_3
\end{array}\right| \\
& =\left(\frac{\partial G_3}{\partial y}-\frac{\partial G_2}{\partial z}\right) \hat{\mathbf{i}}+\left(\frac{\partial G_1}{\partial z}-\frac{\partial G_3}{\partial x}\right) \hat{\mathbf{j}}+\left(\frac{\partial G_2}{\partial x}-\frac{\partial G_1}{\partial y}\right) \hat{\mathbf{k}}
\end{aligned}
$$
Bringing in the definition of $\mathbf{F}$, this means the desired property that $\nabla \times \mathbf{G}=\mathbf{F}$ breaks down into the following three equations:
$$
\begin{aligned}
& \frac{\partial G_3}{\partial y}-\frac{\partial G_2}{\partial z}=y^2 \\
& \frac{\partial G_1}{\partial z}-\frac{\partial G_3}{\partial x}=z^2 \\
& \frac{\partial G_2}{\partial x}-\frac{\partial G_1}{\partial y}=x^2
\end{aligned}
$$




--- pic\Stokes' theorem examples.pdf_12.png ---
Solving this is like solving a puzzle. You try some things, tweak them when they don't work, attempting all the while to keep things simple. After playing around a bit, you might find that the simplest strategy is as follows: Let $G_3$ take care of the entire first equation, $G_1$ take care of the entire second equation, and $G_2$ take care of the last equation. Specifically:
$$
\begin{aligned}
& G_3=\frac{1}{3} y^3 \\
& G_1=\frac{1}{3} z^3 \\
& G_2=\frac{1}{3} x^3
\end{aligned}
$$
Or, written in the format requested in the question:
$$
\mathbf{G}(x, y, z)=\frac{1}{3} z^3 \hat{\mathbf{i}}+\frac{1}{3} x^3 \hat{\mathbf{j}}+\frac{1}{3} y^3 \hat{\mathbf{k}}
$$
In a sense, we were lucky with this example, since there was enough symmetry that things didn't get complicated. In general, equations that are expressed using partial derivatives of a function can be very hard to solve. As in, one of them currently has a million dollar prize attached to it. The study of these sorts of equations goes under the name "Partial differential equations", which of course involves more sophisticated tactics than the guess-and-check approach I suggested for this one.>
$$
\begin{aligned}
& \frac{\partial G_3}{\partial y}-\frac{\partial G_2}{\partial z}=y^2 \\
& \frac{\partial G_1}{\partial z}-\frac{\partial G_3}{\partial x}=z^2 \\
& \frac{\partial G_2}{\partial x}-\frac{\partial G_1}{\partial y}=x^2
\end{aligned}
$$
Step 3: Compute the line integral
Given this construction for $\mathbf{G}$, the final step is to compute the right-hand-side line integral in our core equation:
$$
\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) \cdot d \Sigma=\iint_S(\nabla \times \mathbf{G}) \cdot \hat{\mathbf{n}} d \Sigma=\overbrace{\int_C \mathbf{G} \cdot d \mathbf{r}}^{\text {Compute this guy now. }}
$$




--- pic\Stokes' theorem examples.pdf_13.png ---

Target flux integral
Stokes' theorem
In this context, the curve $C$ represents the $2 \times 2$ square in the $y z$-plane with vertices at the following four points:
$$
\left[\begin{array}{l}
0 \\
1 \\
1
\end{array}\right] \quad\left[\begin{array}{c}
0 \\
-1 \\
1
\end{array}\right] \quad\left[\begin{array}{c}
0 \\
-1 \\
-1
\end{array}\right] \quad\left[\begin{array}{c}
0 \\
1 \\
-1
\end{array}\right]
$$
Before computing the line integral around this square, it needs to be oriented in a way that aligns with the orientation of the butterfly net surface $S$.
Concept check: Given that the butterfly net lies in the positive $x$-direction away from the square $C$, and is oriented with outward-facing unit normal vectors, how should $C$ be oriented so that Stokes' theorem can be applied? Answer this question from the perspective of standing on the positive $x$-axis, and looking directly at $C$.
Choose 1 answer:
(A) Clockwise



--- pic\Stokes' theorem examples.pdf_14.png ---
(B) Counterclockwise
Check
[Hide explanation].
Counterclockwise.
As I mentioned in the answer to a similar question in the last example, there are several different ways to phrase the rule for this oritentationalignment.
- If you look at the surface in such a way that the unit normal vectors are all pointed towards your face, the curve should be oriented counterclockwise.
- The curve's orientation should follow the right-hand rule, in the sense that if you stick the thumb of your right hand in the direction of a unit normal vector near the edge of the surface, and curl your fingers, the direction they point on the curve should match its orientation.
- When you are walking along the boundary curve with your body pointing out in the direction of the unit normal vector, you should be walking in such a way that the surface is to your left side.
Concept check: Our construction of $\mathbf{G}$ looks like this:
$$
\mathbf{G}=\frac{1}{3}\left[\begin{array}{c}
z^3 \\
x^3 \\
y^3
\end{array}\right]
$$
Given this, and given the orientation of the square $C$ that you just specified, finish the problem by computing the following line integral:
$$
\int_C \mathbf{G} \cdot d \mathbf{r}=
$$
Check
[Hide explanation].




--- pic\Stokes' theorem examples.pdf_15.png ---

First, draw out the square with its designated counterclockwise orientation in the $y z$-plane.
Now think about the following line integral along each one of these sides:
$$
\int \frac{1}{3}\left[\begin{array}{c}
z^3 \\
x^3 \\
y^3
\end{array}\right] \cdot d \mathbf{r}
$$
- Right side: While going up the right side, the tiny step vector $d \mathbf{r}$ is a step up in the $z$-direction.
$$
d \mathbf{r}=\left[\begin{array}{c}
0 \\
0 \\
d z
\end{array}\right]
$$
Here's what this means for the integral:
$$
\int \frac{1}{3}\left[\begin{array}{c}
z^3 \\
x^3 \\
y^3
\end{array}\right] \cdot\left[\begin{array}{c}
0 \\
0 \\
d z
\end{array}\right]=\int \frac{1}{3} y^3 d z
$$
This integral is taken along the right side of the square, where the value of $y$ is constantly 1 , and $z$ has the bounds $z=-1$ and $z=1$. So our integral simplifies to this:
$$
\int_{-1}^1 \frac{1}{3}(1)^3 d z=\frac{2}{3}
$$



--- pic\Stokes' theorem examples.pdf_16.png ---

- Top side: When going left on the top side, the tiny step vector is
$$
d \mathbf{r}=\left[\begin{array}{c}
0 \\
-d y \\
0
\end{array}\right]
$$
Since this line ranges from the values $y=-1$ to $y=1$, this means the line integral on this portion of the square becomes:
$$
\int_{-1}^1-\frac{1}{3} x^3 d y
$$
Since $x$ is zero on this whole line (or the whole square for that matter), this integral is 0 .
- Left side: Almost identical to the right side, except that $d z$ is negative and the constant value of $y$ is negative. These differences cancel out, so the integral on this side also ends up being $\frac{2}{3}$.
- Bottom side: Almost identical to the top side. It also becomes 0 .
All in all, then, the line integral adds up to $\frac{4}{3}$.
Summary
- Stokes' theorem can be used to turn surface integrals through a vector field into line integrals.
- This only works if you can express the original vector field as the curl of some other vector field.
- Make sure the orientation of the surface's boundary lines up with the orientation of the surface itself.



