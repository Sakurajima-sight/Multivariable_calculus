
--- pic\Arc length of parametric curves.pdf_00.png ---

1. Arc length of parametric curves
参数曲线的弧长

1. How to find the length of a parametric curve?
如何找到参数曲线的长度？

1. This will lead to the idea of a line integral.
这将引出线积分的概念。

1. Background:
背景：

2. Arc length of function graphs
函数图的弧长

3. Parametric curves
参数曲线

4. Derivatives of vector valued function
向量值函数的导数

1. What we're building to
我们正在建设的目标

1. To find the arc length of a curve, set up an integral of the form $\int \sqrt{(dx)^2 + (dy)^2}$.
要找到曲线的弧长，建立一个形式为$\int \sqrt{(dx)^2 + (dy)^2}$的积分。

1. We now care about the case when the curve is defined parametrically, meaning $x$ and $y$ are defined as functions of some new variable $t$. 
我们现在关心的是当曲线以参数的方式定义时的情况，意味着$x$和$y$被定义为新变量$t$的函数。

1. To apply the arc length integral, first take the derivative of both these functions to get $dx$ and $dy$ in terms of $dt$.
要应用弧长积分，首先对这两个函数都取导数，得到以$dt$为单位的$dx$和$dy$。

1. Plug these expressions into the integral and factor the $dt^2$. 
将这些表达式代入积分，并提取出$dt^2$。

5. The length of a parametric curve
参数曲线的长度

1. Consider the parametric curve defined by the following set of equations: 
考虑由以下一组等式定义的参数曲线：

6. If we let $t$ range from $-1.5$ to $1.5$, the resulting curve looks like this:
如果我们让 $t$ 的范围从 $-1.5$ 到 $1.5$，得到的曲线如下：

--- pic\Arc length of parametric curves.pdf_01.png ---

1. Key question: What is the length of this curve?
关键问题：这条曲线的长度是多少？

9. That is, imagine pulling the line straight, as if you were tightening a loose piece of string, then measuring it with a ruler.
也就是说，想象一下把线拉直，就像你在拉紧一条松散的线，然后用尺子测量。

1. What value would you get?
你会得到什么值？

10. In the last article, we saw how to find the arc length of function graphs, not parametric curves.
在上一篇文章中，我们看到了如何找到函数图的弧长，而不是参数曲线。

11. We started by writing down the following integral: $\int \sqrt{dx^2 + dy^2}$.
我们从写下以下积分开始：$\int \sqrt{dx^2 + dy^2}$。

12. Let's quickly recap the meaning behind this integral.
让我们快速回顾一下这个积分背后的含义。

--- pic\Arc length of parametric curves.pdf_02.png ---

1. Imagine approximating the curve with a bunch of tiny straight lines. 
想象一下用一堆微小的直线来近似曲线。

1. The length of each such tiny line is given using the Pythagorean theorem, $\sqrt{(dx)^2 + (dy)^2}$, $dx$ and $dy$ represent the tiny change in $x$ and $y$ values from the start to the end of the line.
每条这样的微小线段的长度是用毕达哥拉斯定理给出的，$\sqrt{(dx)^2 + (dy)^2}$，$dx$ 和 $dy$ 代表从线段的开始到结束，$x$ 和 $y$ 值的微小变化。

1.  This same integral can apply to parametric curves as well as function graphs. 
这个相同的积分既可以应用于参数曲线，也可以应用于函数图。

1.  This time, since $x$ and $y$ are given as functions of $t$, we write $dx$ and $dy$ in terms of $dt$ by taking the derivative of these two functions.
这一次，因为$x$和$y$被给出为$t$的函数，我们通过对这两个函数求导，以$dt$的形式写出$dx$和$dy$。

1.  For example, differentiating the function defining $x$, we get $\frac{dx}{dt}$.
例如，对定义$x$的函数求导，我们得到$\frac{dx}{dt}$。

1. And similarly with $y$:
对于 $y$ 也是类似的：

--- pic\Arc length of parametric curves.pdf_03.png ---

1. You can think of these expressions as answering the question "when you take some value $t$, and increase it slightly by some tiny amount $dt$, how much does it change $x$ and $y$?
你可以将这些表达式视为回答这个问题：“当你取某个值$t$，并稍微增加一些微小量$dt$，$x$和$y$会变化多少？

1. The answer is expressed in terms of $t$ and $dt$.
答案是用$t$和$dt$表示的。

1. Putting these into the integral, we get 
将它们代入积分，我们得到

1. Now everything inside the integral is written in terms of $t$, so the bounds we place on the integral correspond with the starting and ending values of the parameter $t$. 
现在积分内的所有东西都是用$t$表示的，所以我们在积分上设置的边界对应于参数$t$的起始值和终止值。

1. In this case, we are letting $t$ range from $-1.5$ to $1.5$, so we have
在这种情况下，我们让 $t$ 的范围从 $-1.5$ 到 $1.5$，所以我们有

1. This is a very nasty integral to compute. I'm not even sure that an antiderivative exists. 
这是一个非常难计算的积分。我甚至不确定是否存在反导数。

1. However, we've at least reduced the arc length problem down to a state where you can plug it into a computer. 
然而，我们至少已经将弧长问题简化到可以输入计算机的状态。

1. Practice a parametric arc length integral
练习参数化弧长积分

1. Let's look at the parametric curve defined by $x(t) = t^2 - 3t$ $y(t) = 3t^2$.
让我们来看看由$x(t) = t^2 - 3t$ $y(t) = 3t^2$定义的参数曲线。

--- pic\Arc length of parametric curves.pdf_04.png ---

1. Consider the segment of this curve between the points where $t = -2$ and $t = 2$. 
考虑这条曲线在$t = -2$和$t = 2$之间的段。

2. What is the length of this segment?
这段的长度是多少？

11. Since our curve is expressed in terms of $x$ and $y$, our arc length integrals begin life looking like $\int \sqrt{dx^2 + dy^2}$.
因为我们的曲线是用$x$和$y$表示的，所以我们的弧长积分开始时看起来像$\int \sqrt{dx^2 + dy^2}$。

12. To get this integral in terms of $t$, we must write $dx$ and $dy$ each as some expression of $t$.
要将这个积分表示为$t$的函数，我们必须将$dx$和$dy$每个都写成$t$的某个表达式。

13. Step 1: Write $dx$ and $dy$ in terms of $t$.
步骤1：将$dx$和$dy$写成$t$的函数。

14. What is $dx$ in terms of $t$?
$dx$是$t$的函数是什么？

1. Take the derivative of each side of the expression defining $x$
对定义$x$的表达式的每一边取导数

--- pic\Arc length of parametric curves.pdf_05.png ---

1. What Is $dy$ in terms of $t$?
$dy$是$t$的函数是什么？

1.  Take the derivative of each side of the expression defining $y$: 
对定义$y$的表达式的每一边求导：

1.  Step 2: Put these expressions in the integral.
步骤2：将这些表达式代入积分。

1.  What does our integral look like after we plug in these expressions for $dx$ and $dy$? 
当我们将这些表达式代入$dx$和$dy$后，我们的积分看起来是什么样的？

1.  Simplify it down to the point where there is no radical. 
将其简化到没有根号的地方。

1.  $\int \sqrt{(dt)^2 + (3t^2)^2} dt = \int \sqrt{1 + 9t^4} dt$
$\int \sqrt{(dt)^2 + (3t^2)^2} dt = \int \sqrt{1 + 9t^4} dt$

1.  Step 3: Place the appropriate bounds on the integral and solve.
步骤3：在积分上设置适当的边界并求解。

1.  The problem states that the curve runs from $-2$ to $2$. 
问题说明曲线从$-2$运行到$2$。

1. Solve the integral with these bounds.
在这些边界内解决积分。

--- pic\Arc length of parametric curves.pdf_05.png ---

1.  What Is $dy$ in terms of $t$? 
$dy$是$t$的函数是什么？

1. Take the derivative of each side of the expression defining $y$:
对定义$y$的表达式的每一边求导：

1. Step 2: Put these expressions in the integral
步骤2：将这些表达式代入积分

1. What does our integral look like after we plug in these expressions for $dx$ and $dy$? 
当我们将这些表达式代入$dx$和$dy$后，我们的积分看起来是什么样的？

1. Simplify it down to the point where there Is no radical. $\int dt$
将其简化到没有根号的地方。$\int dt$

1. $\int \sqrt{\left(\frac{dt}{dt}\right)^2 + \left(3t^2\right)^2} dt = \int \sqrt{1 + 9t^4} dt$
$\int \sqrt{\left(\frac{dt}{dt}\right)^2 + \left(3t^2\right)^2} dt = \int \sqrt{1 + 9t^4} dt$

1. Step 3: Place the appropriate bounds on the integral and solve
步骤3：在积分上设置适当的边界并求解

1. The problem states that the curve runs from $-2$ to $2$. Solve the integral with these bounds.
问题说明曲线从$-2$运行到$2$。在这些边界内解决积分。

--- pic\Arc length of parametric curves.pdf_06.png ---

1. So evidently the length of this curve is $28$. 
所以显然这条曲线的长度是$28$。

2. Looking at the picture, this seems about right. 
看图，这似乎是正确的。

3. The curve starts from about $y = 12$, goes down to the $x$-axis and back, which takes at least $24$ units of length. 
曲线从大约$y = 12$开始，下降到$x$轴并返回，至少需要$24$个长度单位。

4. Since it has some curvature, wandering left and right as it goes down and up, the true length is a bit more than $24$. 
由于它有一些曲率，当它上下移动时会左右摇摆，真实的长度比$24$稍微大一点。

5. What's next?  
接下来呢？

1. Arc length of parametric curves is a natural starting place for learning about line integrals, a central notion in multivariable calculus.
参数曲线的弧长是学习线积分的自然起点，这是多元微积分的核心概念。

6. To keep things from getting too messy as we do so, I first need to go over some more compact notation for these arc length integrals, which you can find in the next article.
为了防止我们这样做时事情变得太混乱，我首先需要讲解一些更紧凑的表示这些弧长积分的符号，你可以在下一篇文章中找到。

1. Summary
    概要

1. To find the arc length of a curve, set up an integral of the form 
   要找到曲线的弧长，建立一个积分形式

--- pic\Arc length of parametric curves.pdf_07.png ---

1.  When the curve is defined parametrically, with $x$ and $y$ given as functions of $t$, take the derivative of both these functions to get $dx$ and $dy$ in terms of $dt$.
当曲线是参数化定义的，用$x$和$y$作为$t$的函数，对这两个函数都求导，得到以$dt$为单位的$dx$和$dy$。

1. Plug these expressions into the integral and factor the $dt^2$ term out of the radical.
将这些表达式代入积分，并将 $dt^2$ 项从根号中提取出来。