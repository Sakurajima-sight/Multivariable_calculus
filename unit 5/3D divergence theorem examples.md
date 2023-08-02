
--- pic\3D divergence theorem examples.pdf_00.png ---

1. 3D divergence theorem examples
   三维散度定理的例子

2. See how to use the $3 d$ divergence theorem to make surface integral problems simpler.
   看看如何使用$3d$散度定理来简化表面积分问题。

3. Background
   背景

4. 3D divergence theorem
   三维散度定理

5. Flux in three dimensions
   三维的通量

6. Divergence
   散度

7. Triple integrals
   三重积分

8. The divergence theorem (quick recap)
   散度定理（快速回顾）

9. Setup:
   设置：

10. $\mathrm{F}(x, y, z)$ is some three-dimensional vector field.
    $\mathrm{F}(x, y, z)$是某个三维矢量场。

11. $V$ is a three-dimensional volume (think of a blob in space).
    $V$是一个三维体积（想象一下空间中的一个斑点）。

12. $S$ is the surface of $V$.
    $S$是$V$的表面。

13. $\hat{\mathbf{n}}$ is a function which gives unit normal vectors on the surface of $S$.
    $\hat{\mathbf{n}}$是一个函数，它在$S$的表面上给出单位法向量。

14. Here's what the divergence theorem states:
    这就是散度定理的内容：
$$
\underbrace{\iiint_V \operatorname{div} \mathbf{F} d V}_{\begin{array}{c}
\text { 在 } V \text { 中加起小块的 } \\
\text { 外向流 }
\end{array}} = \overbrace{\underbrace{\iint_S \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma}_{\begin{array}{c}
\text { 测量通过 } V \text{'s 边界的总外向流 } \\
\end{array}}}^{\text { 流量积分 }}
$$

--- pic\3D divergence theorem examples.pdf_01.png ---

1. The intuition here is that both integrals measure the rate at which a fluid flowing along the vector field $\mathbf{F}$ is exiting the region $V$ (or entering $V$, if the values of both integrals are negative). Triply integrating divergence does this by counting up all the little bits of outward flow of the fluid inside $V$, while taking the flux integral measures this by checking how much is leaving/entering along the boundary of $V$.
    这里的直觉是，这两个积分都测量了沿着矢量场$\mathbf{F}$流动的流体离开区域$V$的速率（或者如果两个积分的值都是负的，那么就是进入$V$）。通过三重积分散度，我们可以通过计算$V$内部流体的所有小的外流来实现这一点，而通过取通量积分，我们可以通过检查有多少流体沿着$V$的边界离开/进入来测量这一点。

16. Strategizing
    策略

17. The divergence theorem lets you translate between surface integrals and triple integrals, but this is only useful if one of them is simpler than the other. In each of the following examples, take note of the fact that the volume of the relevant region is simpler to describe than the surface of that region.
    散度定理让你可以在表面积分和三重积分之间进行转换，但这只有在其中一个比另一个更简单的情况下才有用。在以下的每一个例子中，注意到相关区域的体积比该区域的表面更简单描述的事实。

18. In general, when you are faced with a surface integral over a closed surface, consider if it would be easier to integrate over the volume enclosed by that surface. If it is, it's a strong signal that the divergence theorem will come in handy.
    一般来说，当你面对一个封闭表面上的表面积分时，考虑一下是否更容易对该表面所围成的体积进行积分。如果是，那么这是一个强烈的信号，说明散度定理会派上用场。

19. Example 1: Surface integral through a cube.
    例1：通过立方体的表面积分。

20. Problem
    问题

21. Let's say $C$ is a $1 \times 1 \times 1$ cube, situated in space such that one corner is on the origin, one corner is at $(1,1,1)$, and so that all its edges are parallel to one of the coordinate axes.
    假设$C$是一个$1 \times 1 \times 1$的立方体，位于空间中，使得一个角在原点，一个角在$(1,1,1)$，并且所有的边都平行于坐标轴之一。

--- pic\3D divergence theorem examples.pdf_02.png ---

1. Let $S$ represents the surface of this cube, which consists of 6 square faces, oriented using outward facing normal vectors. Compute the following surface integral:
   设$S$表示这个立方体的表面，由6个正方形的面组成，使用外向法向量定向。计算以下表面积分：
   $$
   \iint_S\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right) \cdot d \Sigma
   $$

2. Whenever people talk about taking a surface integral of a vector field, this always means taking the dot product with the unit normal vector to that surface:
   每当人们谈到对矢量场进行表面积分时，这总是意味着与该表面的单位法向量取点积：
   $$
   \iint_S(\overrightarrow{\mathbf{v}} \cdot \hat{\mathbf{n}}) d \Sigma
   $$

3. So really, this is a surface integral of a scalar-valued function, it's just that the scalar value arises as the dot product between two vector-valued functions: $(\overrightarrow{\mathbf{v}} \cdot \hat{\mathbf{n}})$.
   所以实际上，这是一个标量值函数的表面积分，只是标量值是由两个矢量值函数之间的点积产生的：$(\overrightarrow{\mathbf{v}} \cdot \hat{\mathbf{n}})$。

4. This is so universal that it often goes without saying that the unit normal vector is involved, so people instead drop the $\hat{\mathbf{n}}$ and write this:
   这是如此普遍，以至于人们经常不言而喻地认为单位法向量参与其中，所以人们省略了$\hat{\mathbf{n}}$，并写成这样：
   $$
   \iint_S \overrightarrow{\mathbf{v}} \cdot d \Sigma
   $$

5. Solution
   解答

6. Concept check: According to the divergence theorem, which of the following is equal to the surface integral we are asked to compute? 
   概念检查：根据散度定理，以下哪一项等于我们被要求计算的表面积分？
   
 
7. Choose 1 answer:
选择1个答案：

1. (B) $\int_0^1 \int_0^1 \int_0^1 \nabla \cdot\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right) d x d y d z$
   


--- pic\3D divergence theorem examples.pdf_03.png ---


1. $$
   \int_0^1 \int_0^1 \int_0^1 \nabla \cdot\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right) d x d y d z
   $$

2. The divergence theorem says that the surface integral of our vector field $\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right)$ through the surface of the cube is the same as the triple integral of the divergence of that vector field throughout the cube.
   散度定理表明，我们的矢量场$\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right)$通过立方体表面的表面积分与该矢量场在整个立方体中的散度的三重积分相同。

3.  The divergence is written like this:
    散度写成这样：
    $$
    \nabla \cdot\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right)
    $$

4.  Describing the cube with a triple integral is relatively straightforward, since each variable $x, y$ and $z$ ranges from 0 to 1, so the appropriate triple integral structure just looks like this:
    用三重积分描述立方体相对简单，因为每个变量$x, y$和$z$的范围都是从0到1，所以适当的三重积分结构就像这样：
    $$
    \int_0^1 \int_0^1 \int_0^1 \ldots d x d y d z
    $$

5.  The cube is a great example of an object whose volume is simpler than its surface. To do this surface integral directly, you would have to address each of the 6 square faces separately. Furthermore, the vector-valued function we are integrating becomes simpler when we take the divergence, as you are about to see. So using the divergence theorem will be doubly helpful!
    立方体是一个体积比表面简单的物体的很好例子。要直接进行这个表面积分，你必须分别处理6个正方形的面。此外，当我们取散度时，我们正在积分的矢量值函数变得更简单，正如你即将看到的。所以使用散度定理将是双重有益的！

6.  Concept check: Compute the divergence of the vector-valued function in the surface integral above.
    概念检查：计算上述表面积分中矢量值函数的散度。
    $$
    \nabla \cdot\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right)=
    $$


--- pic\3D divergence theorem examples.pdf_04.png ---

1. If this feels unfamiliar, consider reviewing the article on divergence.
   如果这感觉不熟悉，可以考虑复习一下关于散度的文章。

2. To compute divergence, think of the symbol $\nabla$ as a vector of partial derivative operators:
   要计算散度，可以将符号$\nabla$视为偏导数运算符的向量：
   $$
   \nabla=\left[\begin{array}{c}
   \frac{\partial}{\partial x} \\
   \frac{\partial}{\partial y} \\
   \frac{\partial}{\partial z}
   \end{array}\right]
   $$

3. Then take the "dot product" between this vector-ish thing and the vector-valued function whose divergence you are computing:
   然后取这个向量和你正在计算散度的向量值函数之间的"点积"：
   $$
   \begin{aligned}
   & \nabla \cdot\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right) \\
   = & {\left[\begin{array}{c}
   \frac{\partial}{\partial x} \\
   \frac{\partial}{\partial y} \\
   \frac{\partial}{\partial z}
   \end{array}\right] \cdot\left[\begin{array}{c}
   2 y \\
   3 y^2 \\
   4 z
   \end{array}\right] } \\
   = & \frac{\partial}{\partial x}(2 y)+\frac{\partial}{\partial y}\left(3 y^2\right)+\frac{\partial}{\partial z}(4 z) \\
   = & 0+6 y+4
   \end{aligned}
   $$

4. Concept check: Use the divergence theorem to finish the problem by plugging the divergence you just computed to the triple integral you chose in the question before that:
   概念检查：使用散度定理来完成问题，将你刚刚计算的散度代入到你在之前的问题中选择的三重积分中：
   $$
   \int_0^1 \int_0^1 \int_0^1 \nabla \cdot\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right) d x d y d z=
   $$


--- pic\3D divergence theorem examples.pdf_05.png ---

1. 
$$
\begin{aligned}
& \int_0^1 \int_0^1 \int_0^1 \underbrace{\nabla \cdot\left(2 y \hat{\mathbf{i}}+3 y^2 \hat{\mathbf{j}}+4 z \hat{\mathbf{k}}\right)}_{\text {将上一个问题的答案代入}} d x d y d z \\
& =\underbrace{\int_0^1 \int_0^1 \int_0^1(6 y+4) d x d y d z}_{\text {分解积分}} \\
& =\underbrace{\int_0^1 \int_0^1 \int_0^1 6 y d x d y d z}_{\begin{array}{c}
\text {这两个积分} \\
\text {将 } 6 y \text {视为常数}
\end{array}}+\underbrace{\int_0^1 \int_0^1 \int_0^1 4 d x d y d z}_{\text {提取常数 } 4} \\
& =\int_0^1 6 y \underbrace{\left(\int_0^1 \int_0^1 d x d z\right)}_{\text {等于 } 1} d y+4 \underbrace{\int_0^1 \int_0^1 \int_0^1 d x d y d z}_{\text {等于 } 1, \text {立方体的体积}} \\
& =\left(\int_0^1 6 y d y\right)+4 \\
& =\left[3 y^2\right]_{y=0}^{y=1}+4 \\
& =3+4 \\
& =7 \\
&
\end{aligned}
$$



2. Example 2: Surface integral through a cylinder
   示例2：通过柱体的表面积分

3. Problem
   问题

4. Let $C$ be a cylinder, whose base is a circle with radius 3 sitting on the $x y$-plane centered at the origin, and whose height is 5 .
   设$C$为一个柱体，其底面是一个半径为3的圆，位于以原点为中心的$xy$平面上，高度为5。



--- pic\3D divergence theorem examples.pdf_06.png ---

1. Letting $S$ represent the surface of this cylinder, oriented with outward facing unit normal vectors compute the following surface integral:
   让$S$表示这个圆柱的表面，以面向外的单位法向量计算以下的表面积分：
   $$
   \iint_S\left[\begin{array}{c}
   x^3 \\
   y^3 \\
   x^3+y^3
   \end{array}\right] \cdot d \Sigma
   $$

2. Solution
   解答

3. As with the previous example, what signals that the divergence theorem might be useful is that the volume of our region is easier to describe than its surface. This is especially true if we anticipate integrating using cylindrical coordinates. And again, the divergence of the relevant function will make it simpler.
   和前面的例子一样，提示我们可能会用到散度定理的信号是，我们区域的体积比其表面更容易描述。如果我们预计使用柱面坐标进行积分，这一点尤其正确。再次，相关函数的散度会使它更简单。

4. Concept check: Compute the divergence of the vector-valued function in the integral above.
   概念检查：计算上述积分中向量值函数的散度。
   $$
   \nabla \cdot\left[\begin{array}{c}
   x^3 \\
   y^3 \\
   x^3+y^3
   \end{array}\right]=
   $$


--- pic\3D divergence theorem examples.pdf_07.png ---

1. 
   $$
   \begin{aligned}
   & \nabla \cdot\left[\begin{array}{c}
   x^3 \\
   y^3 \\
   x^3+y^3
   \end{array}\right] \\
   = & {\left[\begin{array}{c}
   \frac{\partial}{\partial x} \\
   \frac{\partial}{\partial y} \\
   \frac{\partial}{\partial z}
   \end{array}\right] \cdot\left[\begin{array}{c}
   x^3 \\
   y^3 \\
   x^3+y^3
   \end{array}\right] } \\
   = & \frac{\partial}{\partial x}\left(x^3\right)+\frac{\partial}{\partial y}\left(y^3\right)+\frac{\partial}{\partial z}\left(x^3+y^3\right) \\
   = & 3 x^2+3 y^2+0
   \end{aligned}
   $$

2. Concept check: Compute the triple integral of this divergence inside the cylinder $C$ described in the problem. As a reminder, its base is a circle of radius 3 on the $x y$-plane centered at the origin, and it has height 5 .
   概念检查：计算问题中描述的圆柱体$C$内部的这个散度的三重积分。作为提醒，它的底面是半径为3的圆，位于以原点为中心的$xy$平面上，高度为5。
   $$
   \iiint_C\left(\nabla \cdot\left[\begin{array}{c}
   x^3 \\
   y^3 \\
   x^3+y^3
   \end{array}\right]\right) d V=
   $$


3. First, just plug in the value you found from the last problem:
   首先，只需插入你从最后一个问题中找到的值：
   $$
   \begin{aligned}
   & \iiint_C \nabla \cdot\left[\begin{array}{c}
   x^3 \\
   y^3 \\
   x^3+y^3
   \end{array}\right] d V \\
   = & \iiint_C 3\left(x^2+y^2\right) d V
   \end{aligned}
   $$


4. Next, because we are integrating over a cylinder, it is very natural to integrate using_cylindrical coordinates.
   接下来，因为我们是在圆柱体上进行积分，所以使用柱面坐标进行积分是非常自然的。

5. For this problem, that involves three steps:
   对于这个问题，这涉及到三个步骤：

6. Replace $d V$ with $r d \theta d r d z$ (don't forget the little $r$ in front, this is what turns $d \theta$ into a unit of length).
     用$r d \theta d r d z$替换$d V$（别忘了前面的小$r$，这是将$d \theta$转换为长度单位的东西）。

7. Replace $x^2+y^2$ with $r^2$.
      用$r^2$替换$x^2+y^2$。



--- pic\3D divergence theorem examples.pdf_08.png ---

1. Set bounds which describe our cylinder. Luckily, all of these are constant:
   设置描述我们的圆柱体的边界。幸运的是，所有这些都是常数：

2. $r$ ranges from 0 to 3 .
   $r$的范围从0到3。

3. $\theta$ ranges from 0 to $2 \pi$.
   $\theta$的范围从0到$2 \pi$。

4. $z$ ranges from 0 to 5 .
   $z$的范围从0到5。

5. Applying all this to the integral, you get something that can be worked out:
   将所有这些应用到积分中，你可以得到一个可以计算的结果：

   $$
   \begin{aligned}
   & \underbrace{\iiint_C}_{\text {插入界限}} 3 \underbrace{\left(x^2+y^2\right)}_{r^2} \underbrace{d V}_{r d \theta d r d z} \\
   & =\int_{z=0}^{z=5} \int_{r=0}^{r=3} \int_{\theta=0}^{\theta=2 \pi}\left(3 r^2\right) r d \theta d r d z \\
   & =3 \underbrace{\int_{z=0}^{z=5} \int_{r=0}^{r=3} \int_{\theta=0}^{\theta=2 \pi} r^3 d \theta d r d z}_{\substack{\text { 这两个积分 } \\
   \text { 将 } r \text { 视为常数。 }}} \\
   & =3 \int_{r=0}^{r=3} r^3 \int_{z=0}^{z=5} \underbrace{\int_{\theta=0}^{\theta=2 \pi} d \theta}_{=2 \pi} d z d r \\
   & =3(2 \pi) \int_{r=0}^{r=3} r^3 \underbrace{\int_{z=0}^{z=5} d z}_{=5} d r \\
   & =3(2 \pi)(5) \int_{r=0}^{r=3} r^3 d r \\
   & =3(2 \pi)(5)\left[\frac{1}{4} r^4\right]_{r=0}^{r=3} \\
   & =3(2 \pi)(5)\left(\frac{1}{4} 3^4-\frac{1}{4} 0^4\right) \\
   & =\frac{3(2 \pi)(5)\left(3^4\right)}{4} \\
   & =\frac{1,215 \pi}{2} \\
   &
   \end{aligned}
   $$


--- pic\3D divergence theorem examples.pdf_09.png ---

1. Example 3: Surface area from a volume integral
   示例3：从体积积分得到的表面积

2. Problem:
   Use the divergence theorem to compute the surface area of a sphere with radius 1 , given the fact that the volume of that sphere is $\frac{4}{3} \pi$.
   问题：
   已知球的体积为$\frac{4}{3} \pi$，使用散度定理计算半径为1的球的表面积。

3. Solution
   This feels a bit different from the previous two examples, doesn't it? To start, there is no vector field in the problem, even though the divergence theorem is all about vector fields!
   解决方案
   这感觉和前两个例子有点不同，不是吗？首先，尽管散度定理全是关于矢量场的，但问题中没有矢量场！

4. If you let $S$ describe the surface of the sphere, its surface area will be given by the following as-simple-as-they-come surface integral:
   如果你让$S$描述球的表面，它的表面积将由下面这个简单的表面积分给出：
   $$
   \iint_S 1 d \Sigma
   $$

 

--- pic\3D divergence theorem examples.pdf_08.png ---

1. Set bounds which describe our cylinder. Luckily, all of these are constant:
   设置描述我们的圆柱体的边界。幸运的是，所有这些都是常数：

2. $r$ ranges from 0 to 3 .
   $r$的范围从0到3。

3. $\theta$ ranges from 0 to $2 \pi$.
   $\theta$的范围从0到$2 \pi$。

4. $z$ ranges from 0 to 5 .
   $z$的范围从0到5。

5. Applying all this to the integral, you get something that can be worked out:
   将所有这些应用到积分中，你可以得到一个可以计算的结果：
   $$
   \begin{aligned}
   & \underbrace{\iiint_C}_{\text {lug in bounds }} 3 \underbrace{\left(x^2+y^2\right)}_{r^2} \underbrace{d V}_{r d \theta d r d z} \\
   & =\int_{z=0}^{z=5} \int_{r=0}^{r=3} \int_{\theta=0}^{\theta=2 \pi}\left(3 r^2\right) r d \theta d r d z \\
   & =3 \underbrace{\int_{z=0}^{z=5} \int_{r=0}^{r=3} \int_{\theta=0}^{\theta=2 \pi} r^3 d \theta d r d z}_{\substack{\text { Two of these integrals } \\
   \text { treat } r \text { as a constant. }}} \\
   & =3 \int_{r=0}^{r=3} r^3 \int_{z=0}^{z=5} \underbrace{\int_{\theta=0}^{\theta=2 \pi} d \theta}_{=2 \pi} d z d r \\
   & =3(2 \pi) \int_{r=0}^{r=3} r^3 \underbrace{\int_{z=0}^{z=5} d z}_{=5} d r \\
   & =3(2 \pi)(5) \int_{r=0}^{r=3} r^3 d r \\
   & =3(2 \pi)(5)\left[\frac{1}{4} r^4\right]_{r=0}^{r=3} \\
   & =3(2 \pi)(5)\left(\frac{1}{4} 3^4-\frac{1}{4} 0^4\right) \\
   & =\frac{3(2 \pi)(5)\left(3^4\right)}{4} \\
   & =\frac{1,215 \pi}{2} \\
   &
   \end{aligned}
   $$

--- pic\3D divergence theorem examples.pdf_09.png ---

6. Example 3: Surface area from a volume integral
   示例3：从体积积分得到的表面积

7. Problem:
   Use the divergence theorem to compute the surface area of a sphere with radius 1 , given the fact that the volume of that sphere is $\frac{4}{3} \pi$.
   问题：
   已知球的体积为$\frac{4}{3} \pi$，使用散度定理计算半径为1的球的表面积。

8. Solution
   This feels a bit different from the previous two examples, doesn't it? To start, there is no vector field in the problem, even though the divergence theorem is all about vector fields!
   解决方案
   这感觉和前两个例子有点不同，不是吗？首先，尽管散度定理全是关于矢量场的，但问题中没有矢量场！

9. If you let $S$ describe the surface of the sphere, its surface area will be given by the following as-simple-as-they-come surface integral:
   如果你让$S$描述球的表面，它的表面积将由下面这个简单的表面积分给出：
   $$
   \iint_S 1 d \Sigma
   $$

--- pic\3D divergence theorem examples.pdf_10.png ---

1. However, this is a surface integral of a scalar-valued function, namely the constant function $f(x, y, z)=1$, but the divergence theorem applies to surface integrals of a vector field. In other words, the divergence theorem applies to surface integrals that look like this:
   然而，这是一个标量值函数的表面积分，即常数函数$f(x, y, z)=1$，但散度定理适用于矢量场的表面积分。换句话说，散度定理适用于如下形式的表面积分：
   $$
   \iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) d \Sigma
   $$

2. Here, $\hat{\mathbf{n}}$ is some function which gives unit normal vectors to $S$, the surface of the sphere. You can turn this into the desired surface area integral by finding a vector-valued function $\mathbf{F}$ such that $\mathbf{F} \cdot \hat{\mathbf{n}}$ always equals 1 .
   这里，$\hat{\mathbf{n}}$是一个函数，它给出了球面$S$的单位法向量。你可以通过找到一个矢量值函数$\mathbf{F}$，使得$\mathbf{F} \cdot \hat{\mathbf{n}}$总是等于1，将其转化为所需的表面积分。

3. Concept check: Which of the following definitions of a vector field $\mathbf{F}$ will ensure the property $\mathbf{F} \cdot \hat{\mathbf{n}}=1$ at all points on the surface of the sphere?
   概念检查：以下哪个矢量场$\mathbf{F}$的定义将确保在球面上所有点处都有$\mathbf{F} \cdot \hat{\mathbf{n}}=1$的性质？

1. Choose 1 answer:
   选择一个答案：
  
1. (A) $\mathbf{F}=\hat{\mathbf{n}}$
   
   
2. $$
   \mathbf{F}=\hat{\mathbf{n}}
   $$
   With this choice, $\mathbf{F} \cdot \hat{\mathbf{n}}=\hat{\mathbf{n}} \cdot \hat{\mathbf{n}}$, and any unit vector dotted against itself equals 1.
   选择这个，$\mathbf{F} \cdot \hat{\mathbf{n}}=\hat{\mathbf{n}} \cdot \hat{\mathbf{n}}$，任何单位向量与自身的点积都等于1。

3. Concept check: Using this choice for $\mathbf{F}$, together with the divergence theorem, which of the following integrals will give the surface area of the unit sphere? Let $B$ represent the volume enclosed by the sphere, also known as the "unit ball".
   概念检查：使用这个$\mathbf{F}$的选择，结合散度定理，以下哪个积分将给出单位球的表面积？让$B$表示由球体所围成的体积，也被称为"单位球"。

1. Choose 1 answer:
   选择一个答案：
   
1. (A) $\iiint_B \nabla \cdot \hat{\mathbf{n}} d V$
   



--- pic\3D divergence theorem examples.pdf_11.png ---

1. The first choice is correct. In fact, the other choice doesn't even make sense, since $(\hat{\mathbf{n}} \cdot \hat{\mathbf{n}})$ gives a scalar valued function, and you can only take the divergence of vector-valued functions.
   第一个选择是正确的。实际上，另一个选择甚至没有意义，因为$(\hat{\mathbf{n}} \cdot \hat{\mathbf{n}})$给出了一个标量值函数，你只能取矢量值函数的散度。

2. The surface integral we want to compute looks like this:
   我们想要计算的表面积分看起来像这样：
   $$
   \iint_S 1 d \Sigma=\iint_S(\hat{\mathbf{n}} \cdot \hat{\mathbf{n}}) d \Sigma
   $$

3. This is the flux of the unit normal vector function $\hat{\mathbf{n}}$ through the surface. According to the divergence theorem, this is the same as integrating the divergence of that vector field within the volume of the sphere:
   这是单位法向量函数$\hat{\mathbf{n}}$通过表面的通量。根据散度定理，这与在球体的体积内积分该矢量场的散度是相同的：
   $$
   \iiint_B \nabla \cdot \hat{\mathbf{n}} d V
   $$

4. Concept check: Which of the following functions gives unit normal vectors to the surface of the unit sphere?
   概念检查：以下哪个函数给出了单位球表面的单位法向量？

1. Choose 1 answer:
   选择一个答案：
   
1. (C) $\hat{\mathbf{n}}(x, y, z)=x \hat{\mathbf{i}}+y \hat{\mathbf{j}}+z \hat{\mathbf{k}}$（见最后一页）

5.  Concept check: Compute the divergence of this function.
    概念检查：计算这个函数的散度。
    $$
    \nabla \cdot \hat{\mathbf{n}}=
    $$

--- pic\3D divergence theorem examples.pdf_12.png ---

1. Plugging in $\hat{\mathbf{n}}(x, y, z)=x \hat{\mathbf{i}}+y \hat{\mathbf{j}}+z \hat{\mathbf{k}}$, here's what we get:
   将$\hat{\mathbf{n}}(x, y, z)=x \hat{\mathbf{i}}+y \hat{\mathbf{j}}+z \hat{\mathbf{k}}$代入，我们得到：

2. $\nabla \cdot \hat{\mathbf{n}}$
   $=\left[\begin{array}{c}\frac{\partial}{\partial x} \\ \frac{\partial}{\partial y} \\ \frac{\partial}{\partial z}\end{array}\right] \cdot\left[\begin{array}{c}x \\ y \\ z\end{array}\right]$
   $=\frac{\partial}{\partial x}(x)+\frac{\partial}{\partial y}(y)+\frac{\partial}{\partial z}(z)$
   $=1+1+1$
   $=3$

3. Concept check: Finally, given the fact that the volume within the unit sphere is $\frac{4}{3} \pi$, compute the following integral:
   概念检查：最后，给定单位球体内的体积是$\frac{4}{3} \pi$，计算以下积分：
   $$
   \iiint_B \nabla \cdot \hat{\mathbf{n}} d V=
   $$

4. Luckily, the expression $\nabla \cdot \hat{\mathbf{n}}$ turned out to be a constant, 3 . This means we are left with a volume integral:
   幸运的是，表达式$\nabla \cdot \hat{\mathbf{n}}$结果是一个常数，3。这意味着我们剩下的是一个体积积分：

   $$
   \begin{aligned}
   & \underbrace{\iiint_C}_{\text {插入界限}} 3 \underbrace{\left(x^2+y^2\right)}_{r^2} \underbrace{d V}_{r d \theta d r d z} \\
   & =\int_{z=0}^{z=5} \int_{r=0}^{r=3} \int_{\theta=0}^{\theta=2 \pi}\left(3 r^2\right) r d \theta d r d z \\
   & =3 \underbrace{\int_{z=0}^{z=5} \int_{r=0}^{r=3} \int_{\theta=0}^{\theta=2 \pi} r^3 d \theta d r d z}_{\substack{\text { 这两个积分 } \\
   \text { 将 } r \text { 视为常数。 }}} \\
   & =3 \int_{r=0}^{r=3} r^3 \int_{z=0}^{z=5} \underbrace{\int_{\theta=0}^{\theta=2 \pi} d \theta}_{=2 \pi} d z d r \\
   & =3(2 \pi) \int_{r=0}^{r=3} r^3 \underbrace{\int_{z=0}^{z=5} d z}_{=5} d r \\
   & =3(2 \pi)(5) \int_{r=0}^{r=3} r^3 d r \\
   & =3(2 \pi)(5)\left[\frac{1}{4} r^4\right]_{r=0}^{r=3} \\
   & =3(2 \pi)(5)\left(\frac{1}{4} 3^4-\frac{1}{4} 0^4\right) \\
   & =\frac{3(2 \pi)(5)\left(3^4\right)}{4} \\
   & =\frac{1,215 \pi}{2} \\
   &
   \end{aligned}
   $$


--- pic\3D divergence theorem examples.pdf_13.png ---

1. And wouldn't you know it, that's the surface area of a unit sphere!
   你知道吗，那就是单位球的表面积！
   
1. In this example, when you computed $\nabla \cdot \hat{\mathbf{n}}$, the result was just a constant, 3 . This was underlying reason behind the fact that the surface area of a unit sphere is 3 times the volume of that sphere.
   在这个例子中，当你计算 $\nabla \cdot \hat{\mathbf{n}}$ 时，结果只是一个常数，3。这就是单位球的表面积是其体积的3倍的事实背后的原因。

2. If you did this problem in two dimensions, the analogous two-dimensional divergence $\nabla \cdot \hat{\mathbf{n}}$ would have been 2 . And in fact, you could use the twodimensional divergence theorem to justify why the circumference of a unit circle is 2 times the area of that circle.
   如果你在二维中解决这个问题，类似的二维散度$\nabla \cdot \hat{\mathbf{n}}$将是2。实际上，你可以使用二维散度定理来证明为什么单位圆的周长是该圆面积的2倍。

3. In general, an analogous argument using the higher-dimensional analog of the divergence theorem can show that the $(n-1)$-dimensional volume of the boundary of an $n$-dimensional unit sphere must be $n$ times the $n$-dimensional volume of that sphere.
   一般来说，使用散度定理的高维类比的类似论证可以显示，$n$维单位球的边界的$(n-1)$维体积必须是该球的$n$维体积的$n$倍。

4. Summary
   总结

5. The divergence theorem is useful whenever the interior volume of a region is easier to describe than its surface.
   当一个区域的内部体积比其表面更容易描述时，散度定理就很有用。

6.  It also helps if the divergence of the relevant vector field turns it into a simpler function.
    如果相关矢量场的散度将其转化为一个更简单的函数，也是有帮助的。

--- pic\3D divergence theorem examples.pdf_14.png ---

1. $\hat{\mathbf{n}}(x, y, z)=x \hat{\mathbf{i}}+y \hat{\mathbf{j}}+z \hat{\mathbf{k}}$
   $\hat{\mathbf{n}}(x, y, z)=x \hat{\mathbf{i}}+y \hat{\mathbf{j}}+z \hat{\mathbf{k}}$

2. The neat thing about the unit sphere centered at the origin is that if you take a vector pointing from the origin to a point on the sphere, then move it so that its tail is on that point, it will be normal to the sphere. This is easiest to draw and see on a circle, but the same principle applies for a sphere:
   关于以原点为中心的单位球体的一个巧妙之处是，如果你取一个从原点指向球体上一点的向量，然后移动它使其尾部在那个点上，它将垂直于球体。这在圆上最容易画出来和看到，但对于球体也适用同样的原理：

3. What's more, since the problem asks about a unit sphere, these vectors are all automatically unit vectors, so there's no need to normalize!
   更重要的是，由于问题是关于单位球体的，这些向量都自动成为单位向量，所以无需标准化！




