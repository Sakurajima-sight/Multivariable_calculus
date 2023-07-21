
--- pic\Reasoning behind second partial derivative test.pdf_00.png ---

1. Reasoning behind second partial derivative test
    对二阶偏导数检验的推理

2. for those of y_0u who want to see why the second partial derivative works, I cover a sketch of a proof here.
    对于那些想要了解为什么二阶偏导数有效的人，我在这里提供了一个证明的概要。

3. Background
    背景

4. Second partial derivative test
    二阶偏导数检验

5. Quadratic approximations
    二次近似法

6. In the last article, I gave the statement of the second partial derivative test, but I only gave a loose intuition for why it's true.
    在上一篇文章中，我给出了二阶偏导数检验的陈述，但我只给出了为什么它是真实的一个模糊的直觉。

7. This article is for those who want to dig a bit more into the math, but it is not strictly necessary if y_0u just want to apply the second partial derivative test.
    这篇文章适合那些想要更深入地探索数学的人，但如果你只是想应用二阶偏导数检验，那么这并不是严格必要的。

1. What we're building to
我们正在构建的是什么

8. To test whether a stable point of a multivariable function is a local minimum/maximum, take a look at the quadratic approximation of the function at that point.
    要测试一个多变量函数的稳定点是否是局部最小值/最大值，可以查看该点的函数的二次近似。

9. It is easier to analyze whether this quadratic approximation has maximum/minimum.
    分析这个二次近似是否有最大值/最小值更容易。

10. for two-variable functions, this boils down to studying expression that look like this: $ax^2 + 2bxy + cy^2$
    对于两变量函数，这归结为研究如下形式的表达式：$ax^2 + 2bxy + cy^2$

11. These are known as quadratic forms.
    这些被称为二次型。

12. The rule for when a quadratic form is always positive or always negative translates directly to the second partial derivative test.
    当一个二次型总是正或总是负的规则可以直接转化为二阶偏导数检验。

2. Single variable case via quadratic approximation
通过二次近似的单变量情况

13. first, I'd like to walk through the formal reasoning behind why the single-variable second derivative test works.
    首先，我想详述一下单变量二阶导数检验为什么有效的正式推理。

14. By formal, I mean capturing the idea of concavity into more of an airtight argument.
    当我说正式时，我是指将凹性的概念更严密地转化为论证。

3. In single-variable calculus, when $f(a) = 0$ for some function $f$ and some input $a$, here's what the second derivative test looks like:
在单变量微积分中，当某个函数$f$和某个输入$a$满足$f(a) = 0$时，二阶导数检验看起来是这样的：

4. $f$ has a local maximum at $a$ if $f''(a) < 0$
如果$f''(a) < 0$，则$f$在$a$处有局部最大值

--- pic\Reasoning behind second partial derivative test.pdf_01.png ---
1. f has a local minimum at a if $f''(a) > 0$
如果$f(a) > 0$，则f在a处有局部最小值。

1. If $f''(a) = 0$, the second derivative alone cannot determine whether f has a maximum, minimum or inflection point at a.
    如果 $f''(a) = 0$，仅仅依靠二阶导数无法确定函数f在a点是否有最大值、最小值或拐点。

16. To think about why this test works, start by approximating the function with a Taylor polynomial out to the quadratic term, also known as a quadratic approximation.
    要理解这个测试为什么有效，首先用泰勒多项式来近似函数，只取到二次项，这也被称为二次近似。

17. Since $f'(a) = 0$, this quadratic approximation simplifies like this: $f(a) + \frac{1}{2} f''(a)(x—a)^2$
    由于 $f'(a) = 0$，这个二次近似可以简化为：$f(a) + \frac{1}{2} f''(a)(x—a)^2$

1. The quadratic approximation at a local minimum.
在局部最小值点的二次近似。

2. Notice, $(x - a)^2 \geq 0$ for all possible x since squares are always positive or zero.
注意，对于所有可能的x，$(x - a)^2 \geq 0$，因为平方总是正数或零。

1. That simple fact tells us everything we need to know! Why?
    这个简单的事实告诉我们我们需要知道的一切！为什么？

2.  It means that when $f''(a) > 0$, we can read our approximation like this: $f(a)+ \frac{1}{2} f''(a)(x—a)^2$
    这意味着当 $f''(a) > 0$时，我们可以像这样读取我们的近似：$f(a)+ \frac{1}{2} f''(a)(x—a)^2$

3. This is $\geq 0$ for all values of x, and equals 0 only when x = a.
这对于所有的x值都是$\geq 0$，只有当x = a时等于0。

--- pic\Reasoning behind second partial derivative test.pdf_02.png ---

1. Therefore a is a local minimum of our approximation. 
    因此a是我们近似的局部最小值。

21. In fact, it is a global minimum, but we only care about the fact that it is a local minimum. 
    实际上，它是全局最小值，但我们只关心它是局部最小值的事实。

22. When the quadratic approximation of a function has a local minimum at the point of approximation, the function itself must also have a local minimum there.
    当函数的二次近似在近似点处有局部最小值时，函数本身也必须在那里有局部最小值。

1. I'll say more on this in the last section, but for now the intuition should be clear since the function and its approximation "hug" one another around the point of approximation a.
我会在最后一节中详细讨论这个问题，但是现在直观的理解应该很清楚，因为函数和它的近似在近似点a附近"相互拥抱"。

23. Similarly, if $f''(a) < 0$, we can read the approximation as $f(a)+ \frac{1}{2} f''(a)(x—a)^2$
    类似地，如果 $f''(a) < 0$，我们可以像这样读取近似：$f(a)+ \frac{1}{2} f''(a)(x—a)^2$

24. This is $\leq 0$ for all values of x, and equals 0 only when $x = a$.
    对于所有的x值都是$\leq 0$，只有当 $x = a$时才等于0。

25. In this case, the approximation has a local maximum at $x = a$, indicating that the function itself also has a local maximum there.
    在这种情况下，近似在 $x = a$处有一个局部最大值，表明函数本身在那里也有一个局部最大值。

--- pic\Reasoning behind second partial derivative test.pdf_03.png ---

1. The quadratic approximation at the inflection point is flat. 
    拐点处的二次近似是平的。

27. When $f''(a) = 0$, our quadratic approximation always equals the constant $f(a)$, meaning our function is in some sense too flat to be analyzed by the second derivative alone. 
    当 $f''(a) = 0$时，我们的二次近似总是等于常数$f(a)$，这意味着我们的函数在某种意义上太平坦，不能仅仅依靠二阶导数进行分析。

1. What to take away from this:
从这里我们可以学到什么：

28. When $f'(a) = 0$, studying whether f has a local maximum or minimum at a comes down to whether the quadratic term of the Taylor approximation $\frac{1}{2} f''(a)(x —a)^2$ is always positive or always negative.
    当 $f'(a) = 0$时，研究f在a处是否有局部最大值或最小值归结为泰勒近似的二次项 $\frac{1}{2} f''(a)(x —a)^2$是否总是正的或总是负的。

2. Two variable case, visual warmup
两个变量的情况，视觉热身


29. Now suppose y_0u have a function $f(x, y)$ with two inputs and one output, and y_0u find a stable point.
    现在假设你有一个函数$f(x, y)$有两个输入和一个输出，并且你找到了一个稳定点。

3. That is, a point where both its partial derivatives are 0,
也就是说，一个点在那里它的两个偏导数都是0，

4. which is more succinctly written as $\nabla f ( x_0 , y_0 ) = 0$
更简洁地写作 $\nabla f ( x_0 , y_0 ) = 0$

5. Zero vector
零向量

--- pic\Reasoning behind second partial derivative test.pdf_04.png ---

1. $\nabla f(x_0,y_0) = 0$ indicates that the tangent plane at $(x_0,y_0)$ is flat. 
    $\nabla f(x_0,y_0) = 0$ 表示在点$(x_0,y_0)$处的切平面是平的。

32. In order to determine whether this is a local maximum, local minimum, or neither, we look to its quadratic approximation. 
    为了确定这是一个局部最大值、局部最小值还是都不是，我们查看其二次近似。

33. Let's start with a visual preview of what we want to do:
    我们从想要做的事情的视觉预览开始：

34. $f$ will have a local minimum at a stable point $(x_0,y_0)$ if the quadratic approximation at that point is a concave-up paraboloid.
    如果在某点的二次近似是一个向上凹的抛物面，那么函数$f$在稳定点$(x_0,y_0)$处将有一个局部最小值。

--- pic\Reasoning behind second partial derivative test.pdf_05.png ---
1. $f$ will have local maximum there if the quadratic approximation is a concave down paraboloid:
如果二次近似是一个向下凹的抛物面，那么函数$f$在那里会有局部最大值。

35. If the quadratic approximation is saddle-shaped, $f$ has neither a maximum nor a minimum, but a saddle point.
    如果二次近似是鞍状的，那么函数$f$既没有最大值也没有最小值，而是一个鞍点。

--- pic\Reasoning behind second partial derivative test.pdf_06.png ---

36. If the quadratic approximation is flat in one or all directions, we do not have enough information to make conclusions about $f$.
    如果二次近似在一个或所有方向上都是平的，我们没有足够的信息来对函数$f$作出结论。

--- pic\Reasoning behind second partial derivative test.pdf_07.png ---

1. Analyzing the quadratic approximation
分析二次近似

2. The formula for the quadratic approximation of f, in vector form, looks like this:
以向量形式表示的f的二次近似公式如下：

3. Since we care about points where the gradient is zero, we can get rid of that gradient term
由于我们关心梯度为零的点，所以我们可以去掉那个梯度项

4. To see this spelled out for the two-variable case, let's expand out the Hessian term,
为了看到这在两变量情况下的详细表述，让我们展开海森矩阵项，

--- pic\Reasoning behind second partial derivative test.pdf_08.png ---

1. This last step follows due to the symmetry of second partial derivatives: $f_{xy} = f_{yx}$
这最后一步是由于二阶偏导数的对称性：$f_{xy} = f_{yx}$

2. (Note, if this approximation or any of the notation feels shaky or unfamiliar, consider reviewing the article on quadratic approximations).
（注意，如果这种近似或任何符号感觉不稳定或不熟悉，可以考虑复习关于二次近似的文章）。

3. As I showed with the single variable case, the strategy is to study if the quadratic term of this approximation is always positive or always negative.
正如我在单变量情况下所展示的，策略是研究这种近似的二次项是否总是正的或总是负的。

--- pic\Reasoning behind second partial derivative test.pdf_09.png ---

1. Is this always > 0?
    这是否总是大于0？

2. Is it always < 0? Can it be either?
    这是否总是小于0？可以是两者之一吗？

3. Right now, this term is a lot to write down, but we can distill its essence by studying expressions of the following form:
    现在，这个项很多，但是我们可以通过研究以下形式的表达式来提取其精华：

4. $ax^2 + 2bxy + cy^2$
    $ax^2 + 2bxy + cy^2$

5. Such expressions are often fancifully called "quadratic forms". 
    这种表达式通常被富有想象力地称为"二次型"。

6. The word "quadratic" indicates that the terms are of order two, meaning they involve the product of two variables.
    "二次"这个词表示项的次数为2，意味着它们涉及到两个变量的乘积。

7. The word "form" always threw me off here, and it makes the idea of a quadratic form sound more complicated than it really is. 
    "形式"这个词总是让我在这里感到困惑，它使得二次型的概念听起来比实际上更复杂。

8. Mathematicians say "quadratic form" instead of "quadratic expression" to emphasize that all terms are of order 2, and there are no linear or constant terms mucking up the expression. 
    数学家们说"二次型"而不是"二次表达式"，以强调所有项都是2阶的，表达式中没有线性或常数项。

9. A phrase like "purely quadratic expression" would have been much too reasonable and understandable to adopt. 
    像"纯二次表达式"这样的短语过于合理和可理解，所以没有被采纳。

10. To make the notation for quadratic forms easier to generalize into higher dimensions, they are often written with respect to a symmetric matrix $M$.
    为了使二次型的表示更容易推广到更高的维度，它们通常以对称矩阵$M$来书写。

11. $x^T Mx = \begin{bmatrix} x & y \end{bmatrix} \begin{bmatrix} a & b \\ b & c \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = x(ax + by) + y(bx + cy) = ax^2 + 2bxy + cy$
    $x^T Mx = \begin{bmatrix} x & y \end{bmatrix} \begin{bmatrix} a & b \\ b & c \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = x(ax + by) + y(bx + cy) = ax^2 + 2bxy + cy$

12. Here is the crucial question:
    这是关键的问题：

13. How can we tell whether the expression $ax^2 + 2bxy + cy^2$ is always positive, always negative, or neither, just by analyzing the constants $a$, $b$, and $c$?
    仅通过分析常数$a$，$b$ 和 $c$，我们如何判断表达式$ax^2 + 2bxy + cy^2$总是正的，总是负的，还是两者都不是？

--- pic\Reasoning behind second partial derivative test.pdf_10.png ---

1.  Analyzing quadratic forms
    分析二次形式

1. If we plug in a constant value $y_0$ for $y$, we get some single variable quadratic function: $ax^2 + 2bx_0y_0 + c(y_0)^2$.
如果我们为$y$插入一个常数值$y_0$，我们将得到一些单变量二次函数：$ax^2 + 2bx_0y_0 + c(y_0)^2$。

2.  The graph of this function is a parabola, and it will only cross the $x$-axis if this quadratic function has real roots.
    这个函数的图像是一个抛物线，只有当这个二次函数有实根时，它才会穿过$x$轴。

3.  A quadratic with two real roots can be both positive and negative. 
    具有两个实根的二次方程可以是正的也可以是负的。

1. Otherwise, it either stays entirely positive or entirely negative, depending on the sign of $a$.
否则，它要么完全为正，要么完全为负，这取决于$a$的符号。

--- pic\Reasoning behind second partial derivative test.pdf_11.png ---

1. A quadratic with no real roots can either be entirely positive or entirely negative. 
    一个没有实根的二次方程要么完全为正，要么完全为负。

41. We can apply the quadratic formula to this expression to see whether its roots are real or complex. 
    我们可以将二次公式应用到这个表达式中，以查看它的根是实数还是复数。

1. The leading term is $a$. The linear term is $2by_0$. The constant term is $$c(y_0)^2$$.
领先项是$a$。线性项是$2by_0$。常数项是$c(y_0)^2$。

1.  Applying the quadratic formula looks like this: 
    应用二次公式看起来像这样：

2.  If $y_0 = 0$, the quadratic has a double root at $x = 0$, meaning the parabola barely kisses the x-axis at that point.
    如果$y_0 = 0$，二次方程在$x = 0$处有一个双重根，这意味着抛物线在那一点几乎只是轻轻地接触了x轴。

1. Otherwise, whether or not these roots are real depends only on the sign of the expression $b^2 - ac$.
否则，这些根是否为实数只取决于表达式$b^2 - ac$的符号。

1. If $b − ac ≥ 0$, there are real roots, so the graph of $ax + 2bxy_0 + c(y_0)$ crosses the $x$ -axis.
如果 $b − ac ≥ 0$，那么存在实根，因此 $ax + 2bxy_0 + c(y_0)$ 的图形会穿过$x$轴。

--- pic\Reasoning behind second partial derivative test.pdf_12.png ---

1. Otherwise, if $b^2 − a c < 0$, there are no real roots, so the graph of $a x^2 + 2 b x y_0 + c ( y_0 )^2$ either stays entirely positive or entirely negative.
否则，如果 $b^2 - ac < 0$，则没有实根，因此 $a x^2 + 2 b x y_0 + c ( y_0 )^2$ 的图形要么完全为正，要么完全为负。

2. For example, consider the case
例如，考虑以下情况

1. In this case, $b - ac = 3^2 - (1)(5) = 4 > 0$, so the graph of $f(x) = x^2 + 6xy_0 + 5y_0^2$ always crosses the x-axis.
在这种情况下，$b - ac = 3^2 - (1)(5) = 4 > 0$，所以函数$f(x) = x^2 + 6xy_0 + 5y_0^2$的图像总是会穿过x轴。

1. Here is a video showing how that graph moves around as we let the value of y 0 slowly change.
这是一个视频，展示了当我们让$y_0$的值慢慢改变时，图形是如何移动的。

3. This corresponds with the fact that the graph of $f ( x , y ) = x^2 + 6 x y + 5 y^2$ can be both positive and negative.
这对应于 $f ( x , y ) = x^2 + 6 x y + 5 y^2$ 的图形可以既为正又为负的事实。

--- pic\Reasoning behind second partial derivative test.pdf_13.png ---

1. In contrast, consider the case
    相反，考虑以下情况

1. Now, $b - ac = 2 - (2)(3) = -2 < 0$.
现在，$b - ac = 2 - (2)(3) = -2 < 0$。

35. This means the graph of $f(x) = 2x^2 + 4xy_0 + 3y_0^2$ never crosses the z-axis, although it kisses it if the constant y_0 is zero.
    这意味着 $f(x) = 2x^2 + 4xy_0 + 3y_0^2$ 的图形从未越过z轴，尽管如果常数y_0为零，它会接触z轴。

1.  Here is a video showing how that graph changes as we let the constant $y_0$ vary.
    这里有一个视频，展示了当我们让常数$y_0$变化时，图形是如何改变的。

2.  This corresponds with the fact that the multivariable function $f(x) = 2x^2 + 4xy_0 + 3y_0^2$ is always positive.
    这对应于多变量函数 $f(x) = 2x^2 + 4xy_0 + 3y_0^2$ 总是正的这个事实。

--- pic\Reasoning behind second partial derivative test.pdf_14.png ---

1. Rule for the sign of quadratic forms
    二次形式符号的规则

1. As if to confuse students who are familiar with the quadratic formula, rules regarding quadratic forms are often phrased with respect to $ac - b^2$ instead of $b^2 - ac$.
对于熟悉二次公式的学生来说，关于二次型的规则通常是根据$ac - b^2$而不是$b^2 - ac$来表述的，这似乎是为了混淆学生。

2. Since one is the negative of the other, this requires switching when you say $≥ 0$ and when you say $≤ 0$.
由于一个是另一个的负数，所以当你说$≥ 0$和$≤ 0$时需要切换。

40. The reason mathematicians prefer $ac - b^2$ is because this is the determinant of the matrix describing the quadratic form.
    数学家们更喜欢$ac - b^2$的原因是因为这是描述二次形式的矩阵的行列式。

41. As a reminder, this is how the quadratic form looks using the matrix. 
    提醒一下，这就是使用矩阵的二次形式的样子。

1. Tying this convention together with what we found in the previous section, we write the rule for the sign of a quadratic form as follows.
将这个约定与我们在前一节中发现的内容结合起来，我们写下了二次形式符号的规则，如下所示。

42. If $ac - b^2<0$, the quadratic form can attain both positive and negative values, and it's possible for it to equal 0 at values other than $(x, y) = (0,0)$. 
    如果 $ac - b^2<0$，二次形式可以取得正值和负值，并且在 $(x, y) = (0,0)$ 的值上可能等于0。

3. If $ac - b^2 > 0$ the form is either always positive or always negative depending on the sign of $a$, but in either case it only equals 0 at $(x, y) = (0, 0)$.
如果$ac - b^2 > 0$，那么这个形式要么总是正的，要么总是负的，这取决于$a$的符号，但在任何情况下，它只在$(x, y) = (0, 0)$时等于0。

43. If $a > 0$, the form is always positive, so $(0, 0)$ is a global minimum point of the form. 
    如果 $a > 0$，形式总是正的，所以 $(0, 0)$ 是形式的全局最小点。

44. If $a < 0$, the form is always negative, so $(0, 0)$ is a global maximum point of the form. 
    如果 $a < 0$，形式总是负的，所以 $(0, 0)$ 是形式的全局最大点。

45. If $ac - b^2 = 0$, the form will again either be always positive or always negative, but now it's possible for it to equal 0 at values other than $(x, y) = (0, 0)$.
如果$ac - b^2 = 0$，那么这个形式再次要么总是正的，要么总是负的，但现在它有可能在$(x, y) = (0, 0)$以外的值处等于0。

1. Some terminology:
一些术语：

1. When $ax^2 + 2bxy + cy^2 > 0$ for all $(x, y)$ other than $(x, y) = (0, 0)$, the quadratic form and the matrix associated with it are both called positive definite.
当对于所有$(x, y)$（除了$(x, y) = (0, 0)$）都有$ax^2 + 2bxy + cy^2 > 0$时，二次型和与之关联的矩阵都被称为正定的。

1. When $ax^2 + 2bxy + cy^2 < 0$ for all $(x, y)$ other than $(x, y) = (0, 0)$, they are both negative definite.
当对于所有$(x, y)$（除了$(x, y) = (0, 0)$）都有$ax^2 + 2bxy + cy^2 < 0$时，它们都是负定的。

1. If you replace the $>$ and $<$ with $≥$ and $≤$, the corresponding properties are positive semi-definite and negative semi-definite.
如果你将$>$和$<$替换为$≥$和$≤$，相应的性质就是半正定和半负定。

--- pic\Reasoning behind second partial derivative test.pdf_15.png ---

1. Applying this to $Q_f$ ;
    将此应用于 $Q_f$ ；

32. Okay zooming back out to where we started, let's write down our quadratic approximation again:
    好的，让我们回到开始的地方，再次写下我们的二次近似：

33. The quadratic portion of  $Q_f$  is written with respect to $(x - x_0)$ and $(y - y_0)$ instead of simply $x$ and $y$,so everywhere where the rule for the sign of quadratic forms references the point $(0,0)$, we apply it instead to the point $(x_0, y_0)$.
     $Q_f$  的二次部分是相对于 $(x - x_0)$ 和 $(y - y_0)$ 而不仅仅是 $x$ 和 $y$ 来写的，所以，对于二次型符号规则引用点 $(0,0)$ 的所有地方，我们将其应用于点 $(x_0, y_0)$。
    

34. As with the single-variable case, when the quadratic approximation  $Q_f$  has a local maximum (or minimum) at $(x_0, y_0)$, it means $f$ has a local maximum (or minimum) at that point.
    和单变量情况一样，当二次近似  $Q_f$  在 $(x_0, y_0)$ 处有一个局部最大值（或最小值），这意味着 $f$ 在那点有一个局部最大值（或最小值）。

35. This means we can translate the rule for the sign of a quadratic form directly to get the second derivative test:
    这意味着我们可以直接将二次型符号的规则翻译为二阶导数测试：

36. Suppose $\nabla f(x_0, y_0) = 0$, then
    假设 $\nabla f(x_0, y_0) = 0$，那么

1. If $f_{xx}(x_0, y_0)f_{yy}(x_0, y_0) - (f_{xy}(x_0, y_0))^2 < 0$, f has neither a minimum nor a maximum at $(x_0, y_0)$, but instead has a saddle point.
如果$f_{xx}(x_0, y_0)f_{yy}(x_0, y_0) - (f_{xy}(x_0, y_0))^2 < 0$，函数f在$(x_0, y_0)$处既不是最小值也不是最大值，而是一个鞍点。

--- pic\Reasoning behind second partial derivative test.pdf_16.png ---

1. If $f_{xx} (x_0, y_0) f_{yy}(x_0, y_0) - (f_{xy} (x_0, y_0))^2 > 0$, $f$ definitely has either a maximum or minimum at $(x_0, y_0)$, and we must look at the sign of $f_{xx}(x_0, y_0)$ to figure out which one it is.
    如果 $f_{xx} (x_0, y_0) f_{yy}(x_0, y_0) - (f_{xy} (x_0, y_0))^2 > 0$，$f$ 一定在 $(x_0, y_0)$ 处有一个最大值或最小值，我们必须查看 $f_{xx}(x_0, y_0)$ 的符号以确定是哪一个。

1. If $f_{xx}(x_0, y_0) > 0$, $f$ has a local minimum.
如果 $f_{xx}(x_0, y_0) > 0$，那么$f$在局部有最小值。

41. If $f_{xx}(x_0, y_0) < 0$, $f$ has a local maximum.
    如果 $f_{xx}(x_0, y_0) < 0$，$f$ 有一个局部最大值。

--- pic\Reasoning behind second partial derivative test.pdf_17.png ---

1. If $f_{xx} (x_0, y_0) f_{yy}(x_0, y_0) - (f_{xy} (x_0, y_0))^2 = 0$, the second derivatives alone cannot tell us whether $f$ has a local minimum or maximum.
    如果 $f_{xx} (x_0, y_0) f_{yy}(x_0, y_0) - (f_{xy} (x_0, y_0))^2 = 0$，仅凭二阶导数我们无法判断 $f$ 是否有局部最小值或最大值。

43. Our current tools are lacking.
    我们当前的工具不足。

44. Everything presented here almost constitutes a full proof, except for one final step.
    这里所呈现的所有内容几乎构成了一个完整的证明，除了最后一步。

45. Intuitively, it might make sense that when a quadratic approximation bends and curves in a certain way, the function should bend and curve in that same way near the point of approximation.
    从直观上看，当二次近似以某种方式弯曲和曲线时，函数应该在近似点附近以同样的方式弯曲和曲线。

46. But how do we formalize this bey_0nd intuition?
    但是我们如何在直觉之外形式化这个问题？

47. Unfortunately, we will not do that here.
    不幸的是，我们在这里不会做那样的事情。

48. Making arguments about derivatives fully rigorous requires using real analysis, the theoretical backbone of calculus.
    完全严格地对导数进行论证需要使用实分析，这是微积分的理论支柱。

49. Furthermore, y_0u might be wondering how this generalizes to functions with more than two inputs.
    此外，你可能会想知道这如何推广到具有多于两个输入的函数。

50. There is a notion of quadratic forms with multiple variables, but phrasing the rule for when such forms are always positive or always negative uses various ideas from linear algebra.
    有一种多变量的二次型的概念，但是表述这样的形式何时总是正或总是负的规则使用了线性代数的各种概念。

--- pic\Reasoning behind second partial derivative test.pdf_18.png ---

1. Summary.
    总结。

52. To test whether a stable point of a multivariable function is a local minimum/maximum, take a look at the quadratic approximation of the function at that point.
    要测试一个多变量函数的稳定点是否是局部最小值/最大值，看一看在那点的函数的二次近似。

53. It is easier to analyze whether this quadratic approximation has maximum/minimum.
    分析这个二次近似是否有最大值/最小值更容易。

54. for two-variable functions, this boils down to studying expressions that look like this: $ax^2 + 2bxy + cy^2$.
    对于二变量函数，这归结为研究像这样的表达式：$ax^2 + 2bxy + cy^2$。

55. These are known as quadratic forms.
    这些被称为二次型。

56. The rule for when a quadratic form is always positive or always negative translates directly to the second partial derivative test.
    一个二次型何时总是正或总是负的规则直接翻译为二阶偏导数测试。