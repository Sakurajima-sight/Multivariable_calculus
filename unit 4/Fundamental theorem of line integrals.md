
--- pic\Fundamental theorem of line integrals.pdf_00.png ---

1. Fundamental theorem of line integrals
    基本线积分定理

2. Also known as the Gradient Theorem, this generalizes the fundamental theorem of calculus to line integrals through a vector field.
    也被称为梯度定理，这将微积分的基本定理推广到通过矢量场的线积分。

3. Background
    背景

4. The gradient
    梯度

5. Line integrals in a vector field
    矢量场中的线积分

6. Only needed if you want to understand the proof: e Multivariable chain rule.
    只有当你想理解证明时才需要：多变量链式法则。

7. What we're building to.
    我们正在构建的。

8. The fundamental theorem of line integrals, also called the gradient theorem, states that:
线积分的基本定理，也称为梯度定理，状态为：

1. The intuition behind this formula is that each side represents the change in the value of a multivariable function $f$ as you walk along a path parameterized by $\vec{r}(t)$.
这个公式背后的直觉是，当你沿着由 $\vec{r}(t)$ 参数化的路径行走时，每一侧都代表了多变量函数 $f$ 的值的变化。

1. This formula implies that gradient fields are path-independent, meaning the line integrals along any two paths connecting the same start and end points will be equal.
这个公式意味着梯度场是路径无关的，意味着沿着连接同一起点和终点的任何两条路径的线积分将相等。

1. Statement of the theorem 
定理的陈述

1.  Recall that the fundamental theorem of calculus in the single-variable world states that:
单变量世界中的微积分基本定理声明：
$\int_a^b g'(x) \, dx = g(b) - g(a)$

1.  In some sense, this says that integration is the opposite of differentiation.
在某种意义上，这说积分是微分的反义。

--- pic\Fundamental theorem of line integrals.pdf_01.png ---

1. The fundamental theorem of line integrals, also known as the gradient theorem, is one of several ways to extend this theorem into higher dimensions.
线积分的基本定理，也被称为梯度定理，是将这个定理扩展到更高维度的几种方式之一。

13. In a sense, it says that line integration through a vector field is the opposite of the gradient.
在某种意义上，它说通过矢量场的线积分是梯度的反义。

14. The statement of the theorem is:
定理的陈述是：

15. Where $f$ is some scalar-valued multivariable function.
其中 $f$ 是某个标量值的多变量函数。

16. $\nabla f$ is the gradient of $f$.
$\nabla f$ 是 $f$ 的梯度。

1. $r(t)$ is a vector-valued function which parameterizes some path through the input space of $f$.
$r(t)$ 是一个向量值函数，它通过 $f$ 的输入空间参数化某条路径。

2. $r(a)$ and $r(b)$ are the end points of the path.
$r(a)$ 和 $r(b)$ 是路径的端点。

3. $r'(t)$ is the derivative of $r(t)$, taken component-wise as usual.
$r'(t)$ 是 $r(t)$ 的导数，像往常一样按组件取。

1. You might also see this theorem written without reference to the parameterization $r(t)$ as follows: 
   你也可能看到这个定理的另一种写法，不引用参数化$r(t)$，如下：
   
2. Where $C$ represents the path through space, with $A$ as its starting point and $B$ as its ending point, and $ds$ is thought of as a tiny step along $C$.
   其中$C$表示通过空间的路径，$A$是它的起点，$B$是它的终点，$ds$被认为是沿$C$的一个微小步长。

3. In short, the theorem states that the line integral of the gradient of a function $f$ gives the total change in the value of $f$ from the start of the curve to its end.
   简而言之，定理表述说，函数$f$的梯度的线积分给出了从曲线的起点到终点$f$的值的总变化。

4. The intuition
直觉

4. The meaning behind this formula is actually fairly straightforward, once we take some time to digest the meaning of each term.
   一旦我们花些时间消化每个术语的含义，这个公式背后的意义实际上是相当直接的。

5. There are two main players on the stage right now:
   现在舞台上有两个主角：

1. A path wandering through space (let's say two-dimensional space, for now, to make drawing easier).
一条在空间中漫游的路径（为了方便画图，我们现在先假设是二维空间）。

5. A function $f$ which takes in points of that path as its input, and outputs a number.
一个函数 $f$，它将路径上的点作为输入，并输出一个数字。

--- pic\Fundamental theorem of line integrals.pdf_02.png ---

1. Think about how the value of the function $f$ changes as we walk along the path.
想想当我们沿着路径走时，函数 $f$ 的值是如何变化的。

1.  The following video shows one way to visualize this, where the graph of some function $f$ is shown in blue, a path in the $xy$-plane is shown in red, and the projection of that path onto the graph is also shown in red. 
下面的视频显示了一种可视化的方法，其中一些函数 $f$ 的图在蓝色中显示，$xy$-plane 的路径在红色中显示，该路径在图上的投影也在红色中显示。

1.  Tracing a path and following the projection on a graph 
跟踪路径并跟随图表上的投影

1.  Think about the height of this graph above each point on the path. 
想想这个图在路径上每个点上方的高度。

1.  How could you mathematically keep track of the change in this height as we walk along the path. 
当我们沿着路径行走时，你如何用数学方式跟踪这个高度的变化。

1.  Instead of projecting the path onto the graph of $f$, we could also overlay it with the gradient field of $f$ (the vector field where each vector represents $\nabla f$).
我们可以不把路径投影到 $f$ 的图上，而是用 $f$ 的梯度场（每个向量都代表 $\nabla f$ 的向量场）覆盖它。

--- pic\Fundamental theorem of line integrals.pdf_03.png ---

1. Let's write down the gradient theorem again:
让我们再次写下梯度定理：

1. The next few questions will have you reason through the left-hand side of this expression.
下几个问题将让你推理出这个表达式的左边。

1. Concept check 1: If we think of $dt$ as a very slight change to the parameter $t$, how can you interpret the vector $\vec{r}'(t)\,dt$?
概念检查 1：如果我们把 $dt$ 看作是对参数 $t$ 的微小变化，你怎么解释向量 $\vec{r}'(t)\,dt$？

1. A tiny step along the path. 
路径上的一个微小步骤。

1. The vector $r'(t)dt$ gives a tiny step along the path.
向量 $r'(t)dt$ 给出了路径上的一个微小步长。

1. This is the motion in the $xy$-plane which results from a slight nudge of size $dt$ to the parameter $t$.
这是由于参数 $t$ 的微小挤压而在 $xy$ 平面上产生的运动。

1. Alternatively, you can think of $\vec{r}'(t)$ as a velocity vector of a particle whose position as a function of time is given by $\vec{r}(t)$.
或者，你可以把 $\vec{r}'(t)$ 看作是一个粒子的速度向量，该粒子的位置是由 $\vec{r}(t)$ 给出的时间函数。

1. Multiplying this velocity vector by the tiny change in time $dt$ gives a tiny change in position, which in this case is a little step along the curve.
把这个速度向量和时间 $dt$ 的微小变化相乘，就得到了位置的微小变化，这在本例中是沿着曲线的一个小步骤。

1. Concept check 2: How can you interpret the dot product $\nabla f(P) \cdot \vec{v}$, where $P$ is some point in space and $\vec{v}$ is some vector?
概念检查 2：你如何解释点积 $\nabla f(P) \cdot \vec{v}$，其中 $P$ 是空间中的某个点，$\vec{v}$ 是某个向量？

1. The directional derivative of $f$ along the vector $\vec{v}$ at the point $P$.
在点 $P$ 处沿向量 $\vec{v}$ 的 $f$ 的方向导数。

1. The rate at which $f$ changes as you move away from $P$ with a velocity given by $v$:
当你以速度 $v$ 离开点 $P$ 时，函数 $f$ 变化的速率。

--- pic\Fundamental theorem of line integrals.pdf_04.png ---

1. Both answers are correct.
两个答案都是正确的。

2. If this seems unfamiliar, consider reviewing the article on directional derivatives.
如果这看起来不熟悉，可以考虑复习一下关于方向导数的文章。

1. Concept check 3: Given these two facts, how can we interpret the dot product $\nabla f(\vec{r}(t)) \cdot \vec{r}'(t)$?
概念检查 3：给定这两个事实，我们如何解释点积 $\nabla f(\vec{r}(t)) \cdot \vec{r}'(t)$？

2. Choose all answers that apply.
选择所有适用的答案。

1. The rate of change of $f$ with respect to $t$.
$f$ 关于 $t$ 的变化率。

1. The directional derivative of $f$ in the direction of $\vec{r}(t)$.
在 $\vec{r}(t)$ 的方向上的 $f$ 的方向导数。

1. From the previous two questions, this is the directional derivative of $f$ in the direction of $r'(t)$.
从前两个问题来看，这是函数 $f$ 在 $r'(t)$ 方向上的方向导数。

1. This can also be interpreted as the rate of change of $f$ with respect to $t$ (given as a function of $t$).
这也可以解释为 $f$ 关于 $t$ 的变化率（作为 $t$ 的函数给出）。

1. I personally like to think about this as a three-step process.
我个人喜欢把这看作是一个三步过程。

1. The parameter $t$ is changed by some tiny amount $dt$.
参数 $t$ 改变了一些微小的量 $dt$。

1. This causes a tiny step along the path, given by the vector $\vec{r'}(t)\,dt$.
这导致路径上的一个微小步骤，由向量 $\vec{r'}(t)\,dt$ 给出。

1. This, in turn, causes a change in the value of $f$, which is given by the directional derivative $\nabla f(\vec{r}(t)) \cdot \vec{r'}(t)\,dt$.
这反过来导致 $f$ 的值的变化，由方向导数 $\nabla f(\vec{r}(t)) \cdot \vec{r'}(t)\,dt$ 给出。

1.  You can also think about this in terms of the multivariable chain rule:
你也可以用多变量链式法则来考虑这个问题：

1.  In fact, the three steps above just spell out the intuition for the multivariable chain rule.
事实上，上述三步只是阐述了多变量链式法则的直觉。

1. Concept check 4: Finally, how can you interpret the integral $\int_{a}^{b} \nabla f(r(t)) \cdot r'(t) dt$?
概念检查4：最后，你如何解释积分 $\int_{a}^{b} \nabla f(r(t)) \cdot r'(t) dt$？

--- pic\Fundamental theorem of line integrals.pdf_05.png ---

1. The change in $f$ from the start of the path to its end.
路径起点到终点的$f$的变化。

1. The integral gives the change in $f$ from the start of the path to its end.
   积分给出了从路径开始到结束的 $f$ 的变化。

2. You can think of it as adding up all the tiny changes in $f$ due to tiny changes in the parameter $t$ which move us along the path.
   你可以把它看作是由于参数 $t$ 的微小变化而沿着路径移动的所有 $f$ 的微小变化的总和。

3. The end result is the total change in $f$ from start to finish.
   最终的结果是从开始到结束的 $f$ 的总变化。

4. The "area under a curtain" interpretation of a line integral only applies to line integrals through scalar fields.
    "窗帘下的区域"对线积分的解释只适用于通过标量场的线积分。

5. For instance, that would be the interpretation of $\int_{C} f \, |ds| = \int_{a}^{b} f(r(t)) \, \left\| r'(t) \right\| \, dt$
    例如，那将是 $\int_{C} f \, |ds| = \int_{a}^{b} f(r(t)) \, \left\| r'(t) \right\| \, dt$ 的解释。

6. The integrand here is a scalar-valued function multiplied by the length of $ds$, not a vector-valued function dotted with $ds$.
    这里的被积函数是一个标量值函数乘以 $ds$ 的长度，而不是一个与 $ds$ 点积的向量值函数。

7. However, there is a much simpler way to think about the change in the value of $f$ from the start of the path to its end: Just evaluate $f$ at both ends, and subtract the difference: $f(\mathbf{r}(b)) - f(\mathbf{r}(a))$
    然而，考虑从路径开始到结束的 $f$ 的值的变化有一个更简单的方法：只需在两端评估 $f$，并减去差异：$f(\mathbf{r}(b)) - f(\mathbf{r}(a))$

8.  In other words, each side of the equation in the gradient theorem computes the change in $f$ across the path, but the left side thinks of it step-by-step, while the right side takes a global perspective.   
    换句话说，梯度定理中的每一边都计算了 $f$ 在路径上的变化，但是左边是一步步地思考，而右边则采取了全局的视角。

我理解了你的要求，以下是格式调整后的文本：

--- pic\Fundamental theorem of line integrals.pdf_06.png ---

1. A quick proof
快速证明

2. Using the multivariable chain rule, we have
使用多变量链式法则，我们得到
   

1. Plugging this into the statement of the gradient theorem, we see it becomes the same as the fundamental theorem of calculus.
将此代入梯度定理的陈述中，我们看到它变为与微积分的基本定理相同。

1. Tada! This proof leverages the powerful fundamental theorem of calculus, along with the multivariable chain rule, and hence looks deceptively simple. 
啪达！这个证明利用了强大的微积分基本定理，再加上多变量链式法则，因此看起来简单得令人误解。

1. A good exercise in understanding this theorem is to think through how exactly this quick and tidy three-line proof encapsulates the intuition for the gradient theorem spelled out in the last section. 
理解这个定理的一个好方法是深思熟虑这个快速而整洁的三行证明如何精确地包含了在上一节中阐述的梯度定理的直觉。  

1. There's nothing wrong with using other powerful theorems to help prove new results. 
使用其他强大的定理来帮助证明新的结果没有什么错。

1. In fact, to avoid doing so would be foolish. 
事实上，避免这样做是愚蠢的。

1. However, walking through such proofs Is often not enough for a deeper understanding, so it's healthy to unravel new results into their full meaning, seeing how they stand up on their own.
然而，仅仅通过这样的证明往往无法深入理解，所以将新的结果解构为他们的完整含义是有益的，看看他们如何独立存在。

1. Example: A sinusoidal path.
示例：正弦路径。

1. Define f as $f(x, y) = x^2 + y^2$
定义函数 $f$ 为 $f(x, y) = x^2 + y^2$

--- pic\Fundamental theorem of line integrals.pdf_07.png ---

1. Let $C$ represent the path parameterized by $r(t)$ between the values $t = 0$ and $t = 2\pi$.
让$C$代表由$r(t)$参数化的路径，$t$的值在$0$和$2\pi$之间。

1. Compute the integral 
计算积分

1.  Solution 1: The old fashioned way.
解决方案1：老式的方式。

1. We can spell out the full line integral and compute it.
我们可以写出完整的线积分并计算它。

1. In preparation, we will need to evaluate the gradient of $f(x, y) = x^2 + y^2$.
在准备过程中，我们需要评估$f(x, y) = x^2 + y^2$的梯度。

1. What is $\nabla f$?
$\nabla f$是什么？

1.  We will also need the derivative of $r(t)$.
我们还需要$r(t)$的导数。

1.  What is $r'(t)$?
$r'(t)$是什么？


--- pic\Fundamental theorem of line integrals.pdf_08.png ---

1. Finally, what do you get when you plug these in and chug through the line integral?
最后，当你插入这些并通过线积分时，你会得到什么？

1. Solution 2: Apply the fundamental theorem of line integrals.
解决方案2：应用线积分的基本定理。

1. Applying the fundamental theorem of line integrals, we can skip over many of the steps from the previous solution, including the computation of the gradient of $f$ and the derivative of $r(t)$. 
   应用线积分的基本定理，我们可以跳过前一个解决方案的许多步骤，包括计算$f$的梯度和$r(t)$的导数。
   
--- pic\Fundamental theorem of line integrals.pdf_09.png ---

1. Solve the line integral above using the gradient theorem.
使用梯度定理解决上面的线积分。

1. If you look back through the full computation of the line integral in solution 1, the computations we performed actually feel pretty silly.
   如果你回头看看解决方案1中线积分的完全计算，我们实际上执行的计算感觉相当愚蠢。

2. We took the derivative of everything, including the partial derivatives of $x^2 + y^2$ and the ordinary derivatives of $t$ and $\sin(t)$, then later integrated those derivatives back up to where they started.
我们对所有东西都取了导数，包括 $x^2 + y^2$ 的偏导数以及 $t$ 和 $\sin(t)$ 的普通导数，然后后来将这些导数积分回到它们开始的地方。

1. Working through this should also help build an intuition for how the fundamental theorem of line integrals derives from the fundamental theorem of calculus. 
通过这个，也应该有助于建立一个直觉，了解线积分的基本定理如何源于微积分的基本定理。

1. Path independence
路径独立性

1. The gradient theorem has a really important consequence regarding gradient fields.
梯度定理对于梯度场有一个非常重要的影响。

1. Suppose you have two distinct curves $C_1$ and $C_2$, each connecting the same two points $A$ and $B$.
   假设你有两条不同的曲线$C_1$和$C_2$，它们分别连接着相同的两点$A$和$B$。

2. Let's say these are wandering through the gradient field of some scalar-valued function $f$:
   假设这些曲线都穿越了某个标量函数$f$的梯度场：

3. According to the gradient theorem, the line integral of $\nabla f$ along each of these curves will be the same since that integral is completely determined by the value of $f$ at $A$ and $B$:
   根据梯度定理，沿着这些曲线的$\nabla f$的线积分将是相同的，因为该积分完全由$f$在$A$和$B$处的值决定：

4. We explore this idea further in the next article on conservative vector fields.
   我们将在关于保守矢量场的下一篇文章中进一步探讨这个概念。

--- pic\Fundamental theorem of line integrals.pdf_10.png ---

1. The fundamental theorem of line integrals, also called the gradient theorem, states that
线积分的基本定理，也被称为梯度定理，其表述为

1. The intuition behind this formula is that each side represents the change in the value of a multivariable function $f$ as you walk along a path parameterized by $r(t)$.
   这个公式背后的直观理解是，每一侧都代表了当你沿着由$r(t)$参数化的路径行走时，多变量函数$f$的值的变化。

2. This formula implies that gradient fields are path independent, meaning the line integrals along any two paths connecting the same start and end points will be equal.
   这个公式表明梯度场是路径无关的，意味着任何两条连接同一起点和终点的路径的线积分都将相等。