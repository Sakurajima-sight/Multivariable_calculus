
--- pic\Interpretation of Lagrange multipliers.pdf_00.png ---

1. Interpretation of Lagrange multipliers
   拉格朗日乘数的解释

2. Lagrange multipliers are more than mere ghost variables that help to solve constrained optimization problems.
   拉格朗日乘数不仅仅是帮助解决约束优化问题的幽灵变量。

1. Background
背景

2. Introduction to Lagrange multipliers
拉格朗日乘数法介绍

3. Gradient
梯度

4. Lagrange multiplier technique, quick recap
拉格朗日乘数技术，快速回顾

1. When you want to maximize (or minimize) a multivariable function $f(x, y, \ldots)$ subject to the constraint that another multivariable function equals a constant, $g(x, y, \ldots) = c$, follow these steps:
当你想要最大化（或最小化）一个多变量函数 $f(x, y, \ldots)$，并且受到另一个多变量函数等于常数的约束，即 $g(x, y, \ldots) = c$，请按照以下步骤操作：

6. Step 1: Introduce a new variable $\lambda$, and define a new function $L$ as follows:
    $L(x,y,.., \lambda) = f(x,y,..) - \lambda(g(x,y,..)-c)$
    步骤1：引入一个新变量$\lambda$，并定义一个新函数$L$，如下所示：
    $L(x,y,.., \lambda) = f(x,y,..) - \lambda(g(x,y,..)-c)$

7.  This function $L$ is called the "Lagrangian", and the new variable $\lambda$ is referred to as a "Lagrange multiplier"
    这个函数$L$被称为“拉格朗日量”，新变量$\lambda$被称为“拉格朗日乘数”

8.  Step 2: Set the gradient of $L$ equal to the zero vector. 
    步骤2：将函数$L$的梯度设为零向量。


--- pic\Interpretation of Lagrange multipliers.pdf_01.png ---

1. In other words, find the critical points of $L$. 
    换句话说，找到$L$的关键点。

10. Step 3 : Consider each solution, which will look something like ($x_0$，$y_0$，…，$\lambda_0$ ) .
步骤3：考虑每个解，它们看起来应该像这样（$x_0$，$y_0$，…，$\lambda_0$）。

1. Plug each one into $f$. 
将每个解代入$f$。

1. Or rather, first remove the λ 0 component, then plug it into f , since f does not have λ as an input.
或者，首先移除$\lambda_0$组件，然后将其代入$f$，因为$f$的输入中没有$\lambda$。

1. Whichever one gives the greatest (or smallest) value is the maximum (or minimum) point you are seeking.
无论哪一个给出的值最大（或最小），那就是你正在寻找的最大（或最小）点。

1. Budgetary constraints, revisited
再次讨论预算约束

6.  The last article covering examples of the Lagrange multiplier technique included the following problem.
    最后一篇涵盖了拉格朗日乘数技术例子的文章包含了以下问题。

7.  Problem: Suppose you are running a factory, producing some sort of widget that requires steel as a raw material.
    问题：假设你在运营一个工厂，生产某种需要钢作为原料的部件。

8.  Your costs are predominantly human labor, which is $20 per hour for your workers, and the steel itself, which runs for $170 per ton.
    你的成本主要是人工，工人每小时20美元，而钢本身每吨170美元。

9.  Suppose your revenue $R$ is loosely modeled by the equation
    假设你的收入$R$被大致模型化为等式

2. Where $h$ represents hours of labor, $s$ represents tons of steel
其中，$h$ 代表劳动小时数，$s$ 代表钢的吨数

10. If your budget is $20,000, what is the maximum possible revenue?
    如果你的预算是$20,000，那么最大可能的收入是多少？

3. You can get a feel for this problem using the following interactive diagram, which let's you see which values of $(h, s)$ yield a given revenue (blue curve) and which values satisfy the constraint (red line).
你可以通过以下的交互式图表来理解这个问题，它让你看到哪些 $(h, s)$ 的值会产生给定的收入（蓝色曲线），以及哪些值满足约束（红线）。

--- pic\Interpretation of Lagrange multipliers.pdf_02.png ---

17. The full details of the solution can be found in the last article.
    解决方案的全部细节可以在最后一篇文章中找到。

18. For our purposes here, you just need to know what happens in principle as we follow the steps of the Lagrange multiplier technique.
    在这里，你只需要知道当我们按照拉格朗日乘数技术的步骤进行时，原则上会发生什么。

19. We start by writing the Lagrangian $L(h, s, \lambda)$ based on the function $R(h, s)$ and the constraint $20h + 170s = 20,000$.
    我们首先根据函数$R(h, s)$和约束条件$20h + 170s = 20,000$来写出拉格朗日函数$L(h, s, \lambda)$。

20. Then we find the critical points of $L$, meaning the solutions to $\nabla L(h, s,\lambda) = 0$.
    然后我们找到$L$的临界点，也就是满足$\nabla L(h, s,\lambda) = 0$的解。

21. There might be several solutions $(h, s, \lambda)$ to this equation, 
    这个方程可能有几个解$(h, s, \lambda)$，

1. so for each one you plug in the $h$ and $s$ components to the revenue function $R(h, s)$ to see which one actually corresponds with the maximum.
所以对于每一个解，你把$h$和$s$代入收入函数$R(h, s)$来看哪个真正对应最大值。


22. It's common to write this maximizing critical point as $(h^*, s^*, \lambda^*)$, using asterisk superscripts to indicate that this is a solution.
    我们通常把这个最大化的临界点写为$(h^*, s^*, \lambda^*)$，使用星号上标来表示这是一个解。

23. This means $h^*$ and $s^*$ represent the hours of labor and tons of steel you should allocate to maximize revenue subject to your budget.
    这意味着$h^*$和$s^*$代表了你应该分配的劳动小时数和钢的吨数，以在预算约束下最大化收入。

24. But how can we interpret the Lagrange multiplier $\lambda^*$ that comes with these maximizing values?
    但是我们如何解释随这些最大值而来的拉格朗日乘数$\lambda^*$呢？

1. This is the core question of the article.
这是本文的核心问题。

--- pic\Interpretation of Lagrange multi pliers.pdf_03.png ---

1. It turns out that $\lambda^*$ tells us how much more money we can make by changing our budget.
    结果$\lambda^*$告诉我们我们可以通过改变预算来赚取多少更多的钱。

26. Let's get a feel for what it means to change the budget.
    让我们感受一下改变预算意味着什么。

1. The following tool is similar to the one above, but now the red line representing which points ( h , s ) satisfy the budget constraint will shift as you let the budget vary around $20,000. 
以下的工具与上面的类似，但现在，表示满足预算约束的点 $(h, s)$ 的红线会随着你让预算在 $20,000 左右变动而移动。

1. This budget is represented with the variable b.
这个预算用变量 $b$ 来表示。

27. For each value of the budget $b$, try to maximize $R$ while ensuring that the curves still touch each other.
    对于预算$b$的每一个值，尝试最大化$R$，同时确保曲线仍然相互接触。

28. Notice that the maximum $R$-value you can achieve changes as $b$ changes.
    注意到你可以达到的最大$R$值随着$b$的变化而变化。

29. We are interested in studying the specifics of that change.
    我们对研究这种变化的细节感兴趣。

30. Let $M^*$ represent the maximum revenue you achieve.
    让$M^*$表示你达到的最大收入。

31. In the next interactive diagram, the only variable you can change is $b$, and you can see how the value of $M^*$ depends on $b$.
    在下一个交互式图表中，你可以改变的唯一变量是$b$，你可以看到$M^*$的值如何依赖于$b$。

--- pic\Interpretation of Lagrange multipliers.pdf_04.png ---

1. In other words, this maximum revenue $M^{* }$ is a function of the budget $b$, so we write It as .
    换句话说，这个最大收入$M^{* }$是预算$b$的函数，所以我们将其写为。

2. We can now express a truly wonderful fact: The Lagrange multiplier $\lambda^{* }(b)$ gives the derivative of $M^{* }$: 
    现在我们可以表达一个真正美妙的事实：拉格朗日乘数$\lambda^{* }(b)$给出了$M^{* }$的导数：

3. In terms of the interactive diagram above, this means $\lambda^{* }(b)$ tells you the rate of change of the black dot representing $M^{* }$ as you move around the green dot representing $b$.
    根据上面的交互式图表，这意味着$\lambda^{* }(b)$告诉你当你在代表$b$的绿点周围移动时，代表$M^{* }$的黑点的变化率。

4. Showing why this is true Is a bit tricky, but first, let's take a moment to interpret it.
    证明这为什么是真的有点复杂，但首先，让我们花一点时间来解释一下。

1. For example, if we found that $\lambda (b) = 2.59$, it would mean each additional dollar you spend over your budget would yield another $2.59 in revenue.
例如，如果我们发现 $\lambda (b) = 2.59$，这意味着你在预算之外每多花一美元就能带来额外的2.59美元的收入。

6.  Conversely, decreasing your budget by a dollar will cost you that much in lost revenue.
    相反，减少一美元的预算将会因为失去的收入而让你付出同样的代价。

7.  This interpretation of $\lambda^{* }$ comes up commonly enough in economics to deserve a name: "Shadow price".
    对$\lambda^{* }$的这种解释在经济学中常见到足以配得上一个名字："影子价格"。

8.  It is the money gained by loosening the constraint by a single dollar, or conversely the price of strengthening the constraint by one dollar.
    这是通过放宽一美元的约束所获得的金钱，或者反过来说，这是通过加强一美元的约束所付出的价格。

1. Generally speaking
一般来说

--- pic\Interpretation of Lagrange multipliers.pdf_05.png ---

1. Let's generalize what we just did with the budget example and see why it's true.
    让我们将我们刚刚在预算例子中所做的事情进行推广，看看为什么它是真的。

14. Spelling out the full result is actually quite a mouthful, but it should be made clear by holding the following mantra in the back of your mind: "How does the solution change as the constraint changes?
    阐述完整的结果实际上是非常冗长的，但如果你在心里牢记下面的咒语，那么它应该是清楚的："当约束变化时，解决方案如何变化？

15. We start with the usual Lagrange multiplier setup.
    我们从常用的拉格朗日乘数设置开始。

16. There is a function we want to maximize
    有一个我们想要最大化的函数

17. And a constraint
    以及一个约束条件

18. We start by writing the Lagrangian, 
    我们首先写出拉格朗日函数，

19. Let $(x^*, y^*, \lambda^*)$ be the critical point of $L$, which solves our constrained optimization problem.
    让$(x^*, y^*, \lambda^*)$成$L$为的关键点，它解决了我们的约束优化问题。

20. In other words, 
    换句话说，

21. And $(x^*, y^*)$ maximizes $f$ (subject to the constraint).
    并且$(x^*, y^*)$最大化了$f$ (受约束)。

22. When we start to think of $c$ as a variable, we must account for the fact that the solution $(x^*, y^*, \lambda^*)$ changes as the constraint $c$ changes.
    当我们开始把$c$当作一个变量时，我们必须考虑到随着约束$c$的变化，解决方案$(x^*, y^*, \lambda^*)$也会变化的事实。

23. To do this, we start writing each component as a function of $c$.
    为了做到这一点，我们开始把每个组件写作为$c$的函数。

24. In other words, when the constraint equals some value c, the solution triplet to the Lagrange multiplier problem is $(x^*(c), y^*(c), \lambda^*(c))$.
    换句话说，当约束等于某个值c时，拉格朗日乘数问题的解组是$(x^*(c), y^*(c), \lambda^*(c))$。

1. We now let $M^*(c)$ represent the (constrained) maximum value of $f$ as a function of $c$, which can be written in terms of $f$, $x^*(c)$ and $y^*(c)$ as follows:
我们现在让 $M^*(c)$ 表示作为 $c$ 的函数的 $f$ 的（受限）最大值，可以用 $f$，$x^*(c)$ 和 $y^*(c)$ 表示如下：

2. The core result we wish to show is that
我们希望展示的核心结果是

--- pic\Interpretation of Lagrange multipliers.pdf_06.png ---

1.  This says that the Lagrange multiplier $\lambda^*$ gives the rate of change of the solution to the constrained maximization problem as the constraint varies.
    这表示拉格朗日乘数$\lambda^*$给出了约束最大化问题的解随着约束的变化而变化的速率。

2.  Want to outsmart your teacher?
    想要比你的老师更聪明吗？

3.  Proving this result could be an algebraic nightmare, since there is no explicit formula for the functions $x^*(c), y^*(c), \lambda^*(c)$ or $M^*(c)$.
    证明这个结果可能是一个代数噩梦，因为没有显式公式可以表示函数$x^*(c), y^*(c), \lambda^*(c)$或$M^*(c)$。

29. This means you would have to start with the defining property of $x^*$, $y^*$, and $\lambda^*$, namely that $\nabla f(x^*, y^*, \lambda^*) = 0$, and reason your way towards $\frac{dM^*}{dc}$”.
    这意味着你必须从$x^*$, $y^*$ 和 $\lambda^*$的定义属性开始，即$\nabla f(x^*, y^*, \lambda^*) = 0$，并推理出$\frac{dM^*}{dc}$”。

30. This is not at all straight forward (try it!)
    这一点都不直接（试试看！）

31. There is a fun story, in which a professor was asked what the harshest truth he ever learned from a student was.
    有一个有趣的故事，其中一个教授被问到他从学生那里学到的最残酷的真理是什么。

32. He recalled a class he taught when he went through a long and algebraically heavy proof, only to be shown by a student that there is a much simpler approach.
    他回忆起他教过的一个课程，当时他经历了一个长且代数负担重的证明，结果被一个学生告知有一个更简单的方法。

33. The lesson, he said, was that he was not as smart as he thought he was.
    他说，他从中学到的教训是，他并不像他以为的那么聪明。

34. The result he was talking about just so happens to be what we are now trying to prove.
    他谈论的结果恰好就是我们现在试图证明的结果。

35. Although the student's approach is not quite so simple as the story makes it out to be, it is still a clean way to view the problem.
    虽然学生的方法并不像故事中那样简单，但它仍然是看待问题的一个清晰的方式。

36. More importantly, it is easier to remember than other proofs, so I'll spell it out in full here.
    更重要的是，它比其他的证明更容易记住，所以我会在这里详细地阐述。

37. As happens so often in math, a little insight can save us from excessive algebra.
    正如在数学中经常发生的那样，一点洞察力可以使我们免于过多的代数计算。

38. The underlying insight is that evaluating the Lagrangian itself at a solution $(x^*(c), y^*(c), \lambda^*(c))$ will give the maximum value $M^*$.
    基本的洞察力是，将拉格朗日函数本身在解$(x^*(c), y^*(c), \lambda^*(c))$处进行评估将给出最大值$M^*$。

39. This is because the "$g(x, y) - c$" term in the Lagrangian goes to zero (since a solution must satisfy the constraint), so we have .
    这是因为拉格朗日函数中的"$g(x, y) - c$"项为零（因为解必须满足约束），所以我们有。

40. Given that we want to find $\frac{dM^*}{dc}$, this suggests that we should find a way to treat $L$ as a function of $c$.
    考虑到我们想要找到$\frac{dM^*}{dc}$，这表明我们应该找到一种方式将$L$视为$c$的函数。

41. Then we might be able to relate the derivative we want to a derivative of $L$ with respect to $c$.
    然后我们可能能够将我们想要的导数与$L$对$c$的导数联系起来。

1. The insight
洞察

--- pic\Interpretation of Lagrange multipliers.pdf_07.png ---

1. The followthrough
   后续处理

2. Start by treating $L$ as a function of four variable instead of three, since $c$ is now modeled as a changing value:
   由于现在将$c$视为一个变化的值，所以首先将$L$视为四个变量的函数，而不是三个变量的函数：
   
3. Reflection question: When $L$ is written as a four-variable function like this, what is $\frac{\partial L}{\partial c}$?
   反思问题：当$L$以这样的四变量函数形式写出时，$\frac{\partial L}{\partial c}$是什么？

1. This partial derivative is promising, since our goal is to show that  $\frac{dM^*}{dc} = \lambda^*$ , and we know that $M^* = L$ at solutions. 
这个偏导数很有希望，因为我们的目标是证明  $\frac{dM^*}{dc} = \lambda^*$，我们知道在解决方案中 $M^* = L$。

4.  However, we still have work to do.
    但是，我们还有工作要做。

5.  To encode the fact that we only care about the value of $L$ at a solutions $(x^*(c), y^*(c), \lambda^*(c))$ for a given value of $c$, we replace $x$, $y$, and $\lambda$ with $x^*$, $y^*$, and $\lambda^*$.
    为了表达我们只关心在给定$c$值的解决方案$(x^*(c), y^*(c), \lambda^*(c))$处$L$的值，我们将$x$, $y$和$\lambda$替换为$x^*$, $y^*$ 和 $\lambda^*$。

6.  These are functions of $c$ which correspond to the solution of the Lagrangian problem for a given choice of the "constant" $c$.
    这些是$c$的函数，对应于给定"常数"$c$的选择的拉格朗日问题的解。

7.  This lets us write $M^*$ as a function of $c$ as follows:
    这让我们可以将$M^*$写为以下形式的$c$的函数：

10. Even though this expression has only one variable, $c$, there is a four-variable function $L$ as an intermediary.
    尽管这个表达式只有一个变量$c$，但是有一个四变量函数$L$作为中介。

2. Therefore, to take its (ordinary) derivative with respect to $c$ , we use the multivariable chain rule :
因此，为了对 $c$ 取其（普通）导数，我们使用多元链式法则：

--- pic\Interpretation of Lagrange multipliers.pdf_08.png ---

1. Note, each partial derivative in the expression above should be evaluated at $(x^*(c), y^*(c), \lambda^*(c), c)$, but writing that would make the expression more messy than it already is.
    注意，上述表达式中的每个偏导数都应在$(x^*(c), y^*(c), \lambda^*(c), c)$处求值，但是写出这些会使表达式比现在更混乱。

18. This might seem like a lot, but remember where the terms $x^*$, $y^*$, and $\lambda^*$ each came from.
    这可能看起来很多，但是记住$x^*$, $y^*$ 和 $\lambda^*$各自来自哪里。

19. Each partial derivative $\frac{\partial L}{\partial x}$ $\frac{\partial L}{\partial y}$ and $\frac{\partial L}{\partial \lambda}$ is zero when evaluated at $(x^*(c), y^*(c), \lambda^*(c))$.
    在$(x^*(c), y^*(c), \lambda^*(c))$处评估时，每个偏导数$\frac{\partial L}{\partial x}$、$\frac{\partial L}{\partial y}$和$\frac{\partial L}{\partial \lambda}$都是零。

20. That's how a solution $(x^*, y^*, \lambda^*)$ is defined!
    这就是解$(x^*, y^*, \lambda^*)$的定义方式！

21. This means the first three terms go to zero.
    这意味着前三项都趋于零。

22. Moreover, since $\frac{dc}{dc} = 1$, the entire expression simplifies to 
    此外，由于$\frac{dc}{dc} = 1$，整个表达式简化为

23. It's important to notice that the reason for this simplification relies on the special properties of solution points $(x^*, y^*, \lambda^*)$.
    重要的是要注意，这种简化的原因依赖于解点$(x^*, y^*, \lambda^*)$的特殊性质。

24. Otherwise, working out the full derivative based on the multivariable chain rule could have been a nightmare!
 否则，基于多变量链规则计算出全导数可能会是一场噩梦！

25. For the sake of notational cleanliness, we left out the inputs to these derivatives, but let's write them in.
    为了符号的清晰，我们省略了这些导数的输入，但让我们写入它们。

26. Since we saw in the reflection question above that $\frac{\partial L}{\partial c}=\lambda$, this means 
    由于我们在上面的反思问题中看到$\frac{\partial L}{\partial c}=\lambda$，这意味着

27. Done!
    完成！

--- pic\Interpretation of Lagrange multipliers.pdf_09.png ---

28. The anecdote about professor and student originally come from this Quora post.
    关于教授和学生的轶事最初来自这个Quora帖子。