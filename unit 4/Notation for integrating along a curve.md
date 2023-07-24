
--- pic\Notation for integrating along a curve.pdf_00.png ---

1. Notation for integrating along a curve
沿曲线积分的表示法

1. There is a very compact way to express arc length integrals, which lays a foundation for writing line integrals.
有一种非常紧凑的方式来表示弧长积分，这为写线积分奠定了基础。

1. Background:
背景：

2. Arc length of parametric curves
参数曲线的弧长

3. Derivatives of vector valued function
向量值函数的导数

4. What we're building to
我们正在构建的是什么

1. The arc length integral
$\int \sqrt{(dx)^2 + (dy)^2}$
may alternatively be written as
$\int_C ds$
where $C$ represents the curve, and $ds$ is shorthand for $\sqrt{(dx)^2 + (dy)^2}$, representing the length of a tiny step along the curve.
弧长积分
$\int \sqrt{(dx)^2 + (dy)^2}$
可以写为
$\int_C ds$
其中 $C$ 代表曲线，$ds$ 是 $\sqrt{(dx)^2 + (dy)^2}$ 的简写，表示沿曲线的微小步长。

1. When the parametric curve is given by a vector-valued function $r(t)$ in the range $a \leq t \leq b$, the arc length integral looks like:
当参数曲线由向量值函数 $r(t)$ 给出，并且满足范围 $a \leq t \leq b$ 时，弧长积分看起来像：

--- pic\Notation for integrating along a curve.pdf_01.png ---

1. In other words, the small step $ds$ along the curve is the magnitude of the derivative of $r(t)$.
换句话说，沿曲线的小步长 $ds$ 是 $r(t)$ 的导数的大小。

2. This is the standard notation for line integrals, introduced in the next article.
这是线积分的标准表示法，将在下一篇文章中介绍。

1. Writing arc length compactly
紧凑地写出弧长

3. When we talked about finding the arc length of function graphs and the arc length of parametric curves, we started by setting up an integral of the form $\int \sqrt{(dx)^2 + (dy)^2}$.
当我们谈到寻找函数图的弧长和参数曲线的弧长时，我们开始是设立一个形如 $\int \sqrt{(dx)^2 + (dy)^2}$ 的积分。

1. Instead of always writing $\sqrt{(dx)^2 + (dy)^2}$ to represent a tiny change in arc length, a common convention is to express this tiny change as $ds$. 
   为了表示微小的弧长变化，我们通常不总是写成 $\sqrt{(dx)^2 + (dy)^2}$，一个常见的约定是将这个微小的变化表示为 $ds$。

4. You think of $ds$ as a tiny step along whatever curve we're talking about, in the same way that $dx$ is a tiny step in the $x$-direction or $dy$ is a tiny step in the $y$-direction.
你可以把 $ds$ 想象成我们正在讨论的任何曲线上的一个微小步骤，就像 $dx$ 是 $x$ 方向上的一个微小步骤，或者 $dy$ 是 $y$ 方向上的一个微小步骤。

2. Settling bound awkwardness
   解决边界尴尬问题

整理后的文本如下：

--- pic\Notation for integrating along a curve.pdf_02.png ---

1. Throughout the last few articles, we procrastinated putting bounds on the integral $\int \sqrt{(dx)^2 + (dy)^2}$.
在过去的几篇文章中，我们一直在推迟对积分$\int \sqrt{(dx)^2 + (dy)^2}$设置边界。

1. Which we now know could be written simply as $\int ds$.
我们现在知道，这可以简单地写成 $\int ds$。

2. If everything inside the integral was written in terms of $x$, the bounds will reflect $x$ values.
如果积分内的所有内容都以 $x$ 表示，那么边界将反映 $x$ 的值。

9. If it is all in terms of $t$, the bounds reflect $t$ values, etc.
如果全部是关于$t$的，边界就反映$t$的值等等。

3. If you are uncomfortable with your integral looking so naked but you don't want to make a commitment about which variable owns the bounds, here's what you do.
如果你对你的积分看起来如此赤裸感到不舒服，但你又不想确定哪个变量拥有边界，你可以这么做。

4. You say, "Let $C$ be the curve defined by . . ." and you go on defining your curve.
你说，“让 $C$ 是由...定义的曲线”，然后你继续定义你的曲线。

1.  Then you just write your integral with a little $C$ at the bottom:
"然后你只需在积分下面写一个小的$C$：

1.  This basically tells the person reading it to go find where the curve $C$ is defined, then plug in the relevant boundary values when it comes time to compute.
这基本上告诉读者去找到曲线$C$在哪里定义，然后在计算时插入相关的边界值。

1.  On the one hand, this notation is so simple as to be nearly meaningless.
一方面，这种表示法太简单，几乎没有意义。

1.  You might read it out loud by saying "The arc length of $C$ is the integral over $C$ of tiny steps along $C$".
你可能会大声读出来，说“$C$的弧长是沿着$C$的微小步骤对$C$的积分”。

1. Silly, right?
傻了吧，对吧？

1.  This entirely sweeps under the rug the details of what solving the arc-length problem entails, expanding $ds$ and encoding the definition of $C$ into the integral.
这完全忽视了解决弧长问题所涉及的细节，扩展$ds$并将$C$的定义编码到积分中。

1.  But, that's actually the point. 
但是，那实际上就是问题所在。

1. Part of the reason for talking about arc length integrals is to set the stage for the broader idea of line integrals.
讨论弧长积分的部分原因是为了为更广泛的线积分概念做铺垫。

1.  When we get to line integrals, you don't always want the full details of the curve and the tiny change in arc length $ds$ to spill out into your notation.
当我们谈到线积分时，你并不总是希望曲线的全部细节和弧长$ds$的微小变化都显露在你的符号中。

1.  There will be other things to deal with.
将会有其他事情要处理。

1.  In that context, abstracting the arc length away to something as simple as $\int_C ds$ will be a more-than-welcome simplification.
在那种情况下，将弧长抽象为简单的$\int_C ds$会是非常受欢迎的简化。


--- pic\Notation for integrating along a curve.pdf_03.png ---

1. In the language of vector calculus
在向量微积分的语言中

1. In vector calculus, we move away from thinking about a parametric curve as a set of parametric equations like $x(t) = t\cos(t), y(t) = t\sin(t)$.
在向量微积分中，我们不再把参数曲线看作是一组参数方程，比如 $x(t) = t\cos(t), y(t) = t\sin(t)$。

1. Instead, we think of these curves as the output of a single vector-valued function,
相反，我们把这些曲线看作是一个向量值函数的输出，

1. The derivative of a vector-valued function like this gives another vector valued function,
像这样的向量值函数的导数会给出另一个向量值函数，

1. This gives us a very nice way to express $ds$, the length of a tiny step along the curve, $ds = |r'(t)|dt$.
这为我们提供了一个很好的方式来表示沿曲线的一小步长度$ds$，即 $ds = |r'(t)|dt$。

1. Why is this true? One way is to expand out the expression $|r'(t)|dt$ and simplify. Try it! 
为什么是这样？一种方法是展开表达式$|r'(t)|dt$并简化。试试看！

--- pic\Notation for integrating along a curve.pdf_04.png ---

1. Alternatively, think about how we interpret vector-derivatives. 
另外，想想我们如何解释向量导数。

1. Imagine standing on a value $t_0$ in the input space, also known as the parameter space, and getting a slight nudge of size $dt$, bringing you up to the point $t_0 + dt$.
想象一下你站在输入空间，也称为参数空间的一个值$t_0$上，然后得到一个大小为$dt$的微小推动，把你带到了点$t_0 + dt$。

1.  The derivative vector $r'(t)$ is the resulting "nudge" in the output space along the curve. 
导数向量$r'(t)$是沿曲线在输出空间的结果“推动”。

1.  When we multiply that derivative by the tiny amount $dt$ to get $r'(t)dt$, it's helpful to think about this as a tiny step along the curve.
当我们把那个导数乘以微小量$dt$得到$r'(t)dt$时，把它看作沿曲线的一个微小步骤是有帮助的。

1.  Technically it's a tiny step in the tangent direction, which might be slightly off from the curve.
从技术上讲，它是切线方向的一个微小步骤，这可能会稍微偏离曲线。

1.  However, as $dt$ approaches 0, a step in the tangent direction and a step along the curve can be treated as the same thing.
然而，随着$dt$趋近于0，切线方向的步骤和沿曲线的步骤可以被视为同一件事。

1.  The magnitude of this vector is the size of our small step along the curve, $ds$. 
这个向量的大小是我们沿曲线的小步长，$ds$。

1.  This means the arc length integral for a parametric curve defined by a function $r(t)$ between $t = a$ and $t = b$ could look like $\int_{a}^{b} |r'(t)|dt$.
这意味着由函数$r(t)$在$t = a$和$t = b$之间定义的参数曲线的弧长积分可以看起来像$\int_{a}^{b} |r'(t)|dt$。

15. Actually computing this will look no different from when we thought of these curves as a set of equations, since $|r'(t)|dt$ will always expand to look like $\sqrt{(dx)^2 + (dy)^2}$. 
实际上计算这个并不会与我们把这些曲线看作一组方程时有什么不同，因为$|r'(t)|dt$总会扩展成看起来像$\sqrt{(dx)^2 + (dy)^2}$。

1. However, people generally favor this notation.
然而，人们通常喜欢这种表示法。

2. For one thing, it is compact, and for another, it generalizes well to higher dimensions.
一方面，它是紧凑的，另一方面，它很好地推广到更高维度。

3. Onward to line integrals!
继续进行线积分！

--- pic\Notation for integrating along a curve.pdf_05.png ---

16. Armed with this notation, and an understanding of how portrays tiny steps along a curve, you are now ready to learn about line integrals.
装备了这种符号，并理解了如何描绘沿曲线的微小步骤，你现在已经准备好学习线积分了。