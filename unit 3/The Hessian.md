
--- pic\The Hessian.pdf_00.png ---

1. The Hessian
   海森矩阵

2. The Hessian is a matrix that organizes all the second partial derivatives of a function.
   海森矩阵是一个组织函数所有二阶偏导数的矩阵。

3. Background: Second partial derivatives 
   背景：二阶偏导数

1. The Hessian matrix
海森矩阵

1. The "Hessian matrix" of a multivariable function $f(z, y, z, ...)$, which different authors write as $H(f)$, $Hf$, or $H$, organizes all second partial derivatives into a matrix:
多变量函数$f(z, y, z, ...)$的"海森矩阵"，不同的作者将其写为$H(f)$，$Hf$，或$H$，它将所有二阶偏导数组织成一个矩阵：

1. So, two things to notice here: 
   因此，这里要注意两件事：

1. This only makes sense for scalar-valued function.
   这仅适用于标量值函数。

2. This object $Hf$ Is no ordinary matrix; it is a matrix with functions as entries.
   这个对象$Hf$不是普通的矩阵；它是一个条目为函数的矩阵。

3. In other words, it is meant to be evaluated at some point $(x_0, y_0, ...)$.
   换句话说，它是为了在某个点$(x_0, y_0, ...)$上进行评估。

--- pic\The Hessian.pdf_01.png ---

8. As such, you might call this object $Hf$ a "matrix-valued" function.
   因此，你可能会称这个对象$Hf$为"矩阵值"函数。

9. In the single variable world, things were so simple. 
   在单变量世界中，事情是如此简单。

1. The derivative, second derivative, etc.
   导数，二阶导数等。

2.  Now, when a scalar-valued function f has multiple inputs, the analog of the first derivative is the gradient, $\nabla f$, which is a vector-valued function, and the analog of the second derivative is this Hessian $Hf$, which is a matrix-valued function.
    现在，当一个标量函数f有多个输入时，第一导数的类似物是梯度$\nabla f$，它是一个矢量值函数，第二导数的类似物是这个海森矩阵$Hf$，它是一个矩阵值函数。

3.  You might wonder if there are analogous ideas for higher order derivatives, third, fourth, etc. 

    你可能会想知道是否有类似的高阶导数概念，如三阶、四阶等。

1. There are! And there is even a nice extension of Taylor's formula using them all.
   确实有！甚至有一个很好的扩展泰勒公式，使用所有的这些导数。

1. "Really, what are they?", I hear you asking eagerly.
"真的，它们是什么？"我听到你热切地问。

2. Well, expressing them in their full glory involves something called "multilinear algebra".
嗯，全面地表达它们涉及到一种叫做"多线性代数"的东西。

3. It is both fascinating and beautiful, but unfortunately a bit outside the scope of our current discussion.
它既迷人又美丽，但不幸的是，它有点超出了我们当前讨论的范围。

4. Patience.
耐心。

2.  One more important thing, the word "Hessian" also sometimes refers to the determinant of this matrix, instead of to the matrix itself.
    还有一点重要的事情，"海森"这个词有时也指的是这个矩阵的行列式，而不是矩阵本身。

5. Example: Computing a Hessian
示例：计算海森矩阵

6. Problem: Compute the Hessian of $f(x, y) = x^3 - 2xy - y^6$ at the point $(1, 2)$:
问题：在点$(1, 2)$处计算$f(x, y) = x^3 - 2xy - y^6$的海森矩阵：

7. Solution: Ultimately we need all the second partial derivatives of f, so let's first compute both partial derivatives:
解决方案：最终我们需要f的所有二阶偏导数，所以让我们首先计算两个偏导数：

8. With these, we compute all four second partial derivatives:
有了这些，我们计算所有四个二阶偏导数：

--- pic\The Hessian.pdf_02.png ---

13. The Hessian matrix in this case is a $2 \times 2$matrix with these functions as entries.
    在这种情况下，海森矩阵是一个$2 \times 2$的矩阵，其条目为这些函数。

14. We were asked to evaluate this at the point $(x, y) = (1, 2)$, so we plug in these values.
    我们被要求在点$(x, y) = (1, 2)$处对其进行评估，所以我们代入这些值。

15. Now, the problem is ambiguous, since the "Hessian" can refer either to this matrix or to its determinant. 
    现在，问题不明确，因为"海森"可以指代这个矩阵或者其行列式。

1. What you want depends on context.
你想要的取决于上下文。

1. For example, in optimizing multivariable functions, there is something called the "second partial derivative test" which uses the Hessian determinant.
   例如，在优化多变量函数时，有一种叫做"二阶偏导数检验"的方法，它使用海森矩阵的行列式。

2. When the Hessian is used to approximate functions, you just use the matrix itself.
当海森矩阵用于近似函数时，你只需要使用矩阵本身。

1. If it's the determinant we want, here's what we get:
如果我们想要的是行列式，这就是我们得到的：

1.  By capturing all the second-derivative information of a multivariable function, the Hessian matrix often plays a role analogous to the ordinary second derivative in single variable calculus.
    通过捕获多元函数的所有二阶导数信息，海森矩阵经常扮演着与单变量微积分中的普通二阶导数相似的角色。

2.  Most notably, it arises in these two cases: 
    最明显的是，在以下两种情况中，它会出现：

3. Quadratic approximations of multivariable functions, which is a bit like a second order Taylor expansion, but for multivariable functions.
   多元函数的二次近似，这有点像二阶泰勒展开，但用于多元函数。

1. The second partial derivative test, which helps you find the maximum/minimum of a multivariable function.
二阶偏导数检验，它可以帮助你找到多变量函数的最大值/最小值。