
--- pic\Line integrals in a scalar field.pdf_00.png ---

1. Line integrals in a scalar field
    线积分在标量场中

2. Learn how to compute and interpret line integrals, also known as path integrals or curve integrals.
   学习如何计算和解释线积分，也被称为路径积分或曲线积分。

1. Background
背景

2. Notation for integrating along a curve
沿曲线积分的符号表示

3. Multivariable functions
多元函数

4. Parametric function
参数函数

3. In the same way that an ordinary integral $\int_{a}^{b} f(x) \, dx$ has you walking along the $x$-axis and adding up certain tiny quantities as you go, a line integral $\int_{C} f(x, y) \, ds$ has you walking on a curve in the $x$-$y$-plane, adding up certain quantities depending on the multivariable function $f(x, y)$. 
   就像普通的积分 $\int_{a}^{b} f(x) \, dx$ 让你沿着$x$轴行走，并在行走过程中加上一些微小的量，线积分 $\int_{C} f(x, y) \, ds$ 让你在$x$-$y$平面的曲线上行走，根据多变量函数 $f(x, y)$ 添加一些量。

4. If a curve $C$ is parameterized by a vector-valued function $\mathbf{r}(t)$ between the values $t = a$ and $t = b$, the line integral is written as follows: 
   如果曲线$C$由向量值函数$\mathbf{r}(t)$参数化，$t$的值在$a$和$b$之间，线积分写作：

5. In this case, $f$ is a scalar-valued function, so we call this process "line integration in a scalar field," to distinguish from a related idea we'll cover next: line integration in a vector field.
   在这种情况下，$f$是一个标量值函数，所以我们称这个过程为"在标量场中的线积分"，以便区分我们接下来要讨论的相关概念：在向量场中的线积分。

5. What is a line integral
什么是线积分

--- pic\Line integrals in a scalar field.pdf_01.png ---

1. In the last article, I introduced some compact notation for an arc length integral:
   在上一篇文章中，我为弧长积分引入了一些紧凑的符号。

7. The term $ds$ represents a tiny change in length along the curve.
   术语$ds$代表沿曲线的微小长度变化。

8. Let's say you are given the parametric equations defining the curve: $x(t) = \text{yada yada yada}$, $y(t) = \text{blah blah blah}$.
   假设你被给定了定义曲线的参数方程：$x(t) = \text{yada yada yada}$，$y(t) = \text{blah blah blah}$。

9. Then $ds$, the tiny step along $C$, is given explicitly in terms of $x$ and $y$ using the Pythagorean theorem. 
   然后，沿$C$的微小步长$ds$，使用勾股定理显式地以$x$和$y$表示。

10. You should think of $dx$ and $dy$ as being the $x$ and $y$ components of the tiny step $ds$.
    你应该将$dx$和$dy$看作是微小步长$ds$的$x$和$y$组件。

1. Computationally they are the derivatives of $x(t)$ and $y(t)$:
在计算上，它们是 $x(t)$ 和 $y(t)$ 的导数：

--- pic\Line integrals in a scalar field.pdf_02.png ---

1. $C$ is just a name we give to the curve.
 $C$只是我们给曲线的一个名称。

1. Putting it at the base of the integral, like this $\int_C$, is a way to postpone the need to place actual bounds on the integral.
   将其放在积分的基底，就像$\int_C$这样，是推迟需要在积分上设置实际界限的一种方法。

2.  Consider the curve defined by these parametric equations: $x(t) = t\cos(t)$, $y(t) = t\sin(t)$.
    考虑由这些参数方程定义的曲线：$x(t) = t\cos(t)$，$y(t) = t\sin(t)$。

3.  Let's say we are looking at the portion of this curve between $t = 0$ and $t = 2\pi$, which looks like this:
    假设我们正在查看这条曲线在$t = 0$和$t = 2\pi$之间的部分，看起来像这样：

4.  We start by writing down the integral $\int_C ds = \int_C \sqrt{dx^2 + dy^2}$.
    我们开始写下积分 $\int_C ds = \int_C \sqrt{dx^2 + dy^2}$。

5.  Both $dx$ and $dy$ need to be written in terms of $dt$.
    $dx$和$dy$都需要用$dt$表示。

1. To do this, we take the derivative of each parametric equation,
为了做到这一点，我们对每个参数方程取导数，

--- pic\Line integrals in a scalar field.pdf_03.png ---

1. Both of these values are then plugged into the integral, and we factor the $dt^2$.
    然后将这两个值插入到积分中，并提取$dt^2$。

17. Now that everything inside the integral is written in terms of $t$, we place the bounding values of $t$ on the integral:
    现在，积分内的所有内容都以$t$的形式写出，我们在积分上设置$t$的界限：

1. Super nasty integral, right?
   超级难解的积分，对吧？

2. Welcome to the world of line integrals.
   欢迎来到线积分的世界。

19. Line integrals extend this idea by placing a multivariable function inside the integral.
    线积分通过在积分内放置多变量函数来扩展这个想法。

20. You can think of this integral as saying "Hey, while you're walking along the curve taking tiny steps of size $ds$, rather than just adding up the sizes of those steps, multiply each step size by the value of the function $f(x, y)$ at the point where you are standing.
    你可以将这个积分理解为说，“嘿，当你沿着曲线以$ds$的大小走小步时，而不只是加起那些步的大小，而是将每一步的大小乘以你所站立的点上函数$f(x, y)$的值。

21. The following animation relates this to the more familiar idea of finding the area under a curve.
    下面的动画将此与找到曲线下面积的更熟悉的想法相关联。

22. Imagine a curtain draped under the three-dimensional graph of $f(x, y)$ along the curve $C$ in the $xy$-plane. 
    想象一下沿着$xy$平面的曲线$C$，在$f(x, y)$的三维图下面覆盖的窗帘。

1. The line integral gives the area of that curtain.
线积分给出了那个窗帘的面积。

23. The initial image is a colored contour plot of the function $f(x, y)$.
    初始图像是函数$f(x, y)$的彩色等高线图。


--- pic\Line integrals in a scalar field.pdf_04.png ---

1. You imagine the area of that curtain being broken up into infinitely many infinitely thin rectangles.
   你可以想象那个幕布的面积被无限地分解为无限薄的矩形。

2. The infinitesimal base of each rectangle is $ds = |r'(t)|$, the size of a tiny step along the curve.
   每个矩形的无穷小基底是 $ds = |r'(t)|$，这是沿曲线的微小步长的大小。

3. The height of each rectangle is $f(x, y)$, the height of the graph of $f$ at that point.
   每个矩形的高度是 $f(x, y)$，即在那个点的 $f$ 图的高度。

4. Vector notation for line integrals
   线积分的矢量符号。

5. At the end of the animation above, the line integral is written like this:
   在上面的动画结束时，线积分是这样写的：

6. Let's break down what each part of this means.
   让我们来分解一下这每部分的含义。

7. The parameterization of $C$ 
   $C$的参数化 

1. $\mathbf{r}(t)$ is some vector-valued function which parameterizes the curve $C$.
$\mathbf{r}(t)$ 是某个向量值函数，它参数化了曲线$C$。

1. In two dimensions, it might look something like this:
在二维中，它可能看起来像这样：

--- pic\Line integrals in a scalar field.pdf_05.png ---

1. The bounds of the integral, $a$ and $b$, are values for $t$ which determine where the curve starts and ends.
   积分的界限，$a$ 和 $b$，是决定曲线开始和结束的$t$的值。

10. Essentially this means that as the value of $t$ ranges between $a$ and $b$, the tip of the vector $\mathbf{r}(t)$ traces over the curve $C$.
    本质上，这意味着当$t$的值在$a$和$b$之间变化时，向量$\mathbf{r}(t)$的尖端在曲线$C$上描绘。

1. Composing f with the parameterization
将函数 $f$ 与参数化进行组合

11. Evaluating $f(\mathbf{r}(t))$ means taking the components $x(t)$ and $y(t)$ of $\mathbf{r}(t)$, and plugging them in as the inputs of $f(x, y)$: $f(\mathbf{r}(t)) = f(x(t), y(t))$
    评估 $f(\mathbf{r}(t))$ 意味着取$\mathbf{r}(t)$的组件$x(t)$和$y(t)$，并将它们作为$f(x, y)$的输入：$f(\mathbf{r}(t)) = f(x(t), y(t))$

12. You can think of it this way: A given value of $t$ puts us at some point on the $xy$-plane, expressed as the tip of the vector $\mathbf{r}(t)$. Then $f(\mathbf{r}(t))$ gives the value of the function $f$ at that point on the plane.
    你可以这样想：给定的$t$的值让我们处于$xy$-平面上的某个点，表示为向量$\mathbf{r}(t)$的尖端。然后$f(\mathbf{r}(t))$给出了该平面点上的函数$f$的值。

2. $ds$ is the magnitude of the derivative (times $dt$)
$ds$ 是导数的大小（乘以 $dt$）


13. The term $ds$, representing a tiny step along the curve, is expanded as $|\mathbf{r}'(t)| dt$, the magnitude of the derivative of $\mathbf{r}(t)$ times $dt$.
    项$ds$，代表沿曲线的微小步骤，展开为$|\mathbf{r}'(t)| dt$，即$\mathbf{r}(t)$的导数的大小乘以$dt$。

14. Intuitively, this is because the derivative answers the question "what happens if you nudge the input slightly by a value $dt$?"
    直观地说，这是因为导数回答了“如果你稍微改变输入的值$dt$会发生什么？”这个问题。

3. The answer is that the output gets nudged along the vector $r(t) dt$ in the $xy$-plane.
答案是，输出在 $xy$ 平面上沿着向量 $r(t) dt$ 微移。

--- pic\Line integrals in a scalar field.pdf_06.png ---

1. The magnitude of this nudge in the output space gives you the size of a step $ds$ along the curve, as a function of the size of the step in the parameter space $dt$.
    在输出空间中这种微小变化的大小给出了沿曲线步长$ds$的大小，作为参数空间中步长$dt$的大小的函数。

1. You can also see this as the compact vector-notation way of saying  $\sqrt{(dx)^2 + (dy)^2}$:
你也可以将其视为紧凑的向量表示法，表示为 $\sqrt{(dx)^2 + (dy)^2}$：

3.  Putting all this together, we get the vector representation of a line integral: 
    把所有这些放在一起，我们得到线积分的向量表示：

4.  Example 1: Compute a simple line integral
    示例1：计算一个简单的线积分

1. Let $C$ be one quarter of a circle with radius $2$ centered at the origin.
   设$C$是以原点为中心的半径为$2$的圆的四分之一。

2. The quarter in the first quadrant to be specific.
   具体说来，是第一象限的四分之一。

--- pic\Line integrals in a scalar field.pdf_07.png ---

1. We can describe this quarter circle parametrically with the following function: 
   我们可以用以下函数参数化地描述这个四分之一圆：

2. If we let $t$ range from $0$ to $\frac{\pi}{2}$, this traces around $C$. 
   如果我们让 $t$ 从 $0$ 到 $\frac{\pi}{2}$ 变化，这就在$C$周围形成了轨迹。

3. Now define the multivariable function $f$ as 
现在定义多元函数 $f$ 为

1. Our goal is to compute the line integral $\int_C f(x,y)ds$ 
   我们的目标是计算线积分 $\int_C f(x,y)ds$

1. The following video shows what the "curtain" beneath the graph of $f$ along the curve $C$ looks like.
   下面的视频展示了沿曲线 $C$ 下 $f$ 的图形下的“幕布”是什么样子。

2. The translucent white plane is the graph of $f(x,y) = x+y$, and the blue surface is the curtain whose area we are computing.
   透明的白色平面是 $f(x,y) =x+y$ 的图形，蓝色的表面是我们正在计算的面积的幕布。

--- pic\Line integrals in a scalar field.pdf_08.png ---

1. Curtain between quarter circle and $z=x+y$
   四分之一圆和 $z=x+y$ 之间的幕布

2. Step 1: Write $ds$ in terms of $dt$
   步骤1：以 $dt$ 的形式写出 $ds$

1. Given that the size of a tiny step $ds$ along the curve is given by the magnitude of the derivative of $r(t)$ times $dt$, $ds = |r'(t)|\,dt$ solve for $ds$ in our example.
考虑到沿曲线的一个微小步长 $ds$ 是由 $r(t)$ 的导数的大小乘以 $dt$ 给出的，即 $ds = |r'(t)|\,dt$，在我们的例子中求解 $ds$。

2. For reference, the parameterization of our curve is $r(t)$.
作为参考，我们曲线的参数化是 $r(t)$。

--- pic\Line integrals in a scalar field.pdf_09.png ---

1. In this case, it turns out to be a simple constant multiple of $dt$.
   在这种情况下，它结果是 $dt$ 的一个简单的常数倍。

2. This corresponds with the fact that the given parameterization of C’ has us walking along the curve at a constant rate.
   这对应于给定的 $C$ 的参数化让我们以恒定的速度沿曲线行走的事实。

6. Step 2: Write $f(x, y)$ in terms of $t$
   步骤2：将 $f(x, y)$ 写成 $t$ 的函数

7. What is $f(r(t))$ in this case?
   在这种情况下，$f(r(t))$ 是什么？

1. Every point on the curve $C$ is of the form $(2 \cos(t), 2 \sin(t))$.
曲线 $C$ 上的每一点都形如 $(2 \cos(t), 2 \sin(t))$.

2. Evaluating $f(x, y) = x + y$ at such a point, we get $f(2 \cos(t), 2 \sin(t)) = 2 \cos(t) + 2 \sin(t)$.
在这样的点上求函数 $f(x, y) = x + y$ 的值，我们得到 $f(2 \cos(t), 2 \sin(t)) = 2 \cos(t) + 2 \sin(t)$.

3. Step 3: Write the integral completely in terms of $t$ and solve.
步骤 3：将积分完全用 $t$ 表示并求解.

--- pic\Line integrals in a scalar field.pdf_10.png ---

1. From the previous two steps, our integral becomes
$\int_C f(x, y)ds = \int_C (2\cos(t) + 2\sin(t))2 dt$.
从前两步来看，我们的积分变成了
$\int_C f(x, y)ds = \int_C (2\cos(t) + 2\sin(t))2 dt$.

1. Since our parameterization of $C$ has $t$ running from 0 to $\frac{\pi}{2}$ these are the bounds of the integral. 
由于我们的 $C$ 的参数化使得 $t$ 从 0 运行到 $\frac{\pi}{2}$，这些就是积分的边界。

1.  Now solve the integral.
现在求解积分。

1. Example 2: More intricate practice
例2：更复杂的实践

1. In principle, line integration is not too bad once you get the hang of it. 
原则上，一旦你掌握了线性积分，它并不太糟糕。

1. You just have to know how to expand the term $ds$, and to rewrite the inputs of the function $f(x, y)$ in terms of the parameterization. 
你只需要知道如何展开 $ds$ 这个项，以及如何将函数 $f(x, y)$ 的输入按照参数化重写。

1. Knowing how to set this up just takes a little practice, which is what we're doing here. 
知道如何设置这个只需要一点练习，这就是我们现在正在做的。

1. That said, line integrals can be a real pain to actually compute. 
也就是说，线性积分实际上可能很难计算。

1. Most of them end up in a state where you need to plug the integral into a computer to get an answer, but even when the integral is solvable the numbers involved can quickly grow cumbersome. 
大多数情况下，你需要将积分输入到计算机中才能得到答案，但即使当积分可解时，涉及的数字也可以迅速变得繁琐。

1.  The following example shows how even for relatively simple functions, computing a line integral to its completion can be a very involved problem. 
下面的例子显示了，即使对于相对简单的函数，计算一个线积分到完成也可能是一个非常复杂的问题。

1.  You will definitely want to have a pencil and scratch paper ready if you choose to go through this example.
如果你选择研究这个例子，你一定会希望准备好一支铅笔和草稿纸。

--- pic\Line integrals in a scalar field.pdf_11.png ---

1. Let $C$ be the curve defined by the function $S(t)$ on the interval $1 < t < 2$.
   让 $C$ 表示由函数$S(t)$在区间 $1 < t < 2$ 上定义的曲线。

1. Let $f$ be the function $f(x, y) = xy^2$.
让 $f$ 是函数 $f(x, y) = xy^2$。

2. Compute the line integral $\int_C f ( x , y ) ds$.
计算线积分 $\int_C f ( x , y ) ds$。

3. Step 1: Write $ds$ in terms of $dt$.
步骤1：将 $ds$ 表示为 $dt$ 的函数。

--- pic\Line integrals in a scalar field.pdf_12.png ---

1. By the way, the function under the radical almost never factors so nicely into a square.
   顺便说一句，根号下的函数几乎从不会如此漂亮地分解为一个平方。

2. For practice problems like this, those of us writing the practice problems tend to purposefully engineer them to come out simply.
   对于这样的练习题，我们这些编写练习题的人倾向于有目的地使它们简单化。

3. More often than not, a random line integral you come up with will not give an easily solvable integral.
   大多数情况下，你提出的一个随机线积分不会给出一个易于解的积分。

4. Step 2: Replace $f(x, y)$ with $f (s(t))$
   步骤2：用 $f (s(t))$ 替换 $f(x, y)$

5. What do you get when you plug the components of $s(t)$ into $f(x, y) = xy^2$?
   当你将 $s(t)$ 的组件代入 $f(x, y) = xy^2$ 时，你会得到什么？

--- pic\Line integrals in a scalar field.pdf_13.png ---

1. Step 3: Solve the integral
   步骤3：解积分

10. Plug the answers from the previous two steps into the integral, then solve.
    将前两步的答案代入积分，然后解出。

11. Since the curve Is defined for $1 < t < 2$, and our integral is now given with respect to $t$, the bounds of the integral are 1 and 2. 
    由于曲线的定义域为 $1 < t < 2$，并且现在我们的积分是关于 $t$ 的，因此积分的上下限是 1 和 2。

12. Warning, this gets super ugly to compute, so feel free to put it in a calculator when the time comes. 
    警告，这个计算起来会非常复杂，所以到时候随便用计算器计算。

1. Ugh! Just throw this in a calculator
哎呀！直接用计算器算吧。

--- pic\Line integrals in a scalar field.pdf_14.png ---

1. Notice, the hard part of this problem is not the new principles of line integration, knowing how to expand $ds$ and all that.
    注意，这个问题的难点不在于线积分的新原理，知道如何展开 $ds$ 等。

14. What makes it hard is that the complexity of the terms involved quickly blows up.
    使其变得困难的是参与的项的复杂性快速增加。

15. Also, if you think this is bad, just wait until we get to surface integrals. 
    另外，如果你认为这个很糟糕，等我们接触到面积分就知道了。

16. Line integrals in a scalar field
    标量场中的线积分

17. In everything written above, the function $f$ is a scalar-valued function, meaning it outputs a number (as opposed to a vector).
    在上面写的所有东西中，函数 $f$ 是一个标量函数，意味着它输出一个数（而不是一个向量）。

18. There is a slight variation on line integrals, where you can integrate a vector-valued function along a curve, which we will cover in the next article. 
    在线积分上有一点变化，你可以沿着曲线积分一个向量值函数，我们将在下一篇文章中介绍。

19. To distinguish these ideas, everything we just covered is typically called line integration in a scalar field and the alternative is referred to as line integration in a vector field.
    为了区分这些观念，我们刚才介绍的所有内容通常被称为标量场中的线积分，而替代的方法被称为向量场中的线积分。

1. The term "scalar field" is just another way of thinking about what a multivariable function does: It associates each point in the $x y$ -plane with some scalar (i.e. number), so that the entire plane is like a field of numbers just waiting for someone to wander along a path through that field and integrate those values.
"标量场"这个术语只是另一种思考多变量函数的方式：它将$x y$平面上的每一点与某个标量（即数字）关联起来，使得整个平面就像一个数字的场域，只等待有人沿着该场域的路径进行积分。

2. Line integral animations from wikipedia, originally by Lucas V. Barbosa.
来自维基百科的线积分动画，最初由 Lucas V. Barbosa 制作。