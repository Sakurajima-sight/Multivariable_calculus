
---
--- pic\Lagrange multipliers, examples.pdf_00.png ---
1. Lagrange multipliers, examples
    拉格朗日乘数法的例子

2. Examples of the Lagrangian and Lagrange multiplier technique in action.
    拉格朗日函数和拉格朗日乘数技术在实际操作中的例子。

1. Background
背景

2. Introduction to Lagrange multipliers
拉格朗日乘数法介绍

3. Gradient
梯度

4. When you want to maximize (or minimizet another multivariable function equals a constant, $g(x, y, \ldots) a multivariable function $f(x, y, \ldots)$ subject to the constraint tha) = c$, follow these steps:
当你想要最大化（或最小化）一个多变量函数 $f(x, y, \ldots)$，并且受到另一个多变量函数等于常数的约束，即 $g(x, y, \ldots) = c$，请按照以下步骤操作：

5. Step 1: Introduce a new variable $\lambda$, and define a new function $L$ as follows:
步骤1：引入一个新的变量 $\lambda$，并按照以下方式定义一个新的函数 $L$：

1. This function $L$ is called the "Lagrangian", and the new variable $\lambda$ is referred to as a "Lagrange multiplier".
    这个函数$L$被称为“拉格朗日函数”，新的变量$\lambda$被称为“拉格朗日乘数”。

6. Step 2: Set the gradient of $L$ equal to the zero vector.
    步骤2：设定$L$的梯度等于零向量。

--- pic\Lagrange multipliers, examples.pdf_01.png ---

1. In other words, find the critical points of $L$. 
    换句话说，找到$L$的临界点。

8. Step 3: Consider each solution, which will look something like $(x_0, y_0,..., \lambda_0)$. 
    步骤3：考虑每一个解，这些解看起来应该是类似$(x_0, y_0,..., \lambda_0)$的形式。

9. Plug each one into $f$. 
    将每一个解代入$f$。

1. Or rather, first remove the $\lambda_0$ component, then plug It into $f$, since $f$ does not have $\lambda$ as an input. 
或者，首先去掉$\lambda_0$这一部分，然后再将其代入$f$，因为$f$没有$\lambda$这一输入。

10. Whichever one gives the greatest (or smallest) value is the maximum (or minimum) point your are seeking. 
    那个给出最大（或最小）值的就是你要找的最大值（或最小值）点。

1. Example 1: Budgetary constraints
示例1：预算约束

11. Suppose you are running a factory, producing some sort of widget that requires steel as a raw material. 
    假设你正在运营一个工厂，生产一种需要钢铁作为原材料的部件。

12. Your costs are predominantly human labor, which is $20 per hour for your workers, and the steel itself, which runs for $170 per ton. 
    你的成本主要是人力，你的工人每小时20美元，还有钢铁本身，每吨170美元。

13. Suppose your revenue $R$ is loosely modeled by the following equation: 
    假设你的收入$R$被大致模拟为以下公式：

1. $h$ represents hours of labor
$h$ 代表劳动小时数

2. $s$ represents tons of steel
$s$ 代表钢的吨数

14. If your budget is $20,000, what is the maximum possible revenue? 
    如果你的预算是$20,000，那么最大可能的收入是多少？

15. The $20 per hour labor costs and $170 per ton steel costs tell us that the total cost of production, in terms of $h$ and $s$, is $20h + 170s$. 
    每小时20美元的劳动力成本和每吨170美元的钢铁成本告诉我们，以$h$和$s$来计算的话，生产的总成本是$20h + 170s$。

16. Therefore the budget of $20,000 can be translated to the constraint $20h + 170s = 20,000$.
    因此，$20,000的预算可以被转化为约束条件$20h + 170s = 20,000$。

2. Before we dive into the computation, you can get a feel for this problem using the following interactive diagram.
在我们深入计算之前，你可以通过以下的交互式图表来理解这个问题。

3. You can see which values of $(h, s)$ yield a given revenue (blue curve) and which values satisfy the constraint (red line).
你可以看到哪些$(h, s)$的值能得到给定的收入（蓝色曲线），以及哪些值满足约束（红线）。

--- pic\Lagrange multipliers, examples.pdf_02.png ---
1. Since we need to maximize a function $R(h, s)$, subject to a constraint, $20h + 170s = 20,000$, we begin by writing the Lagrangian function for this setup: $L(h, s, \lambda) = 200h^{2/3} + S^{1/3} - \lambda(20h + 170s - 20,000)$.
    因为我们需要在约束条件$20h + 170s = 20,000$下最大化函数$R(h, s)$，我们首先写出对应这个问题的拉格朗日函数：$L(h, s, \lambda) = 200h^{2/3} + S^{1/3} - \lambda(20h + 170s - 20,000)$。

18. Next, set the gradient $\nabla L$ equal to the 0 vector. 
    接下来，设定梯度$\nabla L$等于零向量。

1. This is the same as setting each partial derivative equal to 0. 
这和设定每一个偏导数等于0是一样的。

19. First, we handle the partial derivative with respect to $h$.
    首先，我们处理对$h$的偏导数。

20. Next, we handle the partial derivative with respect to $s$.
    接下来，我们处理对$s$的偏导数。

--- pic\Lagrange multipliers, examples.pdf_03.png ---

1. Finally we set the partial derivative with respect to $\lambda$ equal to 0, which as always is just the same thing as the constraint.
最后我们设定对$\lambda$的偏导数等于0，这和以往一样，就等于约束条件。

1. In practice, you can of course just write the constraint itself, but I'll write out the partial derivative here just to make things clear.
在实践中，你当然可以直接写出约束本身，但我会在这里写出偏导数，以便清楚地说明。

22. Putting it together, the system of equations we need to solve is:
综合起来，我们需要解决的方程组是：

23. In practice, you should almost always use a computer once you get to a system of equations like this.
在实际操作中，当你得到一个这样的方程组时，你几乎总是应该使用电脑来解决。

24. Especially because the equation will likely be more complicated than these in real applications.
特别是因为在真实的应用中，方程很可能比这些更复杂。

25. Once you do, you'll find that the answer is
一旦你使用电脑，你会发现答案是

2. This means you should employ about 667 hours of labor, and purchase 39 tons of steel, which will give a maximum revenue of
这意味着你应该雇用大约667小时的劳动力，并购买39吨的钢材，这将带来最大的收入。

--- pic\Lagrange multipliers, examples.pdf_04.png ---

1. The interpretation of this constant $\lambda = 2.593$ is left to the next article.
对这个常数 $\lambda = 2.593$ 的解释将留到下一篇文章中。

2. Example 2: Maximizing dot product
示例2：最大化点积

4. Problem: Let the three-dimensional vector $v$ be defined as follows.
问题：让三维向量$v$按照以下方式定义。

5. Consider every possible unit vector $u$ in three-dimensional space.
考虑三维空间中的每一个可能的单位向量$u$。

6. For which one is the dot product $u \cdot v$ the greatest? 
对于哪一个单位向量$u$，点积$u \cdot v$最大？

7. The diagram below is two-dimensional, but not much changes in the intuition as we move to three dimensions.
下面的图是二维的，但当我们转向三维时，直觉并没有太大的改变。

8. Two-dimensional analogy to the three-dimensional problem we have.
我们有的三维问题的二维类比。

9. Which unit vector $u$ maximizes the dot product $u \cdot v$? 
哪个单位向量$u$可以最大化点积$u \cdot v$？

10. It's one of those mathematical facts worth remembering.
这是值得记住的数学事实之一。

11. If you don't know the answer, all the better!
如果你不知道答案，那就更好了！

12. Because we will now find and prove the result using the Lagrange multiplier method.
因为我们现在将使用拉格朗日乘数法找出并证明结果。

--- pic\Lagrange multipliers, examples.pdf_05.png ---

1. First, we need to spell out how exactly this is a constrained optimization problem.
    首先，我们需要明确这到底是一个受约束的优化问题。

1.  Write the coordinates of our unit vectors as $x$, $y$ and $z$:
    将我们的单位向量的坐标写为$x$，$y$和$z$：

2.  The fact that $u$ is a unit vector means its magnitude is 1:
    $u$是单位向量，这意味着其幅值为1:

3.  This is our constraint.
    这是我们的约束。

4.  Maximizing $u \cdot v$ means maximizing the following quantity:
    最大化$u \cdot v$意味着最大化以下的数量：

5.  The Lagrangian, with respect to this function and the constraint above, is $L(x,y,z,\lambda) = 2x + 3y + 1z - \lambda(x^2 + y^2 + z^2 - 1)$.
    关于此函数和上述约束的拉格朗日函数是$L(x,y,z,\lambda) = 2x + 3y + 1z - \lambda(x^2 + y^2 + z^2 - 1)$。

6.  We now solve for $\nabla L = 0$ by setting each partial derivative of this expression equal to 0.
    我们现在通过使这个表达式的每个偏导数等于0来解决$\nabla L = 0$。

7.  Remember, setting the partial derivative with respect to $\lambda$ equal to 0 just restates the constraint.
    记住，将关于$\lambda$的偏导数设置为0只是重申了约束。

1. Solving for x , y and z in the first three equations above, we get
在上述的前三个等式中解出 $x$，$y$ 和 $z$，我们得到

--- pic\Lagrange multipliers, examples.pdf_06.png ---

1. Ah, what beautiful symmetry. 
   啊，多么美丽的对称。

2. Each of these expressions has the same $\frac{1}{2\lambda}$ factor, and the coefficients 2, 3 and 1 match up with the coordinates of $\mathbf{v}$.
   每个表达式都有相同的$\frac{1}{2\lambda}$因子，且系数2、3和1与向量$\mathbf{v}$的坐标匹配。

3. Being good math students as we are, we won't let good symmetry go to waste.
   作为优秀的数学学生，我们不会让这美丽的对称性白白浪费。

4. In this case, combining the three equations above into a single vector equation, we can relate $\mathbf{u}$ and $\mathbf{v}$ as follows:
   在这种情况下，我们可以将上述三个方程结合成一个向量方程，从而将向量$\mathbf{u}$和$\mathbf{v}$关联起来，如下所示：

5. Therefore $\mathbf{u}$ is proportional to $\mathbf{v}$! Geometrically, this means $\mathbf{u}$ points in the same direction as $\mathbf{v}$.
   因此，向量$\mathbf{u}$与向量$\mathbf{v}$成比例！从几何的角度来看，这意味着$\mathbf{u}$指向与$\mathbf{v}$相同的方向。

6. There are two unit vectors proportional to $\mathbf{v}$.
   有两个与向量$\mathbf{v}$成比例的单位向量。

1. One which points in the same direction, this is the vector that maximizes $u \cdot v$.
指向相同的方向的向量，这是最大化 $u \cdot v$ 的向量。

1. One which points in the opposite direction. This one minimizes $u \cdot v$.
指向相反的方向的向量，这是最小化 $u \cdot v$ 的向量。

1. We can write these two unit vectors by normalizing $v$, which just means dividing $v$ by its magnitude:
我们可以通过归一化 $v$ 来写出这两个单位向量，这只意味着将 $v$ 除以其大小：

1. The magnitude $v = \sqrt{14}$, so we can write the maximizing unit vector $u_{\text{max}}$ explicitly as like this:
大小 $v = \sqrt{14}$，所以我们可以明确地写出最大化单位向量 $u_{\text{max}}$，就像这样：


--- pic\Lagrange multipliers, examples.pdf_07.png ---

1.  Just skip the Lagrangian.
    直接跳过拉格朗日乘子。

2.  If you read the last article, you'll recall that the whole point of the Lagrangian $L$ is that setting $\nabla L = 0$ encodes the two properties a constrained maximum must satisfy:
    如果你阅读了上一篇文章，你会回想起拉格朗日乘子$L$的全部重点是，设定$\nabla L = 0$ 编码了约束最大值必须满足的两个属性：

3.  Gradient alignment between the target function and the constraint function, $\nabla f(x, y) =\lambda\nabla g(x, y)$.
    目标函数和约束函数之间的梯度对齐，$\nabla f(x, y) =\lambda\nabla g(x, y)$。

4.  The constraint itself, $g(x,y) =c$.
    约束本身，$g(x,y) =c$。

5.  When working through examples, you might wonder why we bother writing out the Lagrangian at all.
    在处理实例时，你可能会纳闷我们为什么要费力写出拉格朗日函数。

6.  Wouldn't it be easier to just start with these two equations rather than re-establishing them from $\nabla L = 0$ every time? 
    直接从这两个等式开始，而不是每次都从$\nabla L = 0$重新开始，难道不更容易吗？

7.  The short answer is yes, it would be easier. 
    简单的回答是，是的，这会更容易。

8.  If you find yourself solving a constrained optimization problem by hand, and you remember the idea of gradient alignment, feel free to go for it without worrying about the Lagrangian.
    如果你发现自己在手动解决一个有约束的优化问题，并且你记得梯度对齐的概念，那么尽管去做，不用担心拉格朗日乘子。

9.  In practice, it's often a computer solving these problems, not a human. 
    在实践中，往往是计算机而不是人在解决这些问题。

10. Given that there are many highly optimized programs for finding when the gradient of a given function is 0, it's both clean and useful to encapsulate our problem into the equation $\nabla L = 0$.
    考虑到有许多高度优化的程序可以找出给定函数的梯度何时为0，将我们的问题封装到等式$\nabla L = 0$中是清晰而有用的。

22. Furthermore, the Lagrangian itself, as well as several functions deriving from it, arise frequently in the theoretical study of optimization.
    此外，在优化理论研究中，拉格朗日函数本身及其衍生的几个函数经常出现。

23. In this light, reasoning about the single object $L$ rather than multiple conditions makes it easier to see the connection between high-level ideas. 
    在这个意义上，关于单个对象$L$的推理，而不是多个条件，使我们更容易看到高级思想之间的联系。

24. Not to mention, it's quicker to write down on a blackboard.
    更不用说，这在黑板上写下来更快。

25. In either case, whatever your future relationship with constrained optimization might be, it is good to be able to think about the Lagrangian itself and what it does.
    无论哪种情况，无论你与约束优化的未来关系如何，能够思考拉格朗日函数本身及其作用都是有益的。

26. The examples above illustrate how it works, and hopefully help to drive home the point that $\nabla L = 0$ encapsulates both $\nabla f = \lambda \nabla g$ and $g(x,y) =c$ in a single equation.
    上面的例子说明了它是如何工作的，希望有助于深入理解$\nabla L = 0$在一个等式中包含了$\nabla f = \lambda \nabla g$和$g(x,y) =c$的观点。