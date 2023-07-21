
--- pic\Second partial derivative test.pdf_00.png ---

1. Second partial derivative test
    二阶偏导数测试

2. Learn how to test whether a function with two inputs has a local maximum or minimum.
    学习如何测试一个具有两个输入的函数是否有局部最大值或最小值。
    
1. Background
背景

2. Maximums, minimums, and saddle points
最大值，最小值和鞍点

3. Second partial derivatives
二阶偏导数

4. Not strictly necessary, but used in one section:
不是严格必要的，但在一个部分中使用：

5. The Hessian matrix
海森矩阵

3. Hlso, if you are a little rusty on the second derivative test from single-variable calculus, you might want to quickly review it here since it's a good comparison for the second partial derivative test.
    另外，如果你对单变量微积分的二阶导数测试有些生疏，你可能想在这里快速回顾一下，因为这对二阶偏导数测试是一个很好的对比。

6. [Quick review of second derivative test]
[二阶导数测试的快速回顾]

7. The statement of the second partial derivative test
二阶偏导数测试的声明

4. If you are looking for the local maxima/minima of a two-variable function $f(x,y)$, the first step is to find input points $(x_0, y_0)$ where the gradient is the 0 vector. 
    如果你正在寻找两变量函数$f(x,y)$的局部最大值/最小值，第一步是找到输入点$(x_0, y_0)$在那里梯度是0向量。

5. These are basically points where the tangent plane on the graph of $f$ is flat.
    这些基本上是$f$的图形上切平面是平的点。

--- pic\Second partial derivative test.pdf_01.png ---

1. The second partial derivative test tells us how to verify whether this stable point is a local maximum, local minimum, or a saddle point.
    二阶偏导数测试告诉我们如何验证这个稳定点是局部最大值、局部最小值还是鞍点。

7. Specifically, you start by computing this quantity:
    具体来说，你首先计算这个量：

8. $H = f_{xx}(x_0, y_0) f_{yy}(x_0, y_0) - f_{xy}(x_0, y_0)^2$
    $H = f_{xx}(x_0, y_0) f_{yy}(x_0, y_0) - f_{xy}(x_0, y_0)^2$

9. Then the second partial derivative test goes as follows:
    然后二阶偏导数测试如下：

10. If $H < 0$, then $(x_0, y_0)$ is a saddle point.
    如果 $H < 0$，那么 $(x_0, y_0)$ 是一个鞍点。

11. If $H > 0$, then $(x_0, y_0)$ is either a maximum or a minimum point, and you ask one more question:
    如果 $H > 0$，那么 $(x_0, y_0)$ 是最大点或最小点，你需要再问一个问题：

12. If $f_{xx}(x_0, y_0) < 0$, $(x_0, y_0)$ is a local maximum point.
    如果 $f_{xx}(x_0, y_0) < 0$，那么 $(x_0, y_0)$ 是一个局部最大点。

--- pic\Second partial derivative test.pdf_02.png ---

1. If $f_{xx}(x_0, y_0) > 0$, $(x_0, y_0)$ is a local minimum point.
    如果 $f_{xx}(x_0, y_0) > 0$，那么 $(x_0, y_0)$ 是一个局部最小点。

--- pic\Second partial derivative test.pdf_03.png ---

1. you could also use $f_{yy}(x_0, y_0)$ instead of $f_{xx}(x_0, y_0)$, it actually doesn't matter.
    你也可以使用 $f_{yy}(x_0, y_0)$ 代替 $f_{xx}(x_0, y_0)$，实际上无所谓。

15. If $H = 0$, we do not have enough information to tell.
    如果 $H = 0$，我们没有足够的信息来判断。

1. Hessian determinant
海森矩阵行列式

16. Believe it or not, this key expression $f_{xx}(x_0, y_0) f_{yy}(x_0, y_0) - f_{xy}(x_0, y_0)^2$ was not just handed down from the gods of math.
    信不信由你，这个关键表达式 $f_{xx}(x_0, y_0) f_{yy}(x_0, y_0) - f_{xy}(x_0, y_0)^2$ 不仅仅是数学之神传下来的。

17. It is actually the determinant of the Hessian matrix:
    它实际上是海森矩阵的行列式：

18. In a different tutorial, when I talk about the connections between multivariable calculus and linear algebra, you'll see why this determinant has anything to do with maxima and minima.
    在另一篇教程中，当我谈到多变量微积分和线性代数之间的联系时，你将看到这个行列式为何与最大值和最小值有关。

2. For now, knowing this fact does two things:
目前，了解这个事实有两个作用：

19. It can help you remember what the key expression for the second derivative test is without making little mistakes.
    它可以帮助你记住二阶导数测试的关键表达式，而不会犯小错误。

20. It lets us write the second derivative test much more elegantly:
    它让我们更优雅地写出二阶导数测试：

1. e.g. do you add the square of the mixed partial derivative or subtract it?
例如，你是加上混合偏导数的平方，还是减去它？

21. $det (H_f (x_0, y_0)) < 0$ means $f$ has a saddle point. 
    $det (H_f (x_0, y_0)) < 0$ 表示 $f$ 有一个鞍点。

23. $det (H_f (x_0, y_0)) > 0$ means $f$ has a local maximum or minimum. 
    $det (H_f (x_0, y_0)) > 0$ 表示 $f$ 有一个局部最大值或最小值。

24. $det (H_f (x_0, y_0)) = 0$ means second derivatives alone don't tell us enough to draw a conclusion.
    $det (H_f (x_0, y_0)) = 0$ 表示只有二阶导数还不足以让我们得出结论。

25. Even without linear algebra, we can get a loose intuition for why this expression works as we want it to.
    即使没有线性代数，我们也可以对为什么这个表达式按我们希望的方式工作有一个大概的理解。

3. Loose intuition
粗略的直觉

4. Concavity in x-direction
在x方向的凹性

5. Concavity in y-direction
在y方向的凹性

--- pic\Second partial derivative test.pdf_04.png ---
1. Positive only when x and y directions agree on concavity direction
只有当x和y方向的凹度一致时才为正

2. How much f looks like $g(x, y) = xy$
f看起来有多像$g(x, y) = xy$

1. Focus first on this term: $f_{xx}(x_0, y_0) f_{yy}(x_0, y_0)$
    首先关注这个项：$f_{xx}(x_0, y_0) f_{yy}(x_0, y_0)$

27. You can think of it as cleverly encoding whether or not the concavity of f's graph is the same in both the x and y directions.
    你可以将其视为巧妙地编码了f的图形在x方向和y方向的凹度是否相同。

3. For example, look at the function
例如，看看这个函数

28. This function has a saddle point at $(x, y) = (0,0)$. The second partial derivative with respect to x is a positive constant:
    这个函数在$(x, y) = (0,0)$处有一个鞍点。相对于x的二阶偏导数是一个正常数：

29. In particular, $f_{xx}(x_0, y_0) f_{yy}(x_0, y_0) - f_{xy}(x_0, y_0)^2 > 0$
    特别地，$f_{xx}(x_0, y_0) f_{yy}(x_0, y_0) - f_{xy}(x_0, y_0)^2 > 0$

4. In particular, $f_{xx}(0, 0) = 2 > 0$, and the fact that this is positive means $f(x, y)$ looks like it has upward concavity as we travel in the x-direction.
特别地，$f_{xx}(0, 0) = 2 > 0$，这个正数意味着当我们沿x方向移动时，$f(x, y)$看起来像是有向上的凹度。

5. On the other hand, the second partial derivative with respect to y is a negative constant:
另一方面，关于y的二阶偏导数是一个负常数：