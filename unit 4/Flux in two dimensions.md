
--- pic\Flux in two dimensions.pdf_00.png ---

1. Flux in two dimensions
   二维的流量

2. How line integrals can measure flow rate through a curve. 
   线积分如何测量通过曲线的流量。

3. Learning this is a good foundation for Green's divergence theorem. 
   学习这个是理解格林散度定理的良好基础。

1. Background
背景

2. Line integrals in a scalar field
标量场中的线积分

3. Vector fields
向量场

4. What we're building to
我们正在构建的是什么

4. Given a region enclosed by a curve $C$, and a fluid flow determined by a vector field $F(x, y)$, the rate at which fluid is exiting that region (assuming it has density 1) can be measured with the following line integral:
   给定一个由曲线$C$包围的区域，并由矢量场$F(x, y)$确定的流体流动，流体退出该区域的速率（假设其密度为1）可以用以下的线积分来测量：

5. fluid mass in region
   区域内的流体质量

6. Here, $n(x, y)$ is some function that returns the outward unit normal vector at every point on the curve $C$.
   这里，$n(x, y)$是一个函数，它在曲线$C$上的每一点返回向外的单位法向量。

7. This integral $\int_C F \cdot n ds$ is called a flux integral, or sometimes a "two-dimensional flux integral", since there is another similar notion in three dimensions.
   这个积分$\int_C F \cdot n ds$被称为流量积分，或者有时候被称为"二维流量积分"，因为在三维中有一个相似的概念。

8. In any two-dimensional context where something can be considered flowing, such as a fluid, two-dimensional flux is a measure of the flow rate through a curve.
   在任何可以被认为有东西流动的二维环境中，比如流体，二维流量是通过曲线的流动率的一个度量。

1. In general, the curve isn't necessarily a closed loop.
一般来说，曲线并不一定是一个封闭的循环。

5. Changing fluid mass in a region
改变一个区域中的流体质量

6. Suppose you have some two-dimensional vector field, $F(x, y)$
假设你有一个二维向量场，$F(x, y)$

--- pic\Flux in two dimensions.pdf_01.png ---

1. And consider some closed curve C wandering through this field.
考虑一条在这个场中游荡的闭合曲线 $C$。

1. \triangle s we like to do with vector fields, let's say this represents some kind of fluid flow.
   我们喜欢用矢量场来做，让我们说这代表某种类型的流体流动。

2. But let's limit ourselves to thinking about what happens over a very small amount of time, just a quick instance really.
   但是让我们限制自己去想一想在非常短的时间内会发生什么，只是一个快速的实例。

3. For example, you can imagine each fluid particle moving from the tail of one of the vectors drawn above to its tip.
   例如，你可以想象每个流体粒子从上面绘制的向量的尾部移动到它的尖端。

4. Key question: How can we measure the instantaneous rate of change of the mass of fluid inside the region enclosed by $C$?
   关键问题：我们如何测量由$C$封闭区域内流体质量的瞬时变化率？

5. Specifically, let's say our fluid has a constant density throughout the plane, perhaps 1 kilogram per square meter.
   具体来说，让我们假设我们的流体在整个平面内具有恒定的密度，也许是每平方米1公斤。

6. If we let the fluid flow for a small amount of time, $\Delta t$, what is the total mass of fluid which leaves/enters the region?
   如果我们让流体流动一小段时间，$\Delta t$，那么离开/进入该区域的流体的总质量是多少？

7. The answer, of course, will be some function of the vector field $F$ and the curve $C$.
   答案当然会是矢量场$F$和曲线$C$的某个函数。

1. If this question reminds you of the intuition for divergence, it's for a very good reason.
如果这个问题让你想起了散度的直观理解，那是有很好的原因的。
 
8. In fact, in another article, we will use the formula we are now deriving to give the formal definition of divergence, and to show a special relationship divergence has with line integrals in two dimensions.
   实际上，在另一篇文章中，我们将使用我们现在正在推导的公式来给出散度的正式定义，并展示散度与二维线积分的特殊关系。

1. One bit of length at a time
一次处理一段长度。
 
9. One way to answer this question is to break up the curve into many tiny segments and consider how much fluid leaves or enters each segment.
   回答这个问题的一种方法是将曲线分解成许多小段，然后考虑每一段中有多少流体离开或进入。

10. If we zoom in on a small enough segment, we can basically treat it as a straight line, and the fluid particles going through it are pretty much all moving at the same speed and in the same direction.
    如果我们放大到足够小的一段，我们基本上可以将它视为一条直线，穿过它的流体粒子几乎都以相同的速度和方向移动。

--- pic\Flux in two dimensions.pdf_02.png ---

1. \triangle s we let the fluid flow for the small change in time $\Delta t$, the fluid passing through this segment will form a parallelogram.
   当我们让流体在$\Delta t$的小变化时间内流动时，通过这个部分的流体将形成一个平行四边形。

1. I happened to draw a case where the fluid is going out of the region, but you could just as easily imagine the fluid coming into the region if the velocity vectors at that point were turned the other way.
我恰好画了一个流体从区域中流出的情况，但是如果在那一点的速度向量反向，你同样可以轻易地想象流体进入该区域。

1. Since we are assuming a uniform density of $1 \, \text{kg/m}$ for the fluid, the mass of fluid leaving the region equals the area of this parallelogram.
由于我们假设流体的均匀密度为$1 \, \text{kg/m}$，所以离开该区域的流体质量等于这个平行四边形的面积。

1. Let's break down that area.
让我们分解那个区域。

1. The base of the parallelogram is the length of our tiny segment.
   平行四边形的底是我们微小部分的长度。

2. Let's call that $\Delta s$.
   我们称之为$\Delta s$。

3. The displacement vector of a fluid particle which starts at some point on the tiny segment will be $v\Delta t$, where $v$ is the velocity vector of fluid at that point, and $\Delta t$ is the amount of time the fluid flowed.
   从微小部分上的某一点开始的流体颗粒的位移矢量将是$v\Delta t$，其中$v$是该点处流体的速度矢量，$\Delta t$是流体流动的时间。

4. The height of the parallelogram will be the component of the $v\Delta t$ displacement vector which is perpendicular to the segment.
   平行四边形的高度将是垂直于段的$v\Delta t$位移矢量的分量。

5. You can extract this by taking the dot product between $v\Delta t$ and a unit normal vector to the curve $C$.
   你可以通过取$v\Delta t$与曲线$C$的单位法向量之间的点积来提取这个。

6. Let's name that unit normal vector $n$.
   让我们把那个单位法向量叫做$n$。

7. Concept check: What is the total mass exiting the tiny segment of length $\Delta s$ over the short time $\Delta t$?
   概念检查：在短时间$\Delta t$内，长度为$\Delta s$的小段中流出的总质量是多少？

--- pic\Flux in two dimensions.pdf_03.png ---

1. The first choice is correct: 
   第一个选择是正确的：

1. Take a look at the diagram above.
   看看上面的图。

2. The base of the parallelogram has length $\triangle s$, and the height is $(v \cdot n) \triangle t$.
   平行四边形的底长度是$\triangle s$，高度是$(v \cdot n) \triangle t$。

3. Multiplying these together, we get the area.
   将这两者相乘，我们得到面积。

1. Since we are assuming a fluid density of $1 \, \text{kg/m}$, this area equals the exiting mass.
由于我们假设的流体密度为 $1 \, \text{kg/m}$，这个面积等于流出的质量。

2. Dividing out by $\triangle t$, we have the amount of mass passing through this tiny line segment per unit time:
除以$\triangle t$，我们得到的是每单位时间通过这个微小线段的质量量：

4. Exiting mass per unit time = $(v - n)(\triangle s)$
   单位时间内流出的质量 = $(v - n)(\triangle s)$


1. Bringing it together with an integral
将其与积分结合起来

1. Now think about all of the tiny segments which make up the curve $C$, each with a tiny amount of mass exiting or entering through it per unit time.
   现在考虑一下构成曲线$C$的所有微小段，每个段在单位时间内都有微小的质量通过它流出或流入。

2. If you want to add up all those tiny changes in mass along the curve, what better tool is there than a line integral?
   如果您想要沿着曲线累加所有这些微小的质量变化，有什么比线积分更好的工具呢？


1. Specifically, the line integral will look like this:
具体来说，线积分将如下所示：

--- pic\Flux in two dimensions.pdf_04.png ---

1. The vector field $\mathbf{F}(x, y)$ gives the fluid velocity at each point along the curve.
   向量场 $\mathbf{F}(x, y)$ 给出了曲线上每一点的流体速度。

2. The term $n$ should be considered a function, $n(x, y)$, which takes in a point on $C$ and outputs the unit normal vector to $C$ at that point.
   项 $n$ 应被视为一个函数，$n(x, y)$，它接受一个在 $C$ 上的点，并输出在那一点 $C$ 的单位法向量。

3. Using the symbol $\oint$ instead of $\int$ Is just to emphasize that the line integral is around a closed loop.
   使用符号 $\oint$ 代替 $\int$ 只是为了强调线积分是环绕一个封闭循环的。

1. $ds$ indicates a tiny change in arc length along the curve.
$ds$ 表示曲线上弧长的微小变化。

4. Conceptually it is no different from the $\text{d}s$ term in the previous section, but now we are considering it as an infinitesimal quantity used for integration.
   在概念上，它与前一节的 $\text{d}s$ 项没有什么不同，但现在我们将它视为用于积分的无穷小量。

5. As you walk along the curve $C$, the value $F \cdot n$ measures how much the fluid is leaving/entering the region enclosed by $C$ at each point.
   当你沿着曲线 $C$ 走时，值 $F \cdot n$ 测量的是每一点流体离开/进入由 $C$ 包围的区域的程度。

6. It is positive when the fluid is leaving, and negative when the fluid flows in, so the integral as a whole will return the total mass leaving the region enclosed by $C$ per unit time.
   当流体离开时，它是正的；当流体流入时，它是负的，所以积分作为一个整体将返回每单位时间离开 $C$ 包围的区域的总质量。

7. More elaborately, you might write:
   更详细地，你可以写作：

1. Fluid mass in region
   区域内的流体质量

8. Rate at which mass leaves region
区域内质量离开的速率

2. Mass leaving each region tiny piece of size $ds$
   每个区域离开的质量微小部分的大小为$ds$

1. Definition: This flow rate through a curve is called flux.
   定义：通过曲线的流速被称为通量。

2. More specifically, I should say the component of the flow rate which is perpendicular to the curve is called flux.
   更具体地说，我应该说垂直于曲线的流速分量被称为通量。

2. Many things other than fluids in physics are considered to "flow", such as heat, and (loosely speaking) the electromagnetic field, and the word flux is used very broadly in reference to any one of these circumstances.
   物理学中除了流体外，许多其他东西都被认为是"流动"的，比如热量，（宽泛地说）电磁场，词"通量"被广泛用于参考这些情况中的任何一种。

1. It's most common for the word "flux" to refer to flow rate through a surface in three-dimensions.
   "通量"这个词最常用来指的是通过三维表面的流速。

2. As such, you might call this flow rate through a curve "two-dimensional flux".
   因此，你可能会称这种通过曲线的流速为"二维通量"。

3.  This integral $\oint_C F \cdot n \, ds$ is sometimes called a "flux integral", and as with all new operations, the best way to get a feel for it is to work through an example.
    这个积分 $\oint_C F \cdot n \, ds$ 有时被称为"通量积分"，就像所有新的操作一样，最好的理解方法是通过一个例子来理解。

4. Example: Flux through a circle
示例：通过圆形的通量

--- pic\Flux in two dimensions.pdf_05.png ---

1. Consider the vector field.
   考虑向量场。

1. And draw a circle of radius 3 centered at the origin.
在原点处画一个半径为3的圆。

1. From this picture, you might be able to guess that the fluid flowing along this vector field tends to go out of the circle. 
   从这幅图中，你可能会猜测沿着这个矢量场流动的液体倾向于流出圆形。

2. But how much? 
   但是有多少？

3. To apply the integral from the last section, we first need to do two things: parameterize the circle. 
   要应用上一节的积分，我们首先需要做两件事情：参数化圆形。

4. Find a function for $n$ on the circle. 
   找到圆上的$n$的函数。

5. We parameterize the circle using our friendly neighborhood cosine-sine parameterization:
   我们使用我们熟悉的余弦-正弦参数化法来参数化圆形：

6. This draws a circle with radius 3. 
   这会画出一个半径为3的圆形。

7. For the parameterization to traverse the circle once and only once, let $t$ range from 0 to $2\pi$. 
   为了让参数化只遍历一次圆形，让$t$的范围从0到$2\pi$。

8. Which of the following functions gives the unit normal vector? 
   下面哪个函数给出了单位法向量？

--- pic\Flux in two dimensions.pdf_06.png ---

1. Let $(x, y)$ be some point on the circle.
   让$(x, y)$成为圆上的某个点。

2. The normal vector to the circle at that point will be oriented in the same direction as the vector $\begin{bmatrix} x \\ y \end{bmatrix}$.
   在那个点上的圆的法向量将与向量$\begin{bmatrix} x \\ y \end{bmatrix}$的方向一致。

2. However, the vector $\begin{bmatrix} x \\ y \end{bmatrix}$ has magnitude 3, since our circle is defined to have radius 3, so we must scale this down by a factor of 3 to get a unit normal vector.
   然而，由于我们定义的圆的半径为3，所以向量$\begin{bmatrix} x \\ y \end{bmatrix}$的大小为3，因此我们必须将其缩小3倍以获得单位法向量。

1. We can now apply this data to the line integral we found in the last section.
   我们现在可以将这些数据应用到我们在上一节中找到的线积分。

2. If you are uncomfortable with the computation of the line integral, consider reviewing the article on line integrals in a scalar field.
   如果你对线积分的计算感到不舒服，可以考虑复习一下关于标量场中线积分的文章。

以下是处理你提供的段落的结果：

--- pic\Flux in two dimensions.pdf_07.png ---

1. Once you have an integral in this form, you can just plug it into a calculator (or something like Wolfram Alpha) to get the numerical result.
   一旦你有了这种形式的积分，你可以直接将其输入计算器（或像Wolfram Alpha这样的工具）得到数值结果。

2. Computing a unit normal vector
   计算单位法向量。

3. You might be wondering how to compute the unit normal vector $\mathbf{n}(x, y)$ for an arbitrary curve that is given to you.
   你可能会想知道如何计算给定的任意曲线的单位法向量 $\mathbf{n}(x, y)$。

4. It felt like kind of a special case for the circle, didn't it?
   对于圆形，感觉是一种特殊情况，不是吗？

5. Well, luckily for you, constructing such a unit normal vector just so happens to be the topic of the next article.
   好在，恰好构建这样的单位法向量就是下一篇文章的主题。

1. I actually kind of lied to you when I said the unit normal vector is given with a function $n(x, y)$ with inputs on the $xy$-plane.
实际上，当我说单位法向量是由函数 $n(x, y)$ 给出，其输入在 $xy$ 平面上时，我有点对你撒谎了。

6. In practice, it is typically given as a parametric function $\mathbf{n}(t)$ that "lines up" with the parameterization of the curve $C$.
   在实践中，它通常被给定为一个参数函数 $\mathbf{n}(t)$，它与曲线 $C$ 的参数化"对齐"。

7. In principle, you should still think of it as acting on points in the $xy$-plane, it's just that in practice you only end up defining it for points on the curve $C$ itself, since that's all you need.
   从原则上讲，你仍应将其视为在$xy$平面上的点上起作用，只是在实践中，你只需为曲线 $C$ 自身上的点定义它，因为你只需要那样做。

8. Don't worry, you'll see what I mean in the next article.
   不用担心，你会在下一篇文章中看到我说的意思。

9. Summary: In any context where something can be considered flowing, such as a fluid, two-dimensional flux is a measure of the flow rate through a curve.
   总结：在任何可以考虑某物流动的情况下，比如流体，二维通量是通过曲线的流速的度量。

10. The flux over the boundary of a region can be used to measure whether whatever is flowing tends to go into or out of that region.
    区域边界上的通量可以用来测量流动的物质是否倾向于进入或离开该区域。

11. The flux through a curve $C$ can be measured with the line integral $\int_C F \cdot n ds$.
通过曲线 $C$ 的通量可以用线积分 $\int_C F \cdot n ds$ 来测量。



1. where $F(x, y)$ defines the vector field which indicates the flow rate.
其中，$F(x, y)$ 定义了表示流速的矢量场。

1. $n$ is some function which return the outward unit normal vector at every point on the curve $C$.
$n$ 是某个函数，它在曲线 $C$ 上的每一点返回向外的单位法向量。