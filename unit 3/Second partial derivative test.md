
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

29. In particular, $f_{xx}(0, 0) = 2 > 0$, and the fact that this is positive means $f(x, y)$ looks like it has upward concavity as we travel in the x-direction.
特别地，$f_{xx}(0, 0) = 2 > 0$，这个正数意味着当我们沿x方向移动时，$f(x, y)$看起来像是有向上的凹度。

1. On the other hand, the second partial derivative with respect to y is a negative constant:
另一方面，关于y的二阶偏导数是一个负常数：

--- pic\Second partial derivative test.pdf_05.png ---

1. This indicates downward concavity as we travel in the y-direction. 
    这表明我们在y方向上移动时凹度向下。

32. This mismatch means we must have a saddle point, and it is encoded as the product of the two second partial derivatives: $f_{xx}(0, 0) f_{yy}(0,0) = (2)(-2) = -4 <0$
    这种不匹配意味着我们必须有一个鞍点，它被编码为两个二阶偏导数的乘积：$f_{xx}(0, 0) f_{yy}(0,0) = (2)(-2) = -4 <0$

33. Since $f_{xy}(0,0)^2$ can only be positive, subtracted it will only make the full expression more negative.
    由于 $f_{xy}(0,0)^2$ 只能是正数，减去它只会使整个表达式更为负。

34. On the other hand, when the signs of $f_{xx}(x_0, y_0)$ and $f_{yy}(x_0, y_0)$ are the same, $f_{xx}(x_0, y_0) f_{yy}(x_0, y_0)$ will be positive.
    另一方面，当 $f_{xx}(x_0, y_0)$ 和 $f_{yy}(x_0, y_0)$ 的符号相同时，$f_{xx}(x_0, y_0) f_{yy}(x_0, y_0)$ 将会是正数。

35. But this is not enough! The $f_{xy}$ term also matters.
    但这还不够！$f_{xy}$ 项也很重要。

1. The $f^{2}_{xy}$ term
$f^{2}_{xy}$项

36. Consider the function $f(x,y) =x^2 +y^2 + pxy$ where p is some constant.
    考虑函数 $f(x,y) =x^2 +y^2 + pxy$，其中 p 是某个常数。

2. Concept check: With this definition of f, compute its second derivatives.
概念检查：使用f的这个定义，计算其二阶导数。

--- pic\Second partial derivative test.pdf_06.png ---

1. Because the second derivatives $f_{xx}(0,0)$ and $f_{yy}(0,0)$ are both positive, the graph will appear concave up as we travel in either the pure x direction or the pure y direction (no matter what p is).
因为二阶导数$f_{xx}(0,0)$和$f_{yy}(0,0)$都是正的，所以当我们沿着纯x方向或纯y方向移动时，图形将呈现出凹面向上的形状（无论p是什么）。

2. However, watch the following video where we show how this graph changes as we let the constant p vary from 1 to 3, then back to 1.
然而，请观看下面的视频，我们展示了当我们让常数p从1变化到3，然后又回到1时，这个图形是如何变化的。

--- pic\Second partial derivative test.pdf_07.png ---

1. What's going on here? How can the graph have a saddle point even though it is concave up in both the x and y directions?
    这是怎么回事？尽管图在x方向和y方向上都是凹的，但它怎么会有一个鞍点呢？

39. The short answer is that other directions matter too, and in this case, they are captured by the term $pxy$.
    简短的答案是，其他方向也很重要，在这种情况下，它们被 $pxy$ 项捕获。

40. For example, if we isolate this $xy$ term and look at the graph of $g(x, y) = xy$, here's what it looks like:
    例如，如果我们分离出这个 $xy$ 项，看看 $g(x, y) = xy$ 的图像，它看起来是这样的：

1. Graph of $g(x, y) = xy$. Very similar to the graph of $x² - y²$, but rotated 45° and expanded a bit.
$g(x, y) = xy$的图像。它与$x² - y²$的图像非常相似，但旋转了45°并稍微扩大了一些。

--- pic\Second partial derivative test.pdf_08.png ---
1. It has a saddle point at (0,0). 
    它在(0,0)处有一个鞍点。

1. This is not because the x and y directions disagree about concavity, but instead because the concavity appears positive along the diagonal direction and negative in the other direction.
这不是因为x方向和y方向在凹度上存在分歧，而是因为在对角线方向上凹度呈正，而在其他方向上凹度呈负。

42. Let's see what the second derivative test tells us about the function $f(x,y) =x^2 +y^2 + pxy$.
    让我们看看二阶导数检验对函数 $f(x,y) =x^2 +y^2 + pxy$ 有什么说法。

43. Using the values for the second derivatives you were asked to compute above, here's what we get: $f_{xx} (0, 0) f_{yy}(0,0) -f_{xy}(0,0)^2 = (2)(2) - p^2$.
    使用你在上面被要求计算的二阶导数的值，我们得到：$f_{xx} (0, 0) f_{yy}(0,0) -f_{xy}(0,0)^2 = (2)(2) - p^2$。

44. When $p > 2$, this is negative, so $f$ has a saddle point.
    当 $p > 2$ 时，这是负数，所以 $f$ 有一个鞍点。

45. When $p < 2$, it is positive, so $f$ has a local minimum.
    当 $p < 2$ 时，它是正数，所以 $f$ 有一个局部最小值。

1. You can think of the quantity $f_{xy}(x_0, y_0)$ as measuring how much the function $f$ looks like the graph of $g(x, y) = xy$ near the point $(x_0, y_0)$.
你可以将$f_{xy}(x_0, y_0)$看作是衡量函数$f$在点$(x_0, y_0)$附近看起来像$g(x, y) = xy$的图像的程度。

46. Considering how many directions have to agree with each other, it is actually quite surprising that we only need to consider three values.
    考虑到需要有多少个方向彼此一致，我们只需要考虑三个值，这实际上是相当令人惊讶的。

2. The next article gives more detailed reasoning behind the second partial derivative test.
下一篇文章将给出关于二阶偏导数检验背后更详细的推理。

1. Summary 总结

47. Once you find a point where the gradient of a multivariable function is the zero vector, meaning the tangent plane of the graph is flat at this point, the second partial derivative test is a way to tell if that point is a local maximum, local minimum, or a saddle point.
    一旦你找到一个多元函数的梯度是零向量的点，这意味着图的切平面在这个点是平的，二阶偏导数检验就是一种判断该点是局部最大值、局部最小值还是鞍点的方法。

48. The key term of the second partial derivative test is this: $H = f_{xx}(x_0, y_0) f_{yy}(x_0, y_0) - f_{xy}(x_0, y_0)^2$.
    二阶偏导数检验的关键项是：$H = f_{xx}(x_0, y_0) f_{yy}(x_0, y_0) - f_{xy}(x_0, y_0)^2$。

49. If $H > 0$, the function definitely has a local maximum/minimum at the point $(x_0, y_0)$.
    如果 $H > 0$，函数在点 $(x_0, y_0)$ 处肯定有一个局部最大/最小值。

50. If $H < 0$, the function definitely has a saddle point at $(x_0, y_0)$.
    如果 $H < 0$，函数在点 $(x_0, y_0)$ 处肯定有一个鞍点。

51. If $H = 0$, there is not enough information to tell.
    如果 $H = 0$，信息不足以判断。