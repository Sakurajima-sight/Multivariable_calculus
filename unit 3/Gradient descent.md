
--- pic\Gradient descent.pdf_00.png ---

1. Gradient descent
    梯度下降

2. Gradient descent is a general-purpose algorithm that numerically finds minima of multivariable functions. 
    梯度下降是一种通用算法，可以数值地找到多变量函数的最小值。

3. Background
    背景

4. Gradient
    梯度

5. Maxima and minima
    最大值和最小值

6. So what Is it? Gradient descent is an algorithm that numerically estimates where a function outputs its lowest values. 
    那么它是什么呢？梯度下降是一种算法，它数值地估计了一个函数在哪里输出其最小值。

8. That means It finds local minima, but not by setting $\nabla f$ = 0$ like we've seen before. 
    这意味着它可以找到局部最小值，但不是通过像我们之前看到的那样设置$\nabla f = 0$。

9. Instead of finding minima by manipulating symbols, gradient descent approximates the solution with numbers. 
    梯度下降不是通过操纵符号来找到最小值，而是用数字来近似解。

10. Furthermore, all it needs in order to run Is a function's numerical output, no formula required. 
    此外，运行它所需要的只是函数的数值输出，不需要公式。

11. This distinction is worth emphasizing because it's what makes gradient descent useful. 
    这个区别值得强调，因为这就是使梯度下降有用的地方。

12. If we had a simple formula like $f(x) = x^2$ $\nabla f = 0$ to find that $x = 2$ minimizes $f(x)$. 
    如果我们有一个简单的公式，比如$f(x) = x^2$ $\nabla f = 0$来找到$x = 2$使$f(x)$最小化。

13. Or we could use gradient descent to get a numerical approximation, something like $x \approx 1.99999967$. 
    或者我们可以使用梯度下降来得到一个数值近似，像$x \approx 1.99999967$这样。

14. Both strategies arrive at the same answer. 
    这两种策略得出的答案是相同的。

15. But if we don't have a simple formula for our function, then it becomes hard or impossible to solve $\nabla f = 0$. 
    但是如果我们没有一个简单的函数公式，那么解$\nabla f = 0$就变得困难或不可能。

16. If our function has a hundred or a million variables, then manipulating symbols isn't feasible.
    如果我们的函数有一百个或一百万个变量，那么操纵符号就不可行了。

17. That's when an approximate solution is valuable, and gradient descent can give us these estimates no matter how elaborate our function is.
这就是近似解变得有价值的时候，无论我们的函数多么复杂，梯度下降都可以给我们这些估计。

--- pic\Gradient descent.pdf_01.png ---

1. How gradient descent works
    梯度下降如何工作

18. The way gradient descent manages to find the minima of functions is easiest to imagine in three dimensions. 
    梯度下降找到函数最小值的方式在三维空间中最容易想象。

19. Think of a function $f(x, y)$ that defines some hilly terrain when graphed as a height map. 
    想象一个函数$f(x, y)$，当它被图示为高度图时，它定义了一些丘陵地形。

20. We learned that the gradient evaluated at any point represents the direction of steepest ascent up this hilly terrain. 
    我们了解到，在任何点评估的梯度表示了在这个丘陵地形上最陡峭的上升方向。

21. That might spark an idea for how we could maximize the function: start at a random input, and as many times as we can, take a small step in the direction of the gradient to move uphill. 
    这可能会激发出我们如何能够最大化函数的想法：从一个随机输入开始，尽可能多次地，在梯度的方向上迈出一小步，向上移动。

22. In other words, walk up the hill. 
    换句话说，就是走上山坡。

23. To minimize the function, we can instead follow the negative of the gradient, and thus go in the direction of steepest descent. 
    要最小化函数，我们可以选择跟随梯度的负方向，从而走向最陡峭的下降方向。

24. This is gradient descent. 
    这就是梯度下降。

25. Formally, if we start at a point $x$ and move a positive distance $a$ in the direction of the negative gradient, then our new and improved $x$ will look like this: $x_1 = x_0 -a\nabla f (x_0)$.
    正式地说，如果我们从点$x_0$开始，沿着负梯度方向移动一个正距离$a$，那么我们新的和改进的$x_1$将会如下：$x_1 = x_0 -a\nabla f (x_0)$。

26. More generally, we can write a formula for turning $x_n$ into $x_{n+1}$: $x_{n+1} = x_n - a\nabla f (x_n)$.
    更一般地，我们可以写一个将$x_n$转换为$x_{n+1}$的公式：$x_{n+1} = x_n - a\nabla f (x_n)$。

27. Starting from an initial guess $x_0$, we keep improving little by little until we find a local minimum. 
    从初始猜测$x_0$开始，我们一点一点地改进，直到找到一个局部最小值。

28. This process may take thousands of iterations, so we typically implement gradient descent with a computer.
    这个过程可能需要上千次迭代，所以我们通常用计算机实现梯度下降。

--- pic\Gradient descent.pdf_02.png ---

1. Example 1
    示例 1

30. Consider the function 
    考虑函数

31. As we can see from the graph, this function has many local minima. 
    从图中我们可以看到，这个函数有许多局部最小值。

32. Gradient descent will find different ones depending on our initial guess and our step size. 
    梯度下降会找到不同的局部最小值，具体取决于我们的初始猜测和步长。

1. If we choose $x_0 = 6$ and $\alpha = 0.2$, for example, gradient descent moves as shown in the graph below.
例如，如果我们选择 $x_0 = 6$ 和 $\alpha = 0.2$，梯度下降的移动如下图所示。

33. The first point is $x_0$, and lines connect each point to the next in the sequence. 
    第一个点是$x_0$，线段将序列中的每个点连接到下一个。

34. After only 10 steps, we have converged to the minimum near $x = 4$. 
    只需10步，我们就收敛到了接近$x = 4$的最小值。

2. If we use the same $x_0$ but $\alpha = 1.5$, it seems as if the step size is too large for gradient descent to converge on the minimum.
如果我们使用相同的 $x_0$ 但 $\alpha = 1.5$，则步长似乎对于梯度下降收敛到最小值来说过大。

35. We'll return to this when we discuss the limitations of the algorithm.
    当我们讨论算法的局限性时，我们会回到这个问题。

--- pic\Gradient descent.pdf_03.png ---

1. If we start at $x_0 = 7$ with $\alpha = 0.2$, we descend into a completely different local minimum.
如果我们从 $x_0 = 7$ 开始，取 $\alpha = 0.2$，我们将下降到一个完全不同的局部最小值。

36. Example 2
    示例 2

37. Let's use gradient descent to solve the following problem: how can we best approximate $sin(x)$ with a degree 5 polynomial within the range $-3 < x < 3$? 
    让我们用梯度下降来解决以下问题：我们如何在$-3 < x < 3$的范围内，用5次多项式最好地近似$sin(x)$？

38. In order to use gradient descent, we need to phrase the problem in terms of minimizing a function $f$. 
    为了使用梯度下降，我们需要将问题表述为最小化一个函数$f$。

2. Intuitively, our goal is to find the coefficients $a_0, \ldots, a_5$ that make $p(x)$ as close to $\sin(x)$ as possible while $x$ is between $-3$ and $3$.
直观地说，我们的目标是找到系数 $a_0, \ldots, a_5$，使得当 $x$ 在 $-3$ 和 $3$ 之间时，$p(x)$ 尽可能接近 $\sin(x)$。

40. There are many ways we can turn this idea into a function to minimize.
    有许多方法可以将这个想法转化为一个要最小化的函数。

3. One is called least squares:
一种被称为最小二乘法：

--- pic\Gradient descent.pdf_04.png ---

1. In short, we define our $f$ as the sum of how incorrect $p(x)$ is at each point.
   简单来说，我们定义我们的$f$为每个点处$p(x)$的错误之和。

2. For example, if $p(x) = 2$ near $x = 0$, then $f$ will increase by a lot because $sin(0) = 0$ not 2. 
   例如，如果在$x$接近0时，$p(x) = 2$，那么$f$将大幅增加，因为$sin(0) = 0$而不是2。

3. Gradient descent will try to get $f$ as low as possible, which is the same as making $p(x)$ closer to sin(a). 
   梯度下降将试图使$f$尽可能低，这相当于使$p(x)$更接近$sin(a)$。

4. We square the difference so the integral is always positive. 
   我们对差值进行平方，以便积分始终为正。

1. Here's what happens if we start with  $a_0$  , … ,  $a_5$  as random numbers and then move along the negative gradient.
如果我们以  $a_0$  , … ,  $a_5$  为随机数开始，然后沿着负梯度移动，会发生什么情况。

1. The number in the top left shows how many steps we've taken so far, where we use a step size of $\alpha = 0.001$. 
   左上角的数字显示了我们到目前为止走了多少步，我们使用的步长为$\alpha = 0.001$。

2. We get a pretty good approximation of $sin(x)$! 
   我们得到了一个相当好的$sin(x)$的近似值！

3. Technically, the animation above uses something called momentum gradient descent, which Is a variant that helps it avoid getting stuck in local minima.
   从技术上讲，上面的动画使用了一种叫做动量梯度下降的东西，这是一种变体，可以帮助它避免陷入局部最小值。

--- pic\Gradient descent.pdf_05.png ---

1. The idea is to imagine we are a ball rolling down a hill. 
   这个想法是想象我们是一个滚下山坡的球。

10. As we move, we go faster and faster. 
    随着我们的移动，我们的速度越来越快。

11. If we encounter a small enough local minimum, we will go straight over it because we have the momentum to carry us through it. 
    如果我们遇到一个足够小的局部最小值，我们将直接越过它，因为我们有足够的动量将我们带过去。

12. Without momentum, we get stuck in a local minimum:
    如果没有动量，我们会陷入局部最小值：

1. With momentum, we find the global minimum:
利用动量，我们可以找到全局最小值：

13. Formally, we start with a position $x_0$ and a velocity $v_0$. 
    正式地说，我们从位置$x_0$和速度$v_0$开始。

2. Every step, we add a fraction $\lambda$ (usually around 0.9 ) of the old velocity to the new gradient.
每一步，我们将旧速度的一部分$\lambda$（通常约为0.9）加到新梯度上。

14. That way we keep some of our old momentum each step.
    这样我们每一步都保留一部分旧的动量。

--- pic\Gradient descent.pdf_06.png ---

1. Gradient descent has applications whenever we have a function we want to minimize, which is common in machine learning, for example. 
    无论何时我们有一个我们想要最小化的函数，例如在机器学习中很常见，梯度下降都有应用。

17. But it's important to know its shortcomings so that we can plan around them. 
    但了解其缺点很重要，这样我们才能规避它们。

18. One of its limitations is that it only finds local minima (rather than the global minimum). 
    它的一个限制是它只找到局部最小值（而不是全局最小值）。

19. As soon as the algorithm finds some point that's at a local minimum, it will never escape as long as the step size doesn't exceed the size of the ditch. 
    一旦算法找到某个处于局部最小值的点，只要步长不超过沟的大小，它就永远逃不出来。

20. In the graph above, each local minimum has its own valley that would trap a gradient descent algorithm. 
    在上图中，每个局部最小值都有自己的山谷，会让梯度下降算法陷入其中。

21. After all, the algorithm only ever tries to go down, so once it finds a point where every direction leads up, it will stop. 
    毕竟，算法只是试图下降，所以一旦找到一个所有方向都向上的点，它就会停止。

22. Looking at the graph from a different perspective, we also see that one local minimum is lower than the other. 
    从不同的角度看这个图，我们也可以看到一个局部最小值比另一个更低。

23. When we minimize a function, we want to find the global minimum, but there IS no way that gradient descent can distinguish global and local minima. 
    当我们最小化一个函数时，我们希望找到全局最小值，但是梯度下降无法区分全局和局部最小值。

24. Another limitation of gradient descent concerns the step size $\alpha$.
    梯度下降的另一个限制涉及步长$\alpha$。

1. A good step size moves toward the minimum rapidly, each step making substantial progress.
    一个好的步长能快速地向最小值移动，每一步都能取得实质性的进展。

--- pic\Gradient descent.pdf_07.png ---

1.  Good step size converges quickly. 
    好的步长能快速收敛。

1. If the step size is too large, however, we may never converge to a local minimum because we overshoot it every time.
然而，如果步长过大，我们可能永远无法收敛到局部最小值，因为我们每次都会超过它。

2.  Large step size diverges. 
    大步长会发散。

2. If we are lucky and the algorithm converges anyway, it still might take more steps than it needed.
如果我们幸运的话，算法仍然可能会收敛，但可能需要比所需更多的步骤。

--- pic\Gradient descent.pdf_08.png ---

1. Large step size converges slowly. 
    大步长收敛慢。

1. If the step size is too small, then we'll be more likely to converge, but we'll take far more steps than were necessary.
如果步长过小，那么我们更有可能收敛，但我们将会比必要的步骤多很多。

29. This is a problem when the function we're minimizing has thousands or millions of variables, and evaluating it is cumbersome. 
    当我们要最小化的函数有数千或数百万个变量，而评估它很麻烦时，这就成问题了。

30. Tiny step size converges slowly. 
    微小的步长收敛慢。

31. A final limitation is that gradient descent only works when our function is differentiable everywhere. 
    最后一个限制是，梯度下降只有在我们的函数在任何地方都可微时才工作。

32. Otherwise we might come to a point where the gradient isn't defined, and then we can't use our update formula.
    否则，我们可能会遇到一个梯度未定义的点，然后我们就无法使用更新公式。

--- pic\Gradient descent.pdf_09.png ---

1. Gradient descent fails for non-differentiable functions. 
    对于非可微函数，梯度下降会失败。

34. Summary: Gradient descent minimizes differentiable functions that output a number and have any amount of input variables. 
    概述：梯度下降最小化输出一个数字并有任意数量输入变量的可微函数。

35. It does this by taking a guess $x_0$ and successively applying the formula $x_{n+1} = x_n - \alpha \nabla f (x_n)$. 
    它通过猜测$x_0$并连续应用公式$x_{n+1} = x_n - \alpha \nabla f (x_n)$来实现这一点。

36. In words, the formula says to take a small step in the direction of the negative gradient. 
    用文字来说，公式是说朝负梯度的方向走一小步。

37. Gradient descent can't tell whether a minimum it has found is local or global. 
    梯度下降无法判断找到的最小值是局部的还是全局的。

38. The step size $\alpha$ controls whether the algorithm converges to a minimum quickly or slowly, or whether it diverges. 
    步长$\alpha$控制算法是否快速或慢慢地收敛到最小值，或者是否发散。

39. Many real world problems come down to minimizing a function.
    许多实际问题归结为最小化函数。