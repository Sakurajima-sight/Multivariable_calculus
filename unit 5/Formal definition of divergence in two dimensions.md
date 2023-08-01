
--- pic\Formal definition of divergence in two dimensions.pdf_00.png ---

1. Formal definition of divergence in two dimensions
   二维散度的正式定义

2. Learn how line integrals are used to formalize the idea of divergence. 
   学习线积分是如何用来形式化散度概念的。

3. Background: Divergence, Flux in two dimensions
   背景：散度，二维通量

1. If you haven't already, you may also want to read "Why care about the formal definitions of divergence and curl" for motivation.
   如果你还没有阅读过，你可能也想阅读"为什么要关心散度和旋度的正式定义"以获取动力。

5. What we're building to
   我们正在构建的是什么

6. In two dimensions, divergence is formally defined as follows:
   在二维中，散度的正式定义如下：

2. 2d-flux through $C$ 
   通过 $C$ 的二维通量

7. Flux per unit area
   单位面积的通量

8. $F(x, y)$ is a two-dimensional vector field. 
   $F(x, y)$ 是一个二维矢量场。

1. $(x, y)$ is a specific point on the $xy$-plane.
   $(x, y)$ 是 $xy$ 平面上的一个特定点。

2. $A_{(x, y)}$ is some region of the $xy$-plane which includes the point $(x, y)$. For example, you can think of this as being a circle centered at $(x, y)$.
   $A_{(x, y)}$ 是 $xy$ 平面上的某个区域，包含点 $(x, y)$。例如，你可以将其视为以 $(x, y)$ 为中心的圆。

3. $|A_{(x, y)}|$ is the area of $A_{(x, y)}$.
   $|A_{(x, y)}|$ 是 $A_{(x, y)}$ 的面积。

4. $\lim_{|A_{(x, y)}| \to 0}$ indicates that we are considering the limit as the area $|A_{(x, y)}|$ goes to zero. In other words, as $A_{(x, y)}$ shrinks around the point $(x, y)$.
   $\lim_{|A_{(x, y)}| \to 0}$ 表示我们正在考虑当面积 $|A_{(x, y)}|$ 趋向于零时的极限。换句话说，就是当 $A_{(x, y)}$ 在点 $(x, y)$ 周围收缩时。

9.  $C$ is the boundary of $A_(x,y)$.
    $C$ 是 $A_(x,y)$ 的边界。

5. $n{(x, y)}$ is a function which gives an outward-facing unit normal vector at each point on $C$.
   $n{(x, y)}$ 是一个函数，它在 $C$ 上的每一点给出一个向外的单位法向量。

--- pic\Formal definition of divergence in two dimensions.pdf_01.png ---

1. The line integral $\oint_C F \cdot n ds$ represents the two-dimensional flux of $F$ through $C$.
   线积分$\oint_C F \cdot n ds$代表了$F$通过$C$的二维通量。

2. There ts a lot going on in this definition, but we will build up to it one piece at a time.
   这个定义中有很多内容，但我们会一步步地解构它。

3. The bulk of the intuition comes from the background understanding of flux.
   大部分的直觉来自对通量背景的理解。

1. Vector field $F$ .
矢量场$F$。

4.  Outward flow" at a point doesn't really make sense.
   在一点的"外流"真的没有意义。

5. By this point you should have some idea of what divergence Is trying to measure.
   到此为止，你应该对散度尝试度量什么有一些了解。

6. When a vector field $F(x, y)$ represents a fluid flow, divergence measures the tendency for the fluid to flow away from each point.
   当一个矢量场$F(x, y)$表示流体流动时，散度测量流体从每个点流出的趋势。

7. Simple positiveadiverdence example.
   简单的正散度示例。

8. However, there's a disconnect between the idea of "outward flow" and divergence itself: 
   然而，"外向流"的概念和散度本身之间存在一种脱节：

1. Divergence Is a function which takes in individual points in space.
散度是一个接受空间中单个点的函数。

1. The idea of outward flow only makes sense with respect to a region in space.
   对于空间中的一个区域，流出的概念才有意义。

--- pic\Formal definition of divergence in two dimensions.pdf_02.png ---

1. You can ask if a fluid flows out of a given region or into it, but it doesn't make sense to talk about fluid flowing out of a single point.
   你可以询问流体是否从给定区域流出或流入，但是讨论流体从单一点流出没有意义。

2. Formally defining divergence will involve using a flux integral, which measures the outward flow in a region, then taking the appropriate limit as this region shrinks around a specific point.
   正式定义散度将涉及使用流通量积分，该积分测量区域内的外流，然后当此区域围绕特定点缩小时，取适当的极限。

1. From a region to a point
 从区域到点

3.  In the article on two-dimensional flux, we had the following setup: 
   在关于二维流量的文章中，我们有以下设置：

4. Vector field $F$ .
矢量场$F$。

1. $F(x, y)$ is a vector-valued function representing the velocity vector field of some fluid.
   $F(x, y)$是一个向量值函数，表示某种流体的速度向量场。

2. $C$ is a closed loop in the $xy$-plane.
   $C$是$xy$平面中的一个闭环。

1. $n ( x , y )$ is a function that gives the outward unit normal vector at all points on the curve $C$.
   $n ( x , y )$ 是一个函数，它在曲线 $C$ 上的所有点给出向外的单位法向量。

3. I talked about how if you were tracking the mass of fluid in the region enclosed by the curve $C$, you could compute the rate at which mass is leaving the region using the following line integral:
   我讨论了如果你在追踪由曲线 $C$ 所围成的区域内的流体质量，你可以使用以下线积分来计算质量离开区域的速率：

4. fluid mass in region
流体质量在区域

1. Rate at which mass leaves region
质量离开区域的速率

1. Flux integral
流通量积分


2. This is called a "flux integral". If it is positive, fluid tends to be exiting the region, otherwise it tends to be entering the region.
   这被称为“通量积分”。如果它是正的，流体倾向于离开该区域，否则倾向于进入该区域。

3. You can interpret this integral by imagining walking along the boundary $C$ and measuring how much fluid tends to be exiting/entering the region at each point.
   你可以通过想象沿着边界$C$行走并测量每个点处流体倾向于退出/进入该区域的多少来解释这个积分。

4. What if instead of measuring the change of mass, you wanted to know the change in density? Well, just divide this integral by the area of the region in question.
   如果你想知道密度的变化，而不是测量质量的变化呢？那么，只需将此积分除以所讨论区域的面积。

5.  Let's go ahead and give that region a name, $A$, and say that $|A|$ is the area of the region.
    我们继续给那个区域一个名字，$A$，并说$|A|$是该区域的面积。

--- pic\Formal definition of divergence in two dimensions.pdf_03.png ---

1. (fluid density in region).
   （区域中的流体密度）。

2. Change in mass per unit area in $A$.
   在区域$A$中单位面积的质量变化。

3. To formally define divergence of $F$ at a point $(x, y)$, we consider the limit of this change in density as the region shrinks around the point $(x, y)$.
   为了正式定义点$(x, y)$处$F$的散度，我们考虑随着区域在点$(x, y)$周围收缩，这种密度变化的极限。

4. There is no set-in-stone notation for this, but here's what I'll go with: 
   对此并没有固定不变的记号，但这是我将要使用的：

1. Rather than just writing $A$, write  $A_{(x, y)}$ to emphasize that this region contains a specific point $(x, y)$.
   不是仅仅写 $A$，而是写 $A_{(x, y)}$ 来强调这个区域包含一个特定的点 $(x, y)$。

2. This is important because as we start letting the region shrink, we don't want it to wander away from the point.
当我们开始让区域收缩时，这很重要，因为我们不希望它离开这个点。

1. The expression "$\left|A_{(x, y)}\right| \to 0$" will indicate that we are considering the limit as the area of $A_{(x, y)}$ goes to $0$, meaning $A_{(x, y)}$ is shrinking around the point $(x, y)$. 
   表达式 “$\left|A_{(x, y)}\right| \to 0$” 表示我们正在考虑 $A_{(x, y)}$ 的面积趋近于 $0$ 的极限，意味着 $A_{(x, y)}$ 在点 $(x, y)$ 周围收缩。

1. With all this, here's how we write the formal definition of divergence:
有了所有这些，我们可以如此写出散度的正式定义：

1. Negative change of fluid density in $A(x, y)$.
   $A(x, y)$中流体密度的负变化。

1. Region is shrinking around $(x, y)$.
   区域在 $(x, y)$ 周围收缩。

2. Flux through $C$.
   通过 $C$ 的通量。

1. "Simple" example: Constant divergence 
   "简单"的例子：常数散度

3. Unlike other topics, the purpose of an example here is not to practice a skill that you will need.
与其他主题不同，这里一个例子的目的不是为了练习你将需要的技能。

4. It is just to get a feel for what this relatively abstract definition actually looks like with a concrete function.
它只是为了让你感觉到这个相对抽象的定义在具体函数中实际上是什么样子。

4.  Let's use the quintessential "outward flowing" vector field in two dimensions:
    让我们使用二维中典型的“向外流动”的向量场：

--- pic\Formal definition of divergence in two dimensions.pdf_04.png ---

1. Concept check: Using the usual divergence formula, the one which arises from the notation $\nabla \cdot \mathbf{F}$, what is the divergence of $F(x, y) = \begin{bmatrix} x \\ y \end{bmatrix}$?
   概念检查：使用通常的散度公式，这个公式源于符号$\nabla \cdot \mathbf{F}$，那么$F(x, y) = \begin{bmatrix} x \\ y \end{bmatrix}$的散度是什么？


2. Using the divergence formula, we can see that the divergence happens to be a constant 2 everywhere in the plane: 
   使用散度公式，我们可以看到在平面上的任何地方散度恰好是常数2：

3. Now let's see how the formal definition of divergence works in this case.
   现在让我们看看在这种情况下散度的正式定义是如何工作的。

4. Let's focus on the origin.
   让我们集中在原点。

5. And for our shrinking regions around this point, consider circles.
   而对于围绕这个点的缩小的区域，考虑圆形。

6. Let $C_r$ denote a circle o  f radius $r$ centered at the origin, and $D_r$ represent the region enclosed by that circle, where $D$ stands for "Disk".
   设$C_r$表示以原点为中心的半径为$r$的圆，$D_r$表示该圆所围成的区域，其中$D$代表"Disk"。

--- pic\Formal definition of divergence in two dimensions.pdf_05.png ---

1. Notice, for all values of $r$, the disk $D_r$ will contain the point $(0,0)$, so this is indeed a good family of regions to use.
   注意，对于所有的$r$值，磁盘$D_r$都将包含点$(0,0)$，所以这确实是一个好的区域集合来使用。

2. The formal definition of divergence at $(0,0)$ would then be written as follows: 
   在$(0,0)$处散度的正式定义则可以写为：

3. This is rather abstract, so let's start filling in the details of this integral.
   这是相当抽象的，所以让我们开始填写这个积分的细节。

4. Concept check: What is $|D_r|$?
   概念检查：什么是$|D_r|$？

5. The area of a disk with radius $r$ is 
   半径为$r$的圆盘的面积是

6. Concept check: Which of the following parameterizes $C_r$? 
   概念检查：以下哪个参数化了$C_r$？

1. $\begin{bmatrix} r\cos(t) \\ r\sin(t) \end{bmatrix}$ as $t$ ranges from $0$ to $2\pi$.
   当 $t$ 的范围从 $0$ 到 $2\pi$ 时，$\begin{bmatrix} r\cos(t) \\ r\sin(t) \end{bmatrix}$。

--- pic\Formal definition of divergence in two dimensions.pdf_06.png ---

1. The second answer choice is correct: 
   第二个答案选择是正确的：

1. $\begin{bmatrix} r\cos(t) \\ r\sin(t) \end{bmatrix}$ as $t$ ranges from $0$ to $2\pi$.
   当 $t$ 的范围从 $0$ 到 $2\pi$ 时，$\begin{bmatrix} r\cos(t) \\ r\sin(t) \end{bmatrix}$。

2. We start with the usual parameterization of a unit circle, using the expression: 
   我们从常规的单位圆参数化开始，使用表达式：

1. $\begin{bmatrix} \cos(t) \\ \sin(t) \end{bmatrix}$ as $t$ ranges from $0$ to $2\pi$.
   当 $t$ 的范围从 $0$ 到 $2\pi$ 时，$\begin{bmatrix} \cos(t) \\ \sin(t) \end{bmatrix}$。

1. Then we scale it by the radius $r$.
然后我们按半径$r$进行缩放。

3. Concept check: Using this parameterization, what should we replace $ds$ with in the integral $\int_{C_r} \dots ds$?
   概念检查：使用这种参数化，我们应该用什么替换积分$\int_{C_r} \dots ds$中的$ds$？

4. If you are unfamiliar with this step, consider reviewing the articles on line integrals or arc length.
   如果你对这一步不熟悉，可以考虑复习关于线积分或弧长的文章。

5. The value $ds$ represents a tiny bit of arc length on the curve $C$.
值$ds$表示曲线$C$上的一小段弧长。

6. Start by taking the derivative of the function parameterizing $C$:
从对参数化$C$的函数求导开始：

1. Then take its magnitude: 
然后取其大小：

1. When you multiply this by $dt$, it gives you a little snippet of arc length:
   当你将其乘以$dt$时，它会给你一小段弧长：

--- pic\Formal definition of divergence in two dimensions.pdf_07.png ---

1. Concept check: Which of the following gives an outward facing unit normal vector $n$ to $C_r$.
   概念检查：以下哪项给出了指向 $C_r$ 外侧的单位法向量 $n$。

2. The first answer choice is correct: 
   第一个答案选项是正确的：

3. Consider a point $(x, y)$ on the circle $C_r$.
考虑圆$C_r$上的一个点$(x, y)$。

4. The vector $\begin{bmatrix} x \\ y \end{bmatrix}$ not only points from the origin to $(x, y)$, it also gives a normal vector at that point.
   向量 $\begin{bmatrix} x \\ y \end{bmatrix}$ 不仅指向原点到 $(x, y)$ 的方向，它还给出了该点的法向量。

4. However, since $(x, y)$ is on the circle with radius $r$, the magnitude of this vector is $r$.
然而，由于$(x, y)$在半径为$r$的圆上，所以这个向量的大小为$r$。

5. To get a unit normal vector, we must divide each component by $r:
要得到单位法向量，我们必须将每个分量除以$r$：   

--- pic\Formal definition of divergence in two dimensions.pdf_08.png ---

1. Applying all these answers to the expression we had before, here's what we get: 
   将所有这些答案应用到我们之前的表达式中，我们得到了：

2. So the formal definition does actually match the formula $\nabla \cdot F$ that we know and love.
所以，正式定义实际上与我们所知道和喜欢的公式$\nabla \cdot F$匹配。

3. Well, at least for this specific example anyway.
至少对于这个具体的例子来说是这样。

3. But the point of this formal definition is not to use it for actual computations.
但是这个正式定义的重点不在于将其用于实际的计算。

4. The point is that it does a much better job reflecting the idea of "outward fluid flow" in a mathematical formula.
重点是它在反映"向外流动流体"的概念的数学公式方面做得更好。

5. Having such a solid grasp of that idea will be helpful when you learn about Green's divergence theorem.
当你学习关于格林散度定理时，对这个概念有一个坚实的理解将会很有帮助。

4. What about higher dimensions?
   那么更高维度呢？

--- pic\Formal definition of divergence in two dimensions.pdf_09.png ---

1. In the next article, I'll show how you can do essentially the same thing to define three-dimensional divergence using three-dimensional flux, which involves a surface integral.
   在下一篇文章中，我将展示如何使用三维通量来定义三维散度，这涉及到一个表面积分。

2. Summary.
   总结。

3. Given a fluid flow, divergence tries to capture the idea of "outward flow" at a point.
   对于一个流体流动，散度试图捕捉点处"外向流"的概念。

4. But this doesn't quite make sense, because you can only measure the change in fluid density of a region.
   但这并不完全有意义，因为你只能测量区域内流体密度的变化。

5. When talking about a region, the idea of "outward flow" is the same as flux through that region's boundary.
   当我们谈论一个区域时，"外向流"的概念就等同于通过该区域边界的通量。

6. To adapt the idea of "outward flow in a region" to the idea of "outward flow at a point’, start by considering the average outward flow per unit area in a region.
   为了将"区域内的外向流"的概念适应为"点上的外向流"的概念，首先考虑区域内单位面积的平均外向流。

7. This just means dividing the flux integral by the area of the region.
   这就意味着将通量积分除以区域的面积。

8. Next, consider the limit of this outward flow per unit area as the region shrinks around a specific point.
   接下来，考虑当区域围绕一个特定点缩小时，单位面积的这种外向流的极限。

9. Putting this all into symbols, we get the following definition of divergence:
   把所有这些都转化为符号，我们得到了散度的下列定义：

10. 2d-flux
   二维流量

11. Flux per unit area
   单位面积的流量
