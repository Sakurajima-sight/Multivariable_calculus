
--- pic\Quadratic approximation.pdf_00.png ---

1. Quadratic approximation
二次近似

1. Quadratic approximations extend the notion of a local linearization, giving an even closer approximation of a function.
二次近似扩展了局部线性化的概念，给出了一个函数更精确的近似。

1. Background:
背景：

2. Local linearization
局部线性化

3. Graphs
图表

4. Second partial derivatives
二阶偏导数

1. The goal, as with a local linearization, is to approximate a potentially complicated multivariable function $f$ near some input, which I'll write as the vector $x_0$.
与局部线性化一样，目标是在某个输入附近近似一个可能复杂的多变量函数f，我将其写为向量$x_0$。

1. A quadratic approximation does this more tightly than a local linearization, using the information given by second partial derivatives.
二次近似比局部线性化更紧密地做到了这一点，它使用了由二阶偏导数给出的信息。

5. Non-vector form
非向量形式

1. In the specific case where the input of $f$ is two dimensional, and you are approximating near a point $(x_0, y_0)$, you will see below that the quadratic approximation ends up looking like this:
在f的输入是二维的特定情况下，并且你正在$(x_0, y_0)$附近进行近似，你将在下面看到二次近似最终看起来像这样：

1. $Q(x, y) = f(x_0, y_0) + f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0) + \frac{1}{2}f_{xx}(x_0, y_0)(x - x_0)^2 + f_{xy}(x_0, y_0)(x - x_0)(y - y_0) + \frac{1}{2}f_{yy}(x_0, y_0)(y - y_0)^2$

6. Vector form
向量形式

7. The general form of this, for a scalar-valued function $f$ with any kind of multidimensional input, here's what that approximation looks like:
对于具有任何类型多维输入的标量值函数f，这种近似的一般形式如下：

--- pic\Quadratic approximation.pdf_01.png ---

7. $Q(x) = f(x) + \nabla f(x_0) \cdot (x - x_0) + \frac{1}{2}(x - x_0)^TH_f(x_0)(x - x_0)$
$Q(x) = f(x) + \nabla f(x_0) \cdot (x - x_0) + \frac{1}{2}(x - x_0)^TH_f(x_0)(x - x_0)$

1. I know it looks a bit complicated, but I'll step through it piece by piece later on.
我知道这看起来有点复杂，但我会在后面一步一步地解释。

8. Here's a brief outline of each term.  
以下是每个术语的简要概述。

1. $f$ is a function with multi-dimensional input and a scalar output.
f是一个具有多维输入和标量输出的函数。

1. $\nabla f(x_0)$ is the gradient of $f$ evaluated at $x_0$.
$\nabla f(x_0)$是在$x_0$处评估的f的梯度。

2. $H_f(x_0)$ is the Hessian matrix of $f$ evaluated at $x_0$.
$H_f(x_0)$是在$x_0$处评估的f的海森矩阵。

3. The vector $x_0$ is a specific input, the one we are approximating near.
向量$x_0$是一个特定的输入，我们正在近似的那个。

4. The vector $x$ represents the variable input.
向量x表示变量输入。

3. The vector $x_0$ is a specific input, the one we are approximating near. The vector $x$ represents the variable input.
向量$x_0$是一个特定的输入，是我们近似的那个。向量x表示可变输入。

1.  The approximation function, $Q$, has the same value as $f$ at the point $x_0$, all its partial derivatives have the same value as those of $f$ at this point, and all its second partial derivatives have the same value as those of $f$ at this point.
近似函数$Q$在点$x_0$处的值与f相同，所有的偏导数在这个点上的值与f在这个点上的值相同，所有的二阶偏导数在这个点上的值与f在这个点上的值相同。

5. Tighter and tighter approximations
越来越紧的近似

6. Imagine you are given some function $f ( $x$ , y )$ with two inputs and one output, such as
想象一下，你得到了一个函数$f ( $x$ , y )$，它有两个输入和一个输出，例如

--- pic\Quadratic approximation.pdf_02.png ---

1. The goal is to find a simpler function that approximates $f(x, y)$ near some particular point $(x_0, y_0)$.
目标是找到一个在某个特定点$(x_0, y_0)$附近近似$f(x, y)$的简化函数。

1. For example,
例如，

1. Zero-order approximation
零阶近似

12. The most naive approximation would be a constant function which equals the value of $f$ at $(x_0, y_0)$ everywhere. 
最简单的近似会是一个常数函数，它在任何地方的值都等于$f$在$(x_0, y_0)$的值。

1. We call this a "0-order approximation".
   我们称之为“0阶近似”。

2. In the example:
在例子中：

3. Written in the abstract:
抽象地写出来：

2. Constant function
常数函数

4. Graphically:
图形化：

2.  The graph of this approximation function $C(x, y)$ is a flat plane passing through the graph of our function at the point $(x_0, y_0, f(x_0, y_0))$.
这个近似函数$C(x, y)$的图像是一个平面，它通过我们的函数在点$(x_0, y_0, f(x_0, y_0))$处的图像。

5. Below is a video showing how this approximation changes as we move the point $( x_0 , y_0 )$ around.
下面是一个视频，展示了当我们移动点 $( x_0 , y_0 )$ 时，这个近似如何变化。

--- pic\Quadratic approximation.pdf_03.png ---

1. The graph of $f$ is pictured in blue, the graph of the approximation Is white, and the point $(x_0, y_0, f(x_0, y_0))$ is pictured as a red dot.
$f$的图像用蓝色表示，近似的图像用白色表示，点$(x_0, y_0, f(x_0, y_0))$用红点表示。

1. First-order approximation
一阶近似

1. The constant function zero-order approximation Is pretty lousy.  
常数函数的零阶近似是相当糟糕的。

1. Sure, it is guaranteed to equal $f(x, y)$ at the point $(x_0, y_0)$, but that's about it.
当然，它保证在点$(x_0, y_0)$处等于$f(x, y)$，但仅此而已。

2. One step better is to use a local linearization, also known as a "First-order approximation".
更好的一步是使用局部线性化，也被称为"一阶近似”。

2. In the example:
在例子中：

3. Written in the abstract:
抽象地写出来：

3. $L(x,y) = f(x_0, y_0) + f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)$
$L(x,y) = f(x_0, y_0) + f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)$

4. Here, $f_x$ and $f_y$ denote the partial derivatives of f.
这里，$f_x$ 和 $f_y$ 表示 $f$ 的偏导数。

5. Graphically
图形化：

1.  The graph of a local linearization Is the plane tangent to the graph of $f$ at the point $(x_0, y_0, f(x_0, y_0))$.
局部线性化的图像是平面，在点$(x_0, y_0, f(x_0, y_0))$处切到$f$的图像。

6. Here is a video showing how this approximation changes as we move around the point $( x_0 , y_0 )$ :
这是一个视频，展示了当我们围绕点 $( x_0 , y_0 )$ 移动时，这个近似如何变化。

--- pic\Quadratic approximation.pdf_04.png ---

1. Second-order approximation.
二阶近似。

1.  Better still is a quadratic approximation, also called a "second-order approximation". 
更好的是二次近似，也称为"二阶近似"。

1. The remainder of this article is devoted to finding and understanding the analytic form of such an approximation, but before diving in, let's see what such approximations look like graphically.
本文的其余部分致力于寻找和理解这种近似的分析形式，但在深入研究之前，让我们看看这种近似在图形上是什么样的。

1.  You can think of these approximations as nestling into the curves the graph at the point $(x_0, y_0, f(x_0, y_0))$, giving it a sort of mathematical hug.
你可以把这些近似看作是在点$(x_0, y_0, f(x_0, y_0))$的曲线图中安置，给它一种数学的拥抱。

1. "Quadratic" means product of two variables
"二次"意味着两个变量的乘积。

--- pic\Quadratic approximation.pdf_05.png ---
1. In single variable functions, the word "quadratic" refers to any situation where a variable is squared as in the term x².
在单变量函数中，“二次”这个词指的是任何变量被平方的情况，就像在x²这个项中一样。

1. With multiple variables, "quadratic" refers not only to square terms, like $x^2$ and $y^2$ , but also terms that involve the product of two separate variables, such as $xy$.
对于多个变量，“二次”不仅指平方项，如$x^2$和$y^2$，还指涉及两个单独变量的乘积的项，如$xy$。

1. With multiple variables, "quadratic" refers not only to square terms, like x².
在多变量情况下，“二次”不仅指的是平方项，比如x²。

1. In general, the "order" of a term which is the product of several things, such as 3x²y³, is the total number of variables multiplied into that term.
一般来说，是由几个变量的乘积构成的一个项的“阶”，比如3x²y³，就是该项中乘在一起的变量总数。


2. In this case, the order would be 5 : Two $x$ 's, three y 's, and the constant doesn't matter.
在这种情况下，阶数将为5：两个x，三个y，常数无关紧要。

3. Graphs of quadratic functions
二次函数的图形

1. One way to think of quadratic functions is in terms of their concavity, which might depend on which direction you are moving in.
考虑二次函数的一种方法是从其凹度角度来思考，这可能取决于你移动的方向。

4. If the function has an upward concavity, as is the case, for example, with $f ( $x$ , y ) = x^2 + y^2$ , the graph will look something like this:
如果函数具有向上的凹度，例如，对于$f ( $x$ , y ) = x^2 + y^2$，图形将如下所示：

1. This shape, which is a three-dimensional parabola, goes by the name paraboloid.
这种形状，是一个三维抛物线，被称为抛物面。

5. If the function is concave up in one direction and linear in another, the graph looks like a parabolic curve has been dragged through space to trace out a surface. 
如果函数在一个方向上是凹的，在另一个方向上是线性的，图形看起来像一个抛物线曲线被拖过空间以描绘出一个表面。

1. For example this happens in the case of $f ( $x$ , y ) = x^2 + y$ :
   例如，这在$f ( $x$ , y ) = x^2 + y$的情况下会发生：

--- pic\Quadratic approximation.pdf_06.png ---
1. Finally, if the graph is concave up when traveling in one direction, but concave down when traveling in another direction, as is the case for $f ( $x$ , y ) = x^2 − y^2$, the graph looks a bit like a saddle.
最后，如果图形在一个方向上是凹的，但在另一个方向上是凸的，就像$f ( $x$ , y ) = x^2 − y^2$的情况那样，图形看起来有点像马鞍。

2. Here's what such a graph looks like:
这就是这样一个图形的样子：

3. Reminder on the local linearization recipe.
关于局部线性化方法的提醒。

4. To actually write down a quadratic approximation of a function $f$ near the point $( x_0 , y_0 )$, we build up from the local linearization.
要实际写下函数f在点$( x_0 , y_0 )$附近的二次近似，我们从局部线性化开始构建。

--- pic\Quadratic approximation.pdf_07.png ---
1. It's worth walking through the recipe for finding the local linearization one more time since the recipe for finding a quadratic approximation is very similar.
再次走过寻找局部线性化的步骤是值得的，因为寻找二次逼近的步骤与此非常类似。

1. Start with the constant term $f ( x_0 , y_0 )$, so that our approximation at least matches $f$ at the point $( x_0, y_0 )$.
从常数项$f ( x_0 , y_0 )$开始，这样我们的近似至少在点$( x_0, y_0 )$处与$f$匹配。

2. Add on linear terms $f_x ( x_0 , y_0 ) ( $x$ − x_0 )$ and $f_y ( x_0 , y_0 ) ( y − y_0 )$.
添加线性项$f_x ( x_0 , y_0 ) ( $x$ − x_0 )$和$f_y ( x_0 , y_0 ) ( y − y_0 )$。

3. Use the constants $f_x ( x_0 , y_0 )$ and $f_y ( x_0 , y_0 )$ to ensure that our approximation has the same partial derivatives as $f$ at the point $( x_0 , y_0 )$.
使用常数$f_x ( x_0 , y_0 )$和$f_y ( x_0 , y_0 )$来确保我们的近似在点$( x_0 , y_0 )$处具有与$f$相同的偏导数。

4. Use the terms $( $x$ − x_0 )$ and $( y − y_0 )$ instead of simply $x$ and $y$ so that we don't mess up the fact that our approximation equals $f ( x_0 , y_0 )$ at the point $( x_0, y_0 )$.
使用项$( $x$ − x_0 )$和$( y − y_0 )$，而不仅仅是$x$和$y$，以确保我们不会混淆我们的近似在点$( x_0, y_0 )$处等于$f ( x_0 , y_0 )$的事实。

1. Finding the quadratic approximation
寻找二次近似

1. For the quadratic approximation, we add on the quadratic terms $(x - x_0)^2$, $(x - x_0)(y - y_0)$, and $(y - y_0)^2$, and for now we write their coefficients as the constants $a$, $b$, and $c$ which we will solve for in a moment.
对于二次近似，我们加上二次项 $(x - x_0)^2$，$(x - x₀)(y - y₀)$，和 $(y - y₀)^2$，现在我们将其系数写为常数$a$，$b$ 和 $c$，稍后我们将解出它们。

2. In the same way that we made sure that the local linearization has the same partial derivatives as $f$ at $(x_0, y_0)$, we want the quadratic approximation to have the same second partial derivatives as $f$ at this point.
就像我们确保局部线性化在$(x_0, y_0)$处的偏导数与$f$相同一样，我们希望二次近似在这一点上的二阶偏导数与$f$相同。

3. The really nice thing about the way I wrote $Q_f$ above is that the second partial $\frac{\partial^2 Q_f}{\partial x^2}$ derivative depends only on the $a(x - x_0)^2$ term.
我在上面写$Q_f$的方式真好，因为二阶偏导数$\frac{\partial^2 Q_f}{\partial x^2}$只依赖于$a(x - x_0)^2$项。

--- pic\Quadratic approximation.pdf_08.png ---
1. Try it! Take the second partial derivative with respect to $x$ of every term in the expression of $Q_f(x, y)$ above, and notice that they all go to zero except for the $a(x - x_0)^2$.
试一试！对上面$Q_f(x, y)$表达式中的每一项都求关于$x$的二阶偏导数，你会发现除了$a(x - x_0)^2$，它们都变为零。

1. Did you really try it? I'm serious, take a moment to reason through it. It really helps in understanding why $Q_f$ is expressed the way it is.
你真的试过了吗？我是认真的，花一点时间来理解一下。这对理解为什么$Q_f$以这种方式表示非常有帮助。

1. This fact is nice because rather than taking the second partial derivative of the entire monstrous expression, you can view it like this.
这个事实很好，因为你可以这样看待，而不是对整个巨大的表达式求二阶偏导数。

1. Since the goal is for this to match $f_{xx}$, test yourself: Use similar reasoning to figure out what the constants $b$ and $c$ should be.
既然目标是让这个与$f_{xx}$匹配，那就自己试试看：使用类似的推理来找出常数$b$ 和 $c$应该是什么。

1. Test yourself: Use similar reasoning to figure out what the constants $b$ and $c$ should be.
自我测试：使用类似的推理来确定常数$b$ 和 $c$应该是什么。

1. The mixed partial derivative $\frac{\partial^2 Q}{\partial $x$ \partial y}$ depends only on the $b(x - x_0)(y - y_0)$term ( try it! ), so we have
混合偏导数$\frac{\partial^2 Q}{\partial $x$ \partial y}$只依赖于$b(x - x_0)(y - y_0)$项（试试看！），所以我们有

2. Since we want this mixed partial derivative of our approximation to equal the mixed partial derivative of $f$ at this point, $f_{xy}(x_0, y_0)$, we say
由于我们希望我们的近似的混合偏导数在这一点上等于f的混合偏导数，即$f_{xy}(x_0, y_0)$，我们说

--- pic\Quadratic approximation.pdf_09.png ---
1. Nearly identical reasoning will lead us to the conclusion
几乎相同的推理会让我们得出结论

2. We can now write our final quadratic approximation, with all six of its terms working in harmony to mimic the behavior of $f$ at $(x_0, y_0)$.
我们现在可以写出我们的最终二次逼近，它的所有六个项都在和谐地工作，以模仿在点$(x_0, y_0)$处$f$的行为。

3. Example: Approximating $\sin(x) \cos(y)$.
示例：逼近$\sin(x) \cos(y)$。

4. To see this beast in action, let's try it out on the function from the introduction.
要看这个公式如何应用，让我们在导言中的函数上试一试。

1.  Problem: Find the quadratic approximation of $f(x, y) = \sin(x) \cos(y)$ about the point $(x, y) = \left(\frac{\pi}{4}, \frac{\pi}{4}\right)$.
   问题：找到函数$f(x, y) = \sin(x) \cos(y)$在点$(x, y) = \left(\frac{\pi}{4}, \frac{\pi}{4}\right)$处的二次近似。

2. To collect all the necessary information, you need to evaluate $f(x, y) = \sin(x) \cos(y)$ and all of its partial derivatives and all of its second partial derivatives at the point $(x, y) = \left(\frac{\pi}{4}, \frac{\pi}{4}\right)$.
要收集所有必要的信息，你需要在点$(x, y) = \left(\frac{\pi}{4}, \frac{\pi}{4}\right)$处求出$f(x, y) = \sin(x) \cos(y)$及其所有的偏导数和所有的二阶偏导数。

--- pic\Quadratic approximation.pdf_10.png ---

--- pic\Quadratic approximation.pdf_11.png ---

--- pic\Quadratic approximation.pdf_12.png ---

--- pic\Quadratic approximation.pdf_13.png ---

1. Almost there! As a final step, apply all these values to the formula for a quadratic approximation.
   几乎到了！作为最后一步，将所有这些值应用到二次近似的公式中。


2. So for example, to generate the animation of quadratic approximations, this is the formula I had to plug into the graphing software.
   例如，为了生成二次近似的动画，我必须将这个公式输入到绘图软件中。

1. Vector notation using the Hessian
使用海森矩阵的向量表示法

1. Perhaps it goes without saying that the expression for the quadratic approximation is long.
可能不用说，二次近似的表达式很长。

--- pic\Quadratic approximation.pdf_14.png ---

1. Now imagine if $f$ had three inputs, $x$, $y$, and $z$.
   这是很长的。现在想象一下，如果函数 $f$ 有三个输入，$x$、$y$ 和 $z$。

1. In principle you can imagine how this might go, adding terms involving $f_z$, $f_{xz}$, $f_{zz}$, on and on with all 3 partial derivatives and all 9 second partial derivative. 
原则上，你可以想象这可能会如何进行，添加涉及$f_z$，$f_{xz}$，$f_{zz}$等的项，继续添加所有3个偏导数和所有9个二阶偏导数的项。

1. But this would be a total nightmare!
但这将是一场噩梦！

2. When something is not that complicated in principle, it shouldn't be that complicated in notation.
原则上，当某件事并不那么复杂时，它的符号表示也不应该那么复杂。

1. Now imagine you were writing a program to find the quadratic approximation of a function with 100 inputs.
现在想象一下，你正在编写一个程序来找到具有100个输入的函数的二次近似。

1. Madness! 
疯狂！

3. It actually doesn't have to be that bad.
   实际上，它不必那么糟糕。

4. When something is not that complicated in principle, it shouldn't be that complicated in notation.
   当原则上的事情并不那么复杂时，它在符号表示上也不应该那么复杂。

5. Quadratic approximations are a little complicated, sure, but they're not absurd.
   二次近似确实有点复杂，但并非荒谬。

6. Using vectors and matrices, specifically the gradient and Hessian of f, we can write the quadratic approximation $Q_f$ as follows:
   使用向量和矩阵，特别是函数 $f$ 的梯度和海森矩阵，我们可以按照以下方式写出二次近似$Q_f$：

7. Let's break this down:
   让我们来分解这个公式：

8.  The boldfaced $x$ represents the input variable(s) as a vector,
    加粗的 $x$ 代表作为向量的输入变量，

1. Moreover, $x_0$ is a particular vector in the input space.
此外，$x_0$ 是输入空间中的一个特定向量。

9.   If this has two components, this formula for $Q_f$ ; is just a different way to write the one we derived before, but it could also represent a vector with any other dimension.
    如果它有两个分量，那么 $Q_f$ 的公式只是写出我们之前导出的公式的另一种方式，但它也可以表示任何其他维度的向量。

4. The dot product $\nabla f ( x_0 ) \cdot ( x - x_0 )$ will expand into the sum of all terms of the form $f_x ( x_0 ) ( x - x_0 )$, $f_y ( x_0 ) ( y - y_0 )$, etc.
点积$\nabla f ( x_0 ) \cdot ( x - x_0 )$将展开为所有形如$f_x ( x_0 ) ( x - x_0 )$，$f_y ( x_0 ) ( y - y_0 )$等的项的和。

5. if this is not familiar from the vector notation for local linearization, work it out for yourself in the case of 2 -dimensions to see!
如果你对于局部线性化的向量表示法不熟悉，可以自己在二维情况下推导一下看看！

--- pic\Quadratic approximation.pdf_15.png ---

1. The little superscript $T$ in the expression $(x - x_0)^T$ indicates "transpose".
表达式 $(x - x_0)^T$ 中的小写上标 $T$ 表示 "转置"。

2. This means you take the initial vector $(x - x_0)$ , which looks something like this:
这意味着你取初始向量 $(x - x_0)$，它看起来像这样：

3. Then you flip it, to get something like this:
然后你翻转它，得到像这样的东西：

4. H f( x0 ) is the Hessian of $f$ .
$H_f(x_0)$ 是 $f$ 的海森矩阵。

5. The expression $(x - x_0)^T H_f(x_0) (x - x_0)$ might seem complicated if you have never come across something like it before.
如果你以前从未遇到过类似的东西，那么表达式 $(x - x_0)^T H_f(x_0) (x - x_0)$ 可能看起来很复杂。

6. This way of expressing quadratic terms is actually quite common in vector-calculus and vector-algebra, so it's worth expanding an expression like this at least a few times in your life.
这种表示二次项的方式在向量微积分和向量代数中实际上很常见，所以在你的生活中至少扩展几次这样的表达式是值得的。

7. For example, try working it out in the case where$x$is two-dimensional to see what it looks like.
例如，尝试在$x$是二维的情况下计算它，看看它是什么样子。

--- pic\Quadratic approximation.pdf_16.png ---

1. You should find that it is exactly 2 times the quadratic portion of the non-vectorized formula we derived above.
   你应该发现它正好是我们在上面导出的非向量化公式的二次部分的两倍。

2. What's the point? In truth, it is a real pain to compute a quadratic approximation by hand, and it requires staying very organized to do so without making a little mistake.
   有什么意义呢？事实上，手动计算二次近似是一件真正痛苦的事情，而且在不犯小错误的情况下保持有序是需要的。

3. In practice, people rarely work through a quadratic approximation like the example above, but knowing how they work is useful for at least two broad reasons:
   实际上，人们很少像上面的例子那样进行二次近似，但是知道它们是如何工作的对于至少两个广泛的原因是有用的：

4. Computation: Even if you never have to write out a quadratic approximation, you may one day need to program a computer to do it for a particular function. 
   计算：即使你永远不必写出二次近似，你可能有一天需要为一个特定的函数编程计算机来做这个。或者即使你依赖别人的程序，

1. Or even if you are relying on someone else's program, you may need to analyze how and why the approximation is failing in some circumstance.
你也可能需要分析在某些情况下近似是如何以及为什么失败的。

5. Theory: Being able to reference a second-order approximation helps us to reason about the behavior of general functions near a point.
   理论：能够引用二阶近似有助于我们理解一般函数在某点附近的行为。

1. This will be useful later in figuring out if a point is a local maximum or minimum.
这将在后面确定一个点是否为局部最大或最小值时有所帮助。