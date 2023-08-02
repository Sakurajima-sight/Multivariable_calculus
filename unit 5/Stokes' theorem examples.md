
--- pic\Stokes' theorem examples.pdf_00.png ---

1. Stokes' theorem examples
   斯托克斯定理的例子

2. See how Stokes' theorem is used in practice.
   看看斯托克斯定理在实践中是如何使用的。

3. Background
   背景

4. Stokes' theorem
   斯托克斯定理

5. Line integrals
   线积分

6. Flux in 3D
   三维的通量

7. Curl
   旋度

8. The formula (quick review)
   公式（快速回顾）

9. Stokes' theorem is a tool to turn the surface integral of a curl vector field into a line integral around the boundary of that surface, or vice versa. Specifically, here's what it says:
   斯托克斯定理是一个工具，可以将旋度矢量场的表面积分转化为围绕该表面边界的线积分，反之亦然。具体来说，它是这样说的：

10. Let's go through each term:
    让我们逐个解释每个术语：

--- pic\Stokes' theorem examples.pdf_01.png ---

1. $\mathbf{F}(x, y, z)$ is a three-dimensional vector field.
    $\mathbf{F}(x, y, z)$是一个三维矢量场。

12. $\operatorname{curl} \mathbf{F}$, also often written as $\nabla \times \mathbf{F}$. It is the three-dimensional curl of $\mathbf{F}$, which is a vector field.
    $\operatorname{curl} \mathbf{F}$，也经常写作$\nabla \times \mathbf{F}$。它是$\mathbf{F}$的三维旋度，$\mathbf{F}$是一个矢量场。

13. $S$ is a surface in three dimensions.
    $S$是三维空间中的一个表面。

14. $\hat{\mathbf{n}}$ represents a function that gives unit normal vectors to $S$.
    $\hat{\mathbf{n}}$表示一个给出$S$的单位法向量的函数。

15. $C$ is the boundary of $S$.
    $C$是$S$的边界。

16. $C$ is oriented using the right-hand rule, meaning if you point the thumb of your right hand in the direction of a unit normal vector $\hat{n}$ near the edge of $S$ and curl your fingers, the direction they point indicates the direction you should integrate around $C$.
    $C$是使用右手规则定向的，意思是如果你将右手的拇指指向$S$边缘附近的单位法向量$\hat{n}$的方向并卷曲你的手指，它们指向的方向表示你应该沿着$C$的方向积分。

17. Example 1: From a surface integral to line integral
    例1：从表面积分到线积分

18. Problem
    问题

19. Let $S$ be the half of a unit sphere centered at the origin that is above the $x y$ plane, oriented with outward facing unit normal vectors. Let $\overrightarrow{\mathbf{v}}(x, y, z)$ be the vector field defined as follows:
    设$S$是以原点为中心的单位球的一半，位于$x y$平面之上，定向为向外的单位法向量。设$\overrightarrow{\mathbf{v}}(x, y, z)$是如下定义的矢量场：
    $$
    \overrightarrow{\mathbf{v}}(x, y, z)=y \hat{\mathbf{i}}
    $$

20. Compute the following surface integral:
    计算以下的表面积分：
    $$
    \iint_S \overrightarrow{\mathbf{v}} \cdot d \Sigma
    $$


--- pic\Stokes' theorem examples.pdf_02.png ---

1. Whenever people talk about taking a surface integral of a vector field, this always means taking the dot product with the unit normal vector to that surface:
   每当人们谈论对矢量场进行表面积分时，这总是意味着与该表面的单位法向量进行点积：
   $$
   \iint_S(\overrightarrow{\mathbf{v}} \cdot \hat{\mathbf{n}}) d \Sigma
   $$

2. So really, this is a surface integral of a scalar-valued function, but that scalar value arises as the dot product between two vector-valued functions: $(\overrightarrow{\mathbf{v}} \cdot \hat{\mathbf{n}})$
   所以实际上，这是一个标量值函数的表面积分，但是那个标量值是两个矢量值函数之间的点积得出的：$(\overrightarrow{\mathbf{v}} \cdot \hat{\mathbf{n}})$

3. This is so universal that it often goes without saying that the unit normal vector is involved, so people instead drop the $\hat{\mathbf{n}}$ and write this:
   这是如此普遍，以至于人们经常不言而喻地认为单位法向量是涉及的，所以人们反而省略了$\hat{\mathbf{n}}$，并写成这样：
   $$
   \iint_S \overrightarrow{\mathbf{v}} \cdot d \Sigma
   $$

4. Solution
   解决方案

5. Remember, Stokes' theorem relates the surface integral of the curl of a function to the line integral of that function around the boundary of the surface. This means we will do two things:
   记住，斯托克斯定理将一个函数的旋度的表面积分与该函数围绕表面边界的线积分关联起来。这意味着我们将做两件事：

1. Step 1: Find a function whose curl is the vector field $y \hat{\mathbf{i}}$
   步骤1：找到一个函数，其旋度是向量场 $y \hat{\mathbf{i}}$

--- pic\Stokes' theorem examples.pdf_03.png ---

1. Step 2: Take the line integral of that function around the unit circle in the $x y$-plane, since this circle is the boundary of our half-sphere.
   步骤2：在$x y$平面的单位圆周围对该函数进行线积分，因为这个圆是我们半球的边界。

8. Concept check: Find a vector field $\mathrm{F}(x, y, z)$ satisfying the following property:
   概念检查：找到一个满足以下性质的矢量场$\mathrm{F}(x, y, z)$：
   $$
   \nabla \times \mathbf{F}=y \hat{\mathbf{i}}
   $$

9. There are multiple ways to do this, but one in particular will make our lives easiest. In the one I'm thinking of, the $\hat{\mathbf{i}}$ and $\hat{\mathbf{j}}$ components are 0 , while the $\hat{\mathbf{k}}$ component is non-zero. Can you find it?
   有多种方法可以做到这一点，但有一种特别会让我们的生活变得更容易。在我想到的那个方法中，$\hat{\mathbf{i}}$和$\hat{\mathbf{j}}$组件是0，而$\hat{\mathbf{k}}$组件是非零的。你能找到它吗？
   $$
   \mathbf{F}(x, y, z)=0 \hat{\mathbf{i}}+0 \hat{\mathbf{j}}+\square \hat{\mathbf{k}}
   $$

10. First things first, let's write out how curl is computed. Suppose $F_1, F_2$, and $F_3$ represent the coordinate functions of our vector-valued function:
    首先，让我们写出如何计算旋度。假设$F_1, F_2$和$F_3$表示我们的矢量值函数的坐标函数：
    $$
    \mathbf{F}(x, y, z)=F_1(x, y, z) \hat{\mathbf{i}}+F_2(x, y, z) \hat{\mathbf{j}}+F_3(x, y, z) \hat{\mathbf{k}}
    $$

11. Then curl is computed with the following determinant trick:
    然后，旋度是用以下行列式技巧计算的：
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

12. We want this whole expression to equal the simple vector field $\overrightarrow{\mathbf{v}}(x, y, z)=y \hat{\mathbf{i}}$. This means we need the following equality:
    我们希望这个整个表达式等于简单的矢量场$\overrightarrow{\mathbf{v}}(x, y, z)=y \hat{\mathbf{i}}$。这意味着我们需要以下等式：
    $$
    \left(\frac{\partial F_3}{\partial y}-\frac{\partial F_2}{\partial z}\right)=y
    $$

1. There are many pairs of functions $F_2$ and $F_3$ that will make this equality work. Given how I phrased the question above, though, we want $F_2$ to be 0.
   有许多函数对 $F_2$ 和 $F_3$ 能使这个等式成立。但是，根据我上面提出的问题，我们希望 $F_2$ 为 0。


--- pic\Stokes' theorem examples.pdf_04.png ---

1. This means the term $\frac{\partial F_3}{\partial y}$ must take care of the entire equation. To do this, take the antiderivative of $y$, the function on the right-hand-side, with respect to the variable $y$ :
   这意味着项$\frac{\partial F_3}{\partial y}$必须负责整个等式。为此，对右侧的函数$y$关于变量$y$取反导数：
   $$
   F_3(x, y, z)=\frac{1}{2} y^2
   $$

2. When you set the other two components equal to 0 , you can check the original curl expression to see that $\nabla \times \mathbf{F}=y \hat{\mathbf{i}}$ as desired.
   当你将其他两个分量设为0时，你可以检查原始的旋度表达式，看到$\nabla \times \mathbf{F}=y \hat{\mathbf{i}}$，这正是我们想要的。

3. Given that you can find many different functions satisfying the property $\nabla \times \mathbf{F}=y \hat{\mathbf{i}}$, how do you know which one to choose?
   考虑到你可以找到许多不同的函数满足性质$\nabla \times \mathbf{F}=y \hat{\mathbf{i}}$，你如何知道选择哪一个？

4. To start, we want something as simple as possible, so if you can make all but one component 0 , do it.
   首先，我们希望尽可能简单，所以如果你能让除一个分量外的所有分量都为0，就这么做。

5. From the answer explanation, though, you might have noticed that we could also have chosen a function where only $F_2$ is nonzero, so why not use that? Although it would be fine to use that other function, when you consider the fact that we will ultimately be performing a line integral over the unit circle in the $x y$-plane, having a function with only a $\hat{\mathbf{k}}$-component will make things even simpler.
   从答案解释中，你可能已经注意到我们也可以选择只有$F_2$非零的函数，那为什么不使用那个呢？虽然使用那个其他函数也是可以的，但当你考虑到我们最终将在$x y$平面的单位圆上执行线积分的事实时，只有一个$\hat{\mathbf{k}}$分量的函数会使事情变得更简单。

6. The surface $S$ is defined to be the portion of the unit sphere above the $x y$ plane. The boundary of this hemisphere is the unit circle on the $x y$-plane.
   表面$S$被定义为单位球体上方的部分。这个半球的边界是$x y$平面上的单位圆。

--- pic\Stokes' theorem examples.pdf_05.png ---

7. Concept check: Both of the following parameterize the unit circle on the $x y$ plane, but each with a different orientation. Which one corresponds with the orientation of the hemisphere above the $x y$-plane with outward-facing unit normal vectors? ("Correspond" in the sense that we can apply Stokes' theorem.)
   概念检查：以下两者都参数化了$x y$平面上的单位圆，但每个都有不同的方向。哪一个与上方半球的方向相对应，该半球在$x y$平面上具有向外的单位法向量？（“对应”是指我们可以应用斯托克斯定理的意义。）

8. Choose 1 answer:
   选择1个答案：
   (A) $\left[\begin{array}{c}\cos (t) \\ \sin (t) \\ 0\end{array}\right]$, where $0 \leq t \leq 2 \pi$


9. The first answer choice is correct:
   第一个答案选择是正确的：
   $$
   \left[\begin{array}{c}
   \cos (t) \\
   \sin (t) \\
   0
   \end{array}\right] \text {, where } 0 \leq t \leq 2 \pi
   $$

1. This corresponds to a counterclockwise orientation of the circle.
这对应于圆的逆时针方向。

10. Surfaces are oriented by the chosen direction for their unit normal vectors, and curves are oriented by the chosen direction for their tangent vectors. In order to apply Stokes' theorem, the orientation of a surface and its boundary must "line up" in the right way. Here are several different, but equivalent, ways to phrase how that alignment must look:
    表面的方向由其单位法向量的选择方向确定，曲线的方向由其切线的选择方向确定。为了应用斯托克斯定理，表面和其边界的方向必须以正确的方式“对齐”。以下是几种不同但等效的方式来描述这种对齐应该是什么样的：




--- pic\Stokes' theorem examples.pdf_06.png ---

1. If you look at the surface in such a way that the unit normal vectors are all pointed towards your face, the curve should be oriented counterclockwise.
   如果你以这样的方式观察表面，即单位法向量都指向你的脸，那么曲线应该是逆时针方向的。

2. The curve's orientation should follow the right-hand rule, in the sense that if you stick the thumb of your right hand in the direction of a unit normal vector near the edge of the surface, and curl your fingers, the direction they point on the curve should match its orientation.
   曲线的方向应该遵循右手规则，也就是说，如果你将右手的拇指指向表面边缘附近的单位法向量的方向，然后卷曲你的手指，它们在曲线上指向的方向应该与其方向匹配。

3. When you are walking along the boundary curve with your body pointing out in the direction of the unit normal vector, you should be walking in such a way that the surface is to your left side.
   当你沿着边界曲线行走，你的身体指向单位法向量的方向时，你应该以这样的方式行走，即表面在你的左侧。

4. If you apply any of these images to our specific example, you will see that a counterclockwise orientation of the unit circle "aligns" with outward facing unit normal vectors for the hemisphere.
   如果你将这些图像中的任何一个应用到我们的具体例子中，你会看到，单位圆的逆时针方向与半球的向外面向的单位法向量"对齐"。

5. Concept check: Let $C$ represent the boundary of the surface $S$. Use the parameterization of $C$ that you just chose, together with the definition of $\mathbf{F}$ that you found in the question before that, to solve the following line integral.
   概念检查：让$C$表示表面$S$的边界。使用你刚刚选择的$C$的参数化，以及你在之前的问题中找到的$\mathbf{F}$的定义，来解以下线积分。
   $$
   \oint_C \mathbf{F} \cdot d \mathbf{r}=
   $$


6. $\mathbf{F}(x, y, z)=\frac{1}{2} y^2 \hat{\mathbf{k}}$
   

--- pic\Stokes' theorem examples.pdf_07.png ---

1. You actually don't need to dive into any computations once you think about what this integral means. Take a look at $\mathbf{F}(x, y, z)$ :
   实际上，一旦你思考这个积分的含义，就不需要深入计算了。看一下$\mathbf{F}(x, y, z)$：
   $$
   \mathbf{F}(x, y, z)=\frac{1}{2} y^2 \hat{\mathbf{k}}
   $$

2. Most notably, it only has a $\hat{\mathbf{k}}$-component, so all the vectors are perpendicular to the $x y$-plane. Since the curve $C$ resides completely in the $x y$-plane, all the little tangent vectors $d \mathbf{r}$ will be contained on the $x y$-plane. Therefore, the dot product $\mathbf{F} \cdot d \mathbf{r}$ in the line integral will always be 0 , so the line integral as a whole is just 0 .
   最值得注意的是，它只有一个$\hat{\mathbf{k}}$-分量，所以所有的向量都垂直于$x y$-平面。由于曲线$C$完全位于$x y$-平面上，所有的小切向量$d \mathbf{r}$都将包含在$x y$-平面上。因此，线积分中的点积$\mathbf{F} \cdot d \mathbf{r}$总是0，所以线积分的整体就是0。

3.  Of course, this is a fact you could have recognized even earlier in the problem, before parameterizing the circle. However, I wanted an excuse to let you practice thinking about matching up the orientation of a surface's boundary with the surface itself, since that is an easy thing to accidentally mess up in a Stokes' theorem problem.
    当然，这是一个你在问题中甚至在参数化圆之前就可以认识到的事实。然而，我想找个借口让你练习思考如何将一个表面的边界的方向与表面本身匹配起来，因为在斯托克斯定理问题中，这是一个很容易出错的地方。

4.  Example 2: Wind through a butterfly net
    例2：风穿过蝴蝶网

5.  Problem
    问题

6.  Suppose you have a butterfly net with a square-shaped rim, and the wind is blowing through the net. Think about the square rim positioned in space on the $y z$-plane such that its four corners are at the following four points:
    假设你有一个方形边缘的蝴蝶网，风正在穿过网。想象一下，方形边缘在$y z$平面上的空间位置，使得它的四个角在以下四个点：
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

7.  Furthermore, let the net be some surface emerging from this rim in the positive $x$-direction.
 此外，让网是从这个边缘向正$x$方向出现的一些表面。


--- pic\Stokes' theorem examples.pdf_08.png ---

1. Suppose the velocity vector field for the wind is given by the following function:
   假设风的速度矢量场由以下函数给出：
   $$
   \mathbf{F}=\left[\begin{array}{c}
   y^2 \\
   z^2 \\
   x^2
   \end{array}\right]
   $$

2. Assuming the air has a uniform density of $1 \mathrm{~kg} / \mathrm{m}^3$, how much air passes through your net per unit time? Specifically, suppose air going from the inside of the net to the outside counts positively towards this sum, and air going from the outside to the inside counts negatively.
   假设空气的密度均匀，为$1 \mathrm{~kg} / \mathrm{m}^3$，那么每单位时间有多少空气通过你的网？具体来说，假设从网内部到外部的空气对这个总和有正的贡献，而从外部到内部的空气有负的贡献。

3. Step 1: Dissecting the question
   第一步：解析问题

4. Before anything, we need to compose our thoughts and piece together how this physics-sounding problem is a Stokes' theorem question.
   在一切之前，我们需要整理我们的思绪，并将这个听起来像物理问题的问题拼凑成一个斯托克斯定理的问题。

5. Concept check: What is this question really asking about?
   概念检查：这个问题真正问的是什么？

6. Choose 1 answer:
   选择1个答案：

--- pic\Stokes' theorem examples.pdf_09.png ---

1. (A) The flux of $\mathrm{F}$ through the surface of the butterfly net.
   (A) 通过蝴蝶网表面的$\mathrm{F}$的通量。


2.  This is a flux problem, since it is asking how much fluid passes through a surface, given the velocity vector field of that fluid. See this article on 3D flux if that feels unfamiliar.
    这是一个通量问题，因为它在问，给定流体的速度矢量场，有多少流体通过一个表面。如果你对3D通量感到不熟悉，可以参考这篇文章。

3.  Concept check: More specifically, which of the following integrals represents the answer to the question? Let $S$ denote the surface of the butterfly net, while $C$ is the square rim of that net sitting in the $y z$-plane.
    概念检查：更具体地说，下列哪个积分代表了问题的答案？让$S$表示蝴蝶网的表面，而$C$是位于$y z$平面的网的方形边缘。

4.  Choose 1 answer:
    选择1个答案：

5.  (A) $\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) d \Sigma$, where $\hat{\mathbf{n}}$ represents outward-facing unit normal vectors.
    (A) $\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) d \Sigma$，其中$\hat{\mathbf{n}}$表示朝外的单位法向矢量。





--- pic\Stokes' theorem examples.pdf_10.png ---

1. The rate at which air passes through the net, in terms of volume per unit time, is given by the following flux integral:
   空气通过网的速率，以单位时间的体积来表示，由以下通量积分给出：
   $$
   \iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) d \Sigma
   $$

2. Since the assumption is that air has uniform density $1 \mathrm{~kg} / \mathrm{m}^3$, this also gives the mass of air passing through the net per unit time.
   由于假设空气的密度均匀，为$1 \mathrm{~kg} / \mathrm{m}^3$，这也给出了每单位时间通过网的空气质量。

3. To capture the idea that air going from the inside of the net to the outside counts positively toward flux, while air going from the outside counts negatively towards flux, the unit normal vectors $\hat{\mathbf{n}}$ must be outward-facing. This way, the dot product $\mathbf{F} \cdot \hat{\mathbf{n}}$ will be positive at points where the air's trajectory is outward, and negative when it is inward.
   为了捕捉到从网内部到外部的空气对通量有正向贡献，而从外部到内部的空气对通量有负向贡献的想法，单位法向量$\hat{\mathbf{n}}$必须朝外。这样，当空气的轨迹向外时，点积$\mathbf{F} \cdot \hat{\mathbf{n}}$在点上会是正的，当它向内时会是负的。

4. Again, if this feels unfamiliar, feel free to review the article on 3D flux.
   再次，如果这感觉不熟悉，可以随时复习关于3D通量的文章。

5. Really, this is all just a way to give a physical interpretation to a surface integral through a vector field.
   实际上，这只是一种通过矢量场给出表面积分的物理解释的方式。

6. Step 2: Applying Stokes' theorem
   步骤2：应用斯托克斯定理

7. What might feel weird about this problem, and what suggests that you will need Stokes' theorem, is that the surface of the net is never defined! All that is given is the boundary of that surface: A certain square in the $y z$-plane.
   这个问题可能会让你感到奇怪的是，你需要斯托克斯定理的提示是，网的表面从未定义过！给出的只是那个表面的边界：$y z$平面中的一个特定的正方形。

8. If we can find a way to express $\mathbf{F}(x, y, z)$ as the curl of some other vector field, say $\mathbf{G}(x, y, z)$, we will be able to apply Stokes' theorem to this problem as follows:
   如果我们能找到一种方法将$\mathbf{F}(x, y, z)$表示为某个其他矢量场的旋度，比如$\mathbf{G}(x, y, z)$，我们将能够将斯托克斯定理应用到这个问题上，如下所示：
   $$
   \underbrace{\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) \cdot d \Sigma}_{\text {目标通量积分 }}=\underbrace{\iint_S(\nabla \times \mathbf{G}) \cdot \hat{\mathbf{n}} d \Sigma=\int_C \mathbf{G} \cdot d \mathbf{r}}_{\text {斯托克斯定理 }}
   $$

9. This is analogous to performing the integral $\int f(x) d x$ in single-variable calculus, where you have to find a new function with the property $g^{\prime}(x)=f(x)$, which then lets you compute the integral based on the boundary values. In this case, we are looking for the "anti-curl" of $\mathbf{F}$, so to speak, which will let us compute the surface integral based on the values of this anti-curl function on the boundary of the surface.
   这类似于在单变量微积分中执行积分$\int f(x) d x$，你必须找到一个新的函数，满足$g^{\prime}(x)=f(x)$的性质，然后让你可以基于边界值计算积分。在这种情况下，我们正在寻找$\mathbf{F}$的"反旋度"，可以说，这将让我们能够基于这个反旋度函数在表面边界上的值来计算表面积分。

--- pic\Stokes' theorem examples.pdf_11.png ---

10. Unlike single-variable calculus, not all vector fields $\mathbf{F}$ have such an anti-curl function. Luckily for us, this particular function is one of the special ones that do.
    不像单变量微积分，不是所有的矢量场$\mathbf{F}$都有这样的反旋度函数。幸运的是，对我们来说，这个特定的函数是其中的一个特殊的。

11. Concept check: Find a vector field $\mathbf{G}(x, y, z)$ satisfying the property $\nabla \times \mathbf{G}=\mathbf{F}$.
    概念检查：找到一个满足性质$\nabla \times \mathbf{G}=\mathbf{F}$的矢量场$\mathbf{G}(x, y, z)$。

12. Let $G_1, G_2$ and $G_3$ be the component function of $\mathbf{G}$ :
    让$G_1, G_2$和$G_3$是$\mathbf{G}$的组成函数：
    $$
    \mathbf{G}(x, y, z)=G_1(x, y, z) \hat{\mathbf{i}}+G_2(x, y, z) \hat{\mathbf{j}}+G_3(x, y, z) \hat{\mathbf{k}}
    $$

13. Next, just write out the definition of curl:
    接下来，只需写出旋度的定义：
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

14. Bringing in the definition of $\mathbf{F}$, this means the desired property that $\nabla \times \mathbf{G}=\mathbf{F}$ breaks down into the following three equations:
    引入$\mathbf{F}$的定义，这意味着所需的性质$\nabla \times \mathbf{G}=\mathbf{F}$分解为以下三个方程：
    $$
    \begin{aligned}
    & \frac{\partial G_3}{\partial y}-\frac{\partial G_2}{\partial z}=y^2 \\
    & \frac{\partial G_1}{\partial z}-\frac{\partial G_3}{\partial x}=z^2 \\
    & \frac{\partial G_2}{\partial x}-\frac{\partial G_1}{\partial y}=x^2
    \end{aligned}
    $$



--- pic\Stokes' theorem examples.pdf_12.png ---

1. Solving this is like solving a puzzle. You try some things, tweak them when they don't work, attempting all the while to keep things simple. After playing around a bit, you might find that the simplest strategy is as follows: Let $G_3$ take care of the entire first equation, $G_1$ take care of the entire second equation, and $G_2$ take care of the last equation. Specifically:
   解决这个问题就像解决一个谜题。你尝试一些方法，当它们不起作用时进行调整，一直试图保持简单。玩弄一会儿后，你可能会发现最简单的策略如下：让$G_3$处理整个第一个方程，$G_1$处理整个第二个方程，$G_2$处理最后一个方程。具体来说：
   $$
   \begin{aligned}
   & G_3=\frac{1}{3} y^3 \\
   & G_1=\frac{1}{3} z^3 \\
   & G_2=\frac{1}{3} x^3
   \end{aligned}
   $$

2. Or, written in the format requested in the question:
   或者，按照问题要求的格式写出来：
   $$
   \mathbf{G}(x, y, z)=\frac{1}{3} z^3 \hat{\mathbf{i}}+\frac{1}{3} x^3 \hat{\mathbf{j}}+\frac{1}{3} y^3 \hat{\mathbf{k}}
   $$

3. In a sense, we were lucky with this example, since there was enough symmetry that things didn't get complicated. In general, equations that are expressed using partial derivatives of a function can be very hard to solve. As in, one of them currently has a million dollar prize attached to it. The study of these sorts of equations goes under the name "Partial differential equations", which of course involves more sophisticated tactics than the guess-and-check approach I suggested for this one.
   从某种意义上说，我们在这个例子中很幸运，因为有足够的对称性使事情没有变得复杂。一般来说，使用函数的偏导数表示的方程可能很难解决。就像，其中一个目前有一百万美元的奖金。这类方程的研究被称为"偏微分方程"，当然，它涉及到比我为这个问题建议的猜测和检查方法更复杂的策略。

4. Step 3: Compute the line integral
   第三步：计算线积分

5. Given this construction for $\mathbf{G}$, the final step is to compute the right-hand-side line integral in our core equation:
   给定$\mathbf{G}$的这种构造，最后一步是计算我们核心方程中的右手边的线积分：
$$
\underbrace{\iint_S(\mathbf{F} \cdot \hat{\mathbf{n}}) \cdot d \Sigma}_{\text {目标通量积分 }}=\underbrace{\iint_S(\nabla \times \mathbf{G}) \cdot \hat{\mathbf{n}} d \Sigma=\overbrace{\int_C \mathbf{G} \cdot d \mathbf{r}}^{\text {现在计算这个。 }}}_{\text {斯托克斯定理 }}
$$


--- pic\Stokes' theorem examples.pdf_13.png ---

1. In this context, the curve $C$ represents the $2 \times 2$ square in the $y z$-plane with vertices at the following four points:
   在这个上下文中，曲线$C$表示$y z$平面中的$2 \times 2$正方形，其顶点在以下四点：
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

2. Before computing the line integral around this square, it needs to be oriented in a way that aligns with the orientation of the butterfly net surface $S$.
   在计算这个正方形周围的线积分之前，需要以一种与蝴蝶网表面$S$的方向对齐的方式进行定向。

3.  Concept check: Given that the butterfly net lies in the positive $x$-direction away from the square $C$, and is oriented with outward-facing unit normal vectors, how should $C$ be oriented so that Stokes' theorem can be applied? Answer this question from the perspective of standing on the positive $x$-axis, and looking directly at $C$.
    概念检查：给定蝴蝶网位于正$x$方向，远离正方形$C$，并且以面向外的单位法向量进行定向，那么应该如何定向$C$才能应用斯托克斯定理？从站在正$x$轴上，直接看$C$的角度来回答这个问题。

4.  Choose 1 answer:
    选择1个答案：


--- pic\Stokes' theorem examples.pdf_14.png ---

1. (B) Counterclockwise
   (B) 逆时针

2. Counterclockwise.
   逆时针。

3. As I mentioned in the answer to a similar question in the last example, there are several different ways to phrase the rule for this orientationalignment.
   正如我在上一个例子中对类似问题的回答中提到的，有几种不同的方式来表述这个定向对齐的规则。

4. If you look at the surface in such a way that the unit normal vectors are all pointed towards your face, the curve should be oriented counterclockwise.
   如果你以这样的方式观察表面，即单位法向量都指向你的脸，那么曲线应该是逆时针方向的。

5. The curve's orientation should follow the right-hand rule, in the sense that if you stick the thumb of your right hand in the direction of a unit normal vector near the edge of the surface, and curl your fingers, the direction they point on the curve should match its orientation.
   曲线的方向应该遵循右手规则，意思是如果你将右手的拇指指向表面边缘附近的单位法向量的方向，并卷曲你的手指，它们在曲线上指向的方向应该与其方向匹配。

6. When you are walking along the boundary curve with your body pointing out in the direction of the unit normal vector, you should be walking in such a way that the surface is to your left side.
   当你沿着边界曲线行走，你的身体指向单位法向量的方向时，你应该以这样的方式行走，即表面在你的左侧。

7. Concept check: Our construction of $\mathbf{G}$ looks like this:
   概念检查：我们的$\mathbf{G}$的构造如下：
   $$
   \mathbf{G}=\frac{1}{3}\left[\begin{array}{c}
   z^3 \\
   x^3 \\
   y^3
   \end{array}\right]
   $$

8. Given this, and given the orientation of the square $C$ that you just specified, finish the problem by computing the following line integral:
   给定这个，以及你刚刚指定的正方形$C$的方向，通过计算以下线积分来完成问题：
   $$
   \int_C \mathbf{G} \cdot d \mathbf{r}=
   $$


--- pic\Stokes' theorem examples.pdf_15.png ---

1.  First, draw out the square with its designated counterclockwise orientation in the $y z$-plane.
    首先，在$y z$平面上画出一个指定逆时针方向的正方形。

2.  Now think about the following line integral along each one of these sides:
    现在考虑沿着每一边的以下线积分：
    $$
    \int \frac{1}{3}\left[\begin{array}{c}
    z^3 \\
    x^3 \\
    y^3
    \end{array}\right] \cdot d \mathbf{r}
    $$

3.  Right side: While going up the right side, the tiny step vector $d \mathbf{r}$ is a step up in the $z$-direction.
    右侧：在向右侧上升时，微小的步长向量$d \mathbf{r}$是在$z$方向上的一个步长。
    $$
    d \mathbf{r}=\left[\begin{array}{c}
    0 \\
    0 \\
    d z
    \end{array}\right]
    $$

4.  Here's what this means for the integral:
    这对积分意味着什么：
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

5.  This integral is taken along the right side of the square, where the value of $y$ is constantly 1 , and $z$ has the bounds $z=-1$ and $z=1$. So our integral simplifies to this:
    这个积分是沿着正方形的右侧进行的，其中$y$的值始终为1，$z$的界限为$z=-1$和$z=1$。所以我们的积分简化为这个：
    $$
    \int_{-1}^1 \frac{1}{3}(1)^3 d z=\frac{2}{3}
    $$

--- pic\Stokes' theorem examples.pdf_16.png ---

1. Top side: When going left on the top side, the tiny step vector is
   顶部：当在顶部向左走时，微小的步长向量是
   $$
   d \mathbf{r}=\left[\begin{array}{c}
   0 \\
   -d y \\
   0
   \end{array}\right]
   $$

2. Since this line ranges from the values $y=-1$ to $y=1$, this means the line integral on this portion of the square becomes:
   由于这条线的范围是从$y=-1$到$y=1$，这意味着这个方形部分的线积分变为：
   $$
   \int_{-1}^1-\frac{1}{3} x^3 d y
   $$

3. Since $x$ is zero on this whole line (or the whole square for that matter), this integral is 0 .
   由于在整条线（或者整个正方形）上$x$都是零，所以这个积分是0。

4. Left side: Almost identical to the right side, except that $d z$ is negative and the constant value of $y$ is negative. These differences cancel out, so the integral on this side also ends up being $\frac{2}{3}$.
   左侧：几乎与右侧相同，只是$d z$为负，$y$的常数值为负。这些差异抵消了，所以这一侧的积分也最终变成了$\frac{2}{3}$。

5. Bottom side: Almost identical to the top side. It also becomes 0 .
   底部：几乎与顶部相同。它也变成了0。

6. All in all, then, the line integral adds up to $\frac{4}{3}$.
   总的来说，线积分加起来是$\frac{4}{3}$。

7. Summary
   总结

8. Stokes' theorem can be used to turn surface integrals through a vector field into line integrals.
   斯托克斯定理可以用来将通过矢量场的表面积分转化为线积分。

9. This only works if you can express the original vector field as the curl of some other vector field.
   只有当你能将原始矢量场表示为某个其他矢量场的旋度时，这才有效。

10. Make sure the orientation of the surface's boundary lines up with the orientation of the surface itself.
    确保表面边界的方向与表面本身的方向对齐。






