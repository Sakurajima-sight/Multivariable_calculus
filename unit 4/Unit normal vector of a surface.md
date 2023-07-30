
--- pic\Unit normal vector of a surface.pdf_00.png ---

1. Unit normal vector of a surface.
   表面的单位法向量。

1. Learn how to find the vector that is perpendicular, or "normal," to a surface.
   学习如何找到垂直于或“正常”于表面的向量。

2. You will need this skill for computing flux in three dimensions.
   你将需要这项技能来计算三维中的通量。

3. Background
   背景

4. Partial derivatives of parametric surfaces.
   参数曲面的偏导数。

5. In particular, make sure you have a strong intuition for the partial derivatives of a function parameterizing a surface, and what they represent.
   特别是，确保你对参数化一个表面的函数的偏导数有强烈的直觉，并知道它们代表什么。

6. Cross product (video).
   叉积（视频）。

7. What we're building to: If a surface is parameterized by a function $v(t, s)$, the unit normal vector to this surface is given by the expression.
   我们的目标：如果一个表面是由函数$v(t, s)$参数化的，那么这个表面的单位法向量由以下表达式给出。

1. You always have two choices for a unit vector function.
   对于单位向量函数，你总是有两个选择。

2. If a surface is closed, like a sphere or a torus, those choices can be interpreted as outward-facing and inward-facing vectors.
   如果一个表面是封闭的，像球或圆环，那么这些选择可以被解释为向外和向内的向量。

9. This is useful for the idea of flux in three-dimensions, covered in the next article.
   这对于理解下一篇文章中涵盖的三维通量的概念很有用。

10. Unit normal vector
   单位法向量

--- pic\Unit normal vector of a surface.pdf_01.png ---

1. Normal vector
   法向量

2. Let's say you have some surface, $S$. 
   假设你有一些表面，$S$。

3. If a vector at some point on $S$ is perpendicular to $S$ at that point, it is called a normal vector (of $S$ at that point).
   如果在$S$上某点的向量与该点的$S$垂直，那么它被称为法向量（在那点的$S$的法向量）。

4. More precisely, you might say it is perpendicular to the tangent plane of $S$ at that point, or that it is perpendicular to all possible tangent vectors of $S$ at that point.
   更准确地说，你可能会说它垂直于在那点的$S$的切平面，或者它垂直于在那点的$S$的所有可能的切向量。

5. When a normal vector has magnitude 1, it is called a unit normal vector.
   当法向量的大小为1时，它被称为单位法向量。

6. Notice, there will always be two unit normal vectors, each pointing in opposite directions.
   注意，总会有两个单位法向量，它们各自指向相反的方向。

10. Unit normal vector
   单位法向量

--- pic\Unit normal vector of a surface.pdf_02.png ---

1. Why do we care?
   为什么我们在乎？

2. To compute surface integrals in a vector field, also Known as flux, you will need to find an expression for the unit normal vectors on a given surface.
   为了计算向量场中的曲面积分，也被称为通量，你需要找到一个给定曲面上单位法向量的表达式。

2. This will take the form of a multivariable, vector-valued function, whose inputs live in three dimensions (where the surface lives), and whose outputs are three-dimensional vectors.
   这将采用多变量、向量值函数的形式，其输入在三维空间中（即曲面所在的空间），其输出是三维向量。

3. Example: How to compute a unit normal vector.
   示例：如何计算单位法向量。

4. Consider the surface described by the following parametric function:
   考虑由以下参数函数描述的曲面：

4. In the range where $-2 \leq t \leq 2$ and $-2 \leq s \leq 2$, here's what that surface looks like:
   在$-2 \leq t \leq 2$和$-2 \leq s \leq 2$的范围内，这个表面看起来是这样的：

5. For what follows, I am assuming you know that the two vectors, $s$ and $t$, give vectors which are each tangent to the surface, but in different directions.
   在接下来的内容中，我假设你知道两个向量$s$和$t$分别给出了各自与曲面切线的向量，但方向不同。

--- pic\Unit normal vector of a surface.pdf_03.png ---

1. Step 1: Find a (not necessarily unit) normal vector.
   第一步：找到一个（不一定是单位）法向量。

2. Concept check: Which of the following will give a vector which is perpendicular to the surface parameterized by $v$ at the point $v(1, -2)$? Choose 1 answer:
   概念检查：以下哪个选项会给出在点$v(1, -2)$处与由$v$参数化的表面垂直的向量？


--- pic\Unit normal vector of a surface.pdf_04.png ---

1. The first answer choice is correct: 
   第一个答案选项是正确的：

2. If this seems unclear, consider reviewing the video on cross products.
   如果这看起来不清楚，请考虑复习一下关于叉积的视频。

3. Both partial derivative vectors, $\frac{\partial v}{\partial t}(1,-2)$ and $\frac{\partial v}{\partial s}(1,-2)$, are tangent to the surface at the point $v(1, -2)$.
   两个偏导数向量，$\frac{\partial v}{\partial t}(1,-2)$和$\frac{\partial v}{\partial s}(1,-2)$，都在点$v(1, -2)$处与表面相切。

4. Their cross product gives a vector that is perpendicular to both of them, and which is therefore normal to the surface at that point.
   它们的叉积给出了一个与它们两者都垂直的向量，因此该向量在该点处正对着表面。

5. This is a pretty complicated expression, with two vector-valued partial derivatives and a cross product.
   这是一个相当复杂的表达式，包含两个向量值的偏导数和一个叉积。

6. If you have computed some surface integrals before, you are all-too familiar with the expression and how ugly it can be to compute.
   如果你之前计算过一些曲面积分，你就会非常熟悉这个表达式以及计算它有多么繁琐。

7. Once again, here's how $v(t, s)$ is defined.
   再次强调，这就是$v(t, s)$如何定义的。

8. Concept check: Now compute the cross product of the partial derivatives of $v$.
   概念检查：现在计算$v$的偏导数的叉积。

9. Do this for a general point $(t, s)$, meaning each component of your answer will be a function of $t$ and $s$.
   在一般点$(t, s)$上做这个，意味着你答案的每个组成部分都将是$t$和$s$的函数。

10. As described in the previous problem, this will give you a function for normal vectors of the surface.
    如前面的问题所描述的，这将给你一个求表面法向量的函数。

--- pic\Unit normal vector of a surface.pdf_05.png ---

1. Start off by computing each partial derivative.
   首先计算每个偏导数。

2. First, let's do it with respect to $t$: 
   首先，让我们对$t$求偏导数：

3. Next up, with respect to $s$:
   接下来，对$s$求偏导数：

1. Now, take the cross product:
   现在，取叉积：

4. Or, written as an upright vector, here's what we get:
   或者，写成一个直立向量，我们得到的是：

--- pic\Unit normal vector of a surface.pdf_06.png ---

1. For example, if we plugged in $(t, s) = (1, -2)$, here's what we'd get:
   例如，如果我们插入$(t, s) = (1, -2)$，我们将得到以下结果：

2. This is a vector which is perpendicular to the surface at the point $v(1, -2)$.
   这是一个在点$v(1, -2)$处垂直于表面的向量。

2. However, it is not a unit vector, as you can see by computing its magnitude: $\sqrt{21}$.
   但是，它并不是一个单位向量，你可以通过计算其大小$\sqrt{21}$来看出。

3. Step 2: Make that a unit normal vector.
   第二步：将其变为单位法向量。

4. So we have this expression $\begin{bmatrix} 2t \\ -2s \\ 1 \end{bmatrix}$ that gives us a normal vector for each point $v(t, s)$.
   所以我们有这个表达式$\begin{bmatrix} 2t \\ -2s \\ 1 \end{bmatrix}$，它给我们每个点$v(t, s)$的一个法向量。

5. The next step is to massage this a bit to get an expression for a unit normal vector.
   下一步是稍微处理一下这个表达式，以得到一个单位法向量的表达式。

6. Concept check: What is the unit normal vector to our surface at the point $v(1, -2)$?
   概念检查：在点$v(1, -2)$，我们的表面的单位法向量是什么？

--- pic\Unit normal vector of a surface.pdf_07.png ---

1. As I said in the previous section, when we plug in $(t, s) = (1, -2)$ to our general expression for a normal vector, we get:
   正如我在上一节中所说，当我们把$(t, s) = (1, -2)$代入我们对于法向量的一般表达式，我们得到：

2. And this vector has the following magnitude: 
   而这个向量的大小为：

3. To make this a unit vector, then, we will scale it from a vector with length $\sqrt{21}$ to one with length 1.
   为了将这个向量转变为单位向量，我们将把长度为$\sqrt{21}$的向量缩放到长度为1的向量。

4. To do this, divide each component by $\sqrt{21}$: 
   为此，将每个分量除以$\sqrt{21}$：

1. Unit vector 
单位向量

4. Concept check: More generally, what is the unit normal vector to our surface at an arbitrary point $v(t, s)$, as a function of $t$ and $s$? 
   概念检查：更一般地，$v(t, s)$在我们表面上的任意一点的单位法向量是什么，作为$t$和$s$的函数？

5. Our general expression for a (not necessarily unit) normal vector is 
   我们对于（不一定是单位的）法向量的一般表达式是

6. As a function of $t$ and $s$, this vector has magnitude
   作为$t$和$s$的函数，这个向量的大小为

7. To turn our normal vector expression into a unit normal vector expression, divide each term by this magnitude: 
   为了将我们的法向量表达式转化为单位法向量表达式，将每个项除以这个大小：

--- pic\Unit normal vector of a surface.pdf_08.png ---

1. Bada boom bada bang, you've got yourself a unit normal vector.
   噼里啪啦，你得到了一个单位法向量。

2. If you plug in any value $(t_0, s_0)$ to this expression, you will get a vector which has magnitude 1, and is normal to the surface parameterized by the function $v$ at the point $v(t_0, s_0)$.
   如果你将任何值$(t_0, s_0)$代入这个表达式，你将得到一个大小为1的向量，这个向量在点$v(t_0, s_0)$处是由函数$v$参数化的表面的法线。

3. Choosing orientation
   选择方向

4. Notice, if you multiply your function for a unit normal vector by -1, it will still produce unit normal vectors. They will all just point in the opposite directions.
   注意，如果你将单位法向量的函数乘以-1，它仍然会产生单位法向量。它们都只会指向相反的方向。

5. The choice of direction for the unit normal vectors of your surface is what's called an orientation of that surface.
   对于你的表面的单位法向量的方向选择，被称为该表面的定向。

6. You will see the significance of this in the next article on three-dimensional flux.
   你将在下一篇关于三维流量的文章中看到这个的重要性。

7. In short, orienting your surface is analogous to giving a one-dimensional curve a direction.
   简单来说，定向你的表面类似于给一个一维曲线一个方向。

8. When your surface Is closed, like a sphere or a torus, the two choices for unit normal vectors are often called outward-facing and inward-facing unit normal vectors.
   当你的表面是封闭的，比如一个球体或者一个圆环体，单位法向量的两个选择通常被称为朝外的和朝内的单位法向量。

9. Summary: Given a surface parameterized by a function $v(t, s)$, to find an expression for the unit normal vector to this surface, take the following steps:
   总结：给定一个由函数$v(t, s)$参数化的表面，要找到这个表面的单位法向量的表达式，需要进行以下步骤：

10. Step 1: Get a (non necessarily unit) normal vector by taking the cross product of both partial derivatives of $v(t, s)$:
    步骤1：通过求函数$v(t, s)$的两个偏导数的叉积来得到一个（不一定是单位的）法向量：

11. Step 2: Turn this vector-expression into a unit vector by dividing it by its own magnitude:
    步骤2：通过将这个向量表达式除以它自己的模长，将其变为单位向量：

--- pic\Unit normal vector of a surface.pdf_09.png ---

1. You can also multiply this expression by $-1$, and it will still give unit normal vectors.
   你也可以将这个表达式乘以$-1$，它仍然会给出单位法向量。

2. The main reason for learning this skill is to compute three-dimensional flux.
   学习这项技能的主要原因是为了计算三维通量。