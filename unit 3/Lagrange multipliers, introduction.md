
--- pic\Lagrange multipliers, introduction.pdf_00.png ---

1. Lagrange multipliers, introduction
    拉格朗日乘数法介绍

2. The "Lagrange multipliers" technique is a way to solve constrained optimization problems. Super useful!
    “拉格朗日乘数法”是一种解决约束优化问题的方法。超级有用！

1. Background
背景

2. Contour maps
等高线图

3. Gradient
梯度

4. Local maxima and minima
局部最大值和最小值

3. What we're building to:
    我们正在构建的：

5. The Lagrange multiplier technique lets you find the maximum or minimum of a multivariable function $f ( x , y , … )$ when there is some constraint on the input values you are allowed to use.
拉格朗日乘数法允许你在输入值受到某些约束时，找到多元函数$f ( x , y , … )$的最大值或最小值。

1. This technique only applies to constraints that look something like this:
这种技术只适用于约束看起来像这样的情况：

1. Here, $g$ is another multivariable function with the same input space as $f$, and $c$ is some constant.
    在这里，$g$是另一个与$f$具有相同输入空间的多元函数，而$c$是某个常数。

2. For example, if the input space is two-dimensional, the graph of $f$ with the line representing $g ( x , y ) = c$ projected onto it might look something like this:
例如，如果输入空间是二维的，那么表示$g ( x , y ) = c$的线投影到$f$的图上可能看起来像这样：

--- pic\Lagrange multipliers, introduction.pdf_01.png ---

1. The goal is to find the highest point on that red line. 
    目标是找到那条红线上的最高点。

1. The core idea is to look for points where the contour lines of $f$ and $g$ are tangent to each other. 
核心思想是寻找$f$和$g$的等高线互相切的点。

1. This is the same as finding points where the gradient vectors of $f$ and $g$ are parallel to each other.
这与找到$f$和$g$的梯度向量彼此平行的点是一样的。

7. The entire process can be boiled down into setting the gradient of a certain function, called the Lagrangian, equal to the zero vector. 
    整个过程可以归结为让某个函数（称为拉格朗日函数）的梯度等于零向量。

8. Step 1: Introduce a new variable $\lambda$, and define a new function $L$ as follows:
    $L(x,y,.., \lambda) = f(x,y,..) - \lambda(g(x,y,..)-c)$
    步骤1：引入一个新变量$\lambda$，并定义一个新函数$L$，如下所示：
    $L(x,y,.., \lambda) = f(x,y,..) - \lambda(g(x,y,..)-c)$

9. This function $L$ is called the "Lagrangian", and the new variable $\lambda$ is referred to as a "Lagrange multiplier".
    这个函数$L$被称为“拉格朗日函数”，新变量$\lambda$被称为“拉格朗日乘数”。

10. Step 2: Set the gradient of $L$ equal to the zero vector. 
    $\nabla L(x,y,.., \lambda) = 0$
    步骤2：将$L$的梯度设为零向量。 
    $\nabla L(x,y,.., \lambda) = 0$

11. In other words, find the critical points of $L$. 
    换句话说，找到$L$的临界点。

12. Step 3: Consider each solution, which will look something like $(x_0, y_0,...,\lambda_0)$. 
    步骤3：考虑每个解，这些解看起来像$(x_0, y_0,...,\lambda_0)$。

1. Plug each one into $f$. 
将每个解插入到$f$中。

1. Or rather, first remove the $\lambda_0$ component, then plug it into $f$, since $f$ does not have $\lambda$ as an input.
或者，先去掉$\lambda_0$成分，然后插入$f$，因为$f$的输入中没有$\lambda$。

1.  Whichever one gives the greatest (or smallest) value is the maximum (or minimum) point your are seeking.
无论哪个给出的值最大（或最小），就是你要寻找的最大（或最小）点。

1. Motivating example
激励示例

2. Suppose you want to maximize this function:
假设你想要最大化这个函数：

--- pic\Lagrange multipliers, introduction.pdf_02.png ---

1. But let's also say you limited yourself to inputs $(x, y)$ which satisfy the following equation:
但是，我们也可以说你限制了自己的输入 $(x, y)$，它们满足以下等式：

--- pic\Lagrange multipliers, introduction.pdf_03.png ---

1. All points $(x, y)$ satisfying $x^2 + y^2 = 1$ form a unit circle. 
    所有满足 $x^2 + y^2 = 1$ 的点 $(x, y)$ 形成一个单位圆。

14. In other words, for which point $(x, y)$ on the unit circle is the value $2x + y$ biggest? 
    换句话说，对于单位圆上的哪个点 $(x, y)$，$2x + y$ 的值最大？

15. This is what's known as a constrained optimization problem. 
    这就是所谓的约束优化问题。

1. The restriction to points where $x^2 + y^2 = 1$ is called a "constraint", and $f ( x , y ) = 2 x + y$ is the function that needs to be optimized.
将满足 $x^2 + y^2 = 1$ 的点的限制称为“约束”，而 $f ( x , y ) = 2 x + y$ 是需要优化的函数。

16. The restriction to points where $x^2 + y^2 = 1$ forms a constraint. 
    $x^2 + y^2 = 1$ 形成的限制条件。

17. Here's one way to visualize this: First draw the graph of $f(x, y)$, which looks like a slanted plane since $f$ is linear. 
    这里有一种可视化的方法：首先画出$f(x, y)$的图像，因为$f$是线性的，所以它看起来像一个倾斜的平面。

18. Next, project the unit circle $x^2 + y^2 = 1$ onto the graph. 
    接下来，将单位圆$x^2 + y^2 = 1$投影到这个图上。

19. The maximum we are seeking corresponds with the highest point of this projected circle on the graph. 
    我们正在寻找的最大值对应于图上投影圆的最高点。

2. More general form
更一般的形式

20. In general, constrained optimization problems involve maximizing/minimizing a multivariable function whose input has any number of dimensions: $f(x,y, z,..)$. 
    一般来说，约束优化问题涉及最大化/最小化一个多变量函数，其输入可以有任意数量的维度：$f(x,y, z,..)$。

21. Its output will always be one-dimensional, though, since there's not a clear notion of "maximum" with vector-valued outputs. 
    不过，它的输出总是一维的，因为对于向量值的输出，没有一个清晰的“最大值”的概念。

3. The type of constraints that the Lagrange multiplier technique applies to must take the form of some other multivariable function $g ( x , y , z , … )$ being set equal to a constant $c$.
拉格朗日乘数技术适用的约束类型必须采取某种其他多变量函数 $g ( x , y , z , … )$ 等于常数 $c$ 的形式。

--- pic\Lagrange multipliers, introduction.pdf_04.png ---

1. Since this is meant to be a constraint on the input of $f$, the number of dimensions in the input of $g$ is the same as that of $f$. 
    由于这是对$f$输入的约束，所以$g$的输入维数与$f$的相同。

24. For example, the example outlined above fits this general form as follows:
    $f(x, y) = 2x + y$
    $g(x, y) = x^2 + y^2$
    $c = 1$
    例如，上述的例子符合这种一般形式，如下：
    $f(x, y) = 2x + y$
    $g(x, y) = x^2 + y^2$
    $c = 1$

25. There is a generalization of the Lagrange multiplier technique that applies to situations with multiple constraints on the input. 
    对于输入有多个约束的情况，拉格朗日乘数法有一种泛化形式。

26. However, in this article, I will only talk about the single-constraint case.
    然而，在这篇文章中，我只会谈到单一约束的情况。

1. Using contour maps
使用等高线图

27. Reasoning about this problem becomes easier if we visualize $f$ not with a graph, but with its contour lines. 
    如果我们不用图形而用等高线来可视化$f$，那么理解这个问题就会变得更容易。

28. As a reminder, a contour line of $f(x, y)$ is the set of all points where $f(x,y) = k$ for some constant $k$.
    提醒一下，$f(x, y)$的等高线是所有$f(x,y) = k$点的集合，其中$k$是某个常数。

29. The following interactive tool shows how this line (drawn in blue) changes as the constant  $k$ changes.  
    下面的交互工具显示了当常数$k$改变时，这条线（用蓝色画出）是如何改变的。

1. The circle $g(x, y) = 1$ is also shown (in red).
圆$g(x, y) = 1$也显示出来了（用红色）。

1. Try to make $k$ as big/small as possible while still allowing contour line of $f$ to intersect the circle.
试着使$k$尽可能大/小，同时仍然允许$f$的等高线与圆相交。


--- pic\Lagrange multipliers, introduction.pdf_05.png ---

1. Concept check: What does it mean if for a particular value of $k$, the blue line representing $f(x,y) = k$ does not intersect the red circle representing $g(x,y) =1$? 
    概念检查：如果对于特定的$k$值，代表$f(x,y) = k$的蓝线没有与代表$g(x,y) =1$的红圈相交，这意味着什么？

1. There are no values of $x$ and $y$ satisfying both $2x+ y= k$ and $x^2 + y^2 = 1$.
没有 $x$ 和 $y$ 的值同时满足 $2x+ y= k$ 和 $x^2 + y^2 = 1$ 这两个等式。

3. Notice, the circle where $g(x,y) =1$ can be thought of as a particular contour line of the function $g$. 
    注意，$g(x,y) =1$的这个圆可以被认为是函数$g$的一个特定等高线。

4. So with that, here's the clever way to think about constrained optimization problems:
    所以有了这个，这就是巧妙地思考约束优化问题的方式：

5. Key observation: The maximum and minimum values of $f$, subject to the constraint $g(x,y) =1$, correspond with contour lines of $f$ that are tangent to the contour representing $g(x,y) =1$.
    关键观察：受到约束$g(x,y) =1$的$f$的最大值和最小值，对应于与表示$g(x,y) =1$的等高线相切的$f$的等高线。

--- pic\Lagrange multipliers, introduction.pdf_06.png ---

1. If $f$ were a different function, its contours might not always be straight lines.
如果 $f$ 是一个不同的函数，其等高线可能并不总是直线。

1. This is unique to our example since $f$ is linear.
    这是我们的示例的独特之处，因为$f$是线性的。

2. For example, take a look at this function: 
    例如，看一下这个函数：

3.  Its contour lines look like 
    它的等高线看起来像这样：

4.  That said, the key observation still holds, and is worth repeating: When $k$ is a maximum or minimum of $f$ subject to the constraint, the contour line for $f(x,y) = k$ will be tangent to contour representing $g(x,y) =1$.
    也就是说，关键的观察仍然有效，并值得重复：当$k$是在约束下的$f$的最大值或最小值时，$f(x,y) = k$的等高线将会与表示$g(x,y) =1$的等高线相切。

5. Where the gradient comes into play
在哪里梯度起作用


--- pic\Lagrange multipliers, introduction.pdf_07.png ---

12. How do you put the idea of two contour lines being tangent into a formula you can solve?
    你如何将两条等高线相切的想法放入你可以解的公式中？

13. To answer this, we turn to our loyal friend the gradient. 
    为了回答这个问题，我们转向我们忠诚的朋友梯度。

14. There are many ways to interpret $\nabla f$: The direction of steepest ascent, a tool for computing directional derivatives, etc.
    有许多方式可以解释$\nabla f$：最陡峭的上升方向，计算方向导数的工具等。

15. But for our purposes here, the property we care about is that the gradient of $f$ evaluated at a point (zo, yo) always gives a vector perpendicular to the contour line passing through that point.
    但对于我们在这里的目的，我们关心的属性是，函数f在点(zo, yo)处的梯度总是给出一个与通过该点的等高线垂直的向量。

16. This means when the contour lines of two functions $f$ and g are tangent, their gradient vectors are parallel.
    这意味着当两个函数f和g的等高线相切时，他们的梯度向量是平行的。

17. Here's what that might look like for arbitrary functions $f$ and g:
    这可能是任

意函数f和g的样子：

18. The fact that contour lines are tangent tells us nothing about the magnitude of each of these gradient vectors, but that's okay.
    等高线相切的事实并没有告诉我们这些梯度向量的大小，但这没关系。

19. When two vectors point in the same direction, it means we can multiply one by some constant to get the other.
    当两个向量指向同一个方向时，意味着我们可以将其中一个乘以某个常数来得到另一个。

20. Specifically, let (xo, yo) represent a particular point where the contour lines of $f$ and g are tangent (writing zp and yo with a 0 subscripts just indicates that we are considering constant values, and hence a specific point).
    具体来说，让(xo, yo)表示f和g的等高线相切的特定点（写成zp和yo带有0下标只是表示我们正在考虑恒定的值，因此是特定的点）。

21. Since this tangency means their gradient vectors align, here's what you might write down:
    由于这个相切意味着他们的梯度向量对齐，这是你可能会写下的：

22. $\nabla $f$ (x0, yo) = \lambda_0 \nabla g(x0, Yo)$
    $\nabla $f$ (x0, yo) = \lambda_0 \nabla g(x0, Yo)$

23. Here, $\lambda_p$ represents some constant.
    这里，$\lambda_p$代表一些常数。

24. Some authors use a negative constant, — Ng, but I personally prefer a positive constant, as it gives a cleaner interpretation of $\lambda_y$ down the road.
    一些作者使用负常数，— Ng，但我个人更喜欢正常数，因为它为后面的$\lambda_y$提供了更清晰的解释。

25. Let's see what this looks like in our example where f(z, y) = 2% + y and g(x,y) = x²
    让我们看看在我们的例子中这个公式是什么样的，其中f(z, y) = 2% + y 和 g(x,y) = x²

--- pic\Lagrange multipliers, introduction.pdf_08.png ---

26. $\nabla f(z,y) = <$, $>$
    $\nabla f(z,y) = <$, $>$

27. and the gradient of g Is $\nabla g(z,y) = <$, $>$
    而g的梯度是 $\nabla g(z,y) = <$, $>$

28. Solving the problem in the specific case
    解决特定情况的问题

29. To sum up where we are so far, we are looking for input points (x0, y0) with the following properties:
    总结到目前为止，我们正在寻找具有以下属性的输入点(x0, y0)：

30. g(x0, y0) = 1, which for our example means x² + y² = 1
    g(x0, y0) = 1，对于我们的示例意味着 x² + y² = 1

31. $\nabla f(x0, y0) = \lambda_0 \nabla g(x0, y0)$ for some constant $\lambda_g$, which for our example means 2= 2$\lambda_g x0$ 1= 2$x0 y0$
    对于一些常数$\lambda_g$，我们有 $\nabla f(x0, y0) = \lambda_0 \nabla g(x0, y0)$，在我们的示例中意味着 2= 2$\lambda_g x0$ 1= 2$x0 y0$

32. There are 3 equations and 3 unknowns, so this is a perfectly solvable situation.
    有3个等式和3个未知数，所以这是一个完全可解的情况。

--- pic\Lagrange multipliers, introduction.pdf_09.png ---

1. The approach will be to first solve for Ao, then use the solution to find zp and Yo-
   我们首先解出Ao，然后使用解出的Ao找出zp和Yo。

2. Using the last two equations above, write x9 and yo in terms of Ao. An@o = To = 1 = 2A0y0 > Yo = | = £4A0Y0 Y= 3y.
   使用上面的最后两个方程，将x9和yo用Ao表示。$An@o = To = 1 = 2A_0y_0 > Yo = | = £4A_0Y_0 Y= 3y$。

3. Now to bring in the third equation, plug these results into the equation t+ Yo = 1. 
   现在引入第三个方程，将这些结果代入方程$t+ Yo = 1$。

4. Brae! To get Ay out of the denominators, we multiply everything by 4. Baa A 0 4/5 2 ~ 0
   为了从分母中消去Ay，我们把所有的都乘以4。$Baa A 0 4/5 2 ~ 0$。

5. Using the expressions for zo and yo in terms of Ap that we found above, these two solutions correspond with the pairs ooo (Sea) Ga) « G2
   使用我们在上面找到的表示zo和yo的Ap的表达式，这两个解对应于一对解ooo (Sea) Ga) « G2。

6. We can see which of these is a maximum point and which Is a minimum point by plugging these solutions into f(z, y) and seeing which is bigger.
   我们可以把这些解代入f(z, y)中，看看哪个更大，从而看出哪个是最大点，哪个是最小点。

--- pic\Lagrange multipliers, introduction.pdf_10.png ---

7. J/5 <— Maximum
   $J/5$是最大值。

8. = —/5 <— Minimum
   = $-J/5$是最小值。

9. The Lagrangian function
   拉格朗日函数。

10. Joseph Louis Lagrange, looking peaceful, content, and sleepy, all at the same time.
    Joseph Louis Lagrange，看起来平静、满足和困倦，所有这些感觉同时出现。

--- pic\Lagrange multipliers, introduction.pdf_11.png ---

11. In the 1700's, our buddy Joseph Louis Lagrange studied constrained optimization problems of this kind, and he found a clever way to express all of our conditions into a single equation.
    在1700年代，我们的朋友Joseph Louis Lagrange研究了这类受约束的优化问题，他找到了一种巧妙的方法，将我们所有的条件表达为一个单一的等式。

12. You can write these conditions generally by saying we are looking for constants xo, yo and Xo that satisfy the following conditions:
    你可以一般地写出这些条件，说我们正在寻找满足以下条件的常数xo, yo和Xo：

13. The constraint: 9(Xo, Yo) = C
    约束：$9(Xo, Yo) = C$

14. The tangency condition: V $f$ (0, Yo) = AoV9(Zo, Yo):
    切线条件：$V $f$ (0, Yo) = AoV9(Zo, Yo)$：

15. This can be broken into its components as follows: © fr(£0, Yo) = AoGz(Zo, Yo) ° fy (0, yo) — roGy (Lo, Yo)
    这可以被分解为以下组成部分：© $fr(£0, Yo) = AoGz(Zo, Yo)$ ° $fy (0, yo) — roGy (Lo, Yo)$

16. Lagrange wrote down a special new function which takes in all the same input variables as $f$ and g, along with the new kid in town A, thought of now as a variable rather than a constant.
    Lagrange写下了一个特殊的新函数，它接收与f和g相同的所有输入变量，以及新出现的变量A，现在被视为变量而不是常数。

17. L(x, y; X) — f(x,y) - A(g(z, y) - Cc)


    $L(x, y; X) = f(x,y) - A(g(z, y) - C)$

18. For example, consider our example above. Here's how this new function would look: L(x,y,A) = 2x2 +y-— Xa?
    例如，考虑我们上面的例子。新函数看起来是这样的：$L(x,y,A) = 2x^2 + y - Aa?$

--- pic\Lagrange multipliers, introduction.pdf_12.png ---

19. So we can translate the condition g(z, y) = cas Ly(z,y, X) — —g(z, y) +c=0
    所以我们可以将条件$g(z, y) = c$转化为$Ly(z,y, X) = -g(z, y) +c=0$

20. What's more, look at what we get when we set one of the other partial derivatives equal to 0: L,(xz,y,A) = 0
    更重要的是，当我们把其中一个偏导数设为0时，我们会得到什么：$L,(xz,y,A) = 0$

21. © (F(@,u) — Maley) ~¢)) = 0 fr(x, y) An (x, y) = 0 fr(a, y)= AGa (z, y)
    © $(F(@,u) — Maley) ~¢)) = 0, fr(x, y) An (x, y) = 0, fr(a, y)= AGa (z, y)$

22. That just so happens to be another one of our conditions! Almost identically, the condition L,(z, y, A) = 0 unravels to become fy(2,y) = Agy(z,y)
    这正好是我们的另一个条件！几乎相同，条件$L,(z, y, A) = 0$变为$fy(2,y) = Agy(z,y)$

23. Together, these conditions are the same as saying. Vi (x,y) = AV9(z,y)
    综合来看，这些条件就相当于说$Vi (x,y) = AV9(z,y)$。

24. Therefore, the three conditions we need to solve to find z, y and A come down to the various partial derivatives of £ being equal to 0.
    因此，我们需要解决的三个条件以找出z, y和A的各种偏导数都等于0。

请注意，由于原文中的许多数学公式和符号可能存在格式错误或模糊的问题，所以上述翻译可能会存在一些不准确或者理解上的困难。 

--- pic\Lagrange multipliers, introduction.pdf_13.png ---

1. As a tribute to ol' Joey Lou, we call this function £ the "Lagrangian", and the new variable \ that we introduce is called a "Lagrange multiplier". 
    作为对老乔伊·卢的致敬，我们称这个函数£为“拉格朗日量”，并称我们引入的新变量\为“拉格朗日乘数”。

2. Imagine if someone added "-ian" the end of your last name and made it the name of a function everybody uses. Pretty sweet!
    想象一下，如果有人在你的姓的后面加上“-ian”，并将其做成每个人都使用的函数的名字。相当甜蜜！

3. Warning: Some authors use a convention where the sign of A is reversed: L(x, y,A) = f(z,y) + A(g(z,y) — ©)
    警告：一些作者使用一种约定，即反转A的符号：L(x, y,A) = f(z,y) + A(g(z,y) — ©)

4. This doesn't make any difference when it comes to solving the problem, but you should keep it in mind in case the course you are taking or the text you are reading follows this convention. Hide explanation]
    在解决问题时，这没有任何区别，但如果你正在学习的课程或者你正在阅读的文本遵循这个约定，你应该记住它。

5. Side note: What if the constraint isn't so constraining? There's a slight twist to this story, best illustrated with an example.
    旁注：如果约束不是那么强制呢？这个故事有一个小小的转折，最好用一个例子来说明。

--- pic\Lagrange multipliers, introduction.pdf_14.png ---

6. Subject to the constraint g(z,y) =x-—y=0
    受到约束g(z,y) =x-—y=0

7. The graph of f(z, y) = e^(-x^2+y^2) is a "bell curve", with a round bump above the point (x0, y0) = (0,0), as pictured above.
    函数f(z, y) = e^(-x^2+y^2)的图像是一个“钟形曲线”，在点(x0, y0) = (0,0)上方有一个圆形凸起，如上图所示。

8. This constraint can be pictured as a diagonal line in the zy-plane (shown in red).
    这个约束可以被想象成在zy平面上的一条对角线(以红色显示)。

9. What makes this problem a bit silly is that the (unconstrained) maximum point (0,0) of $f$ already satisfies the constraint g(x, y) = 0, since g(0,0) =0+0=0
    使这个问题显得有点愚蠢的是，函数f的(无约束)最大点(0,0)已经满足了约束g(x, y) = 0，因为g(0,0) =0+0=0

10. It might feel like this makes things easier on us. After all, not having to worry about the constraint should be more straightforward than worrying about it, right? 
    这可能会让我们觉得事情变得更容易。毕竟，不需要担心约束应该比担心约束更直接，对吧？

11. However, if you (or more realistically a computer) were solving a given constrained optimization problem, it's not like you would first find the unconstrained maximum, check if it fits the constraint, then turn to the Lagrange multiplier technique. 
    然而，如果你(或者更实际的是一台计算机)正在解决一个给定的有约束的优化问题，你并不会首先找到无约束的最大值，检查它是否符合约束，然后转向拉格朗日乘数技术。

12. You would just start with the Lagrange multiplier approach, since it's almost never the case that the unconstrained maximum Is also the constrained maximum.
    你会直接从拉格朗日乘数法开始，因为无约束最大值也是有约束最大值的情况几乎从来没有。

13. It turns out that the Lagrange multiplier technique still works when the constrained maximum Is also an unconstrained maximum. 
    结果证明，当受限最大值也是无约束最大值时，拉格朗日乘数技术仍然有效。

14. The reason is a bit subtle since our contour-tangency argument above doesn't quite apply.
    原因有点微妙，因为我们上面的等高线切线论证并不完全适用。

--- pic\Lagrange multipliers, introduction.pdf_15.png ---

15. For example, let's play around with the contours representing e^(x+y^2) — k as k varies between 0. 
    例如，让我们变化k在0之间，玩玩代表e^(x+y^2) - k的轮廓。

16. The contour representing e^(x+y^2) — always crosses the line x — y = 0, and this contour shrinks to a point when k Is as big as it can be. 
    代表e^(x+y^2)的轮廓总是穿过线x — y = 0，当k尽可能大时，这个轮廓收缩到一个点。

17. Previously, we said the contour lines would be tangent when $f$ achieves its constrained maximum, but it feels weird to say a point is tangent to a line. 
    之前，我们说当f达到其受限最大值时，等高线会切线，但是说一个点切线是很奇怪的。

18. Why isn't this a problem then? ∇f (x0, y0) = 0
    那么为什么这不是一个问题呢？∇f (x0, y0) = 0

19. You can think of this as saying the tangent plane at a local maximum Is flat.
    你可以将此理解为，局部最大值处的切平面

是平的。

20. Flat tangent plane of $f$ at its maximum. In this case, the property ∇f (0, yo) = A∇g(Zo, Yo) still holds, because we can set A = 0.
    在f的最大值处，切平面是平的。在这种情况下，性质 ∇f (0, yo) = A∇g(Zo, Yo) 仍然成立，因为我们可以设 A = 0。

21. A funny way to think about this is to say a point is "tangent" to all lines passing through it in the same sense that the zero vector Is "proportional" to all other vectors.
    一种有趣的想法是说，一个点对所有经过它的线都是“切线”，就像零向量对所有其他向量都是“成比例”的一样。

--- pic\Lagrange multipliers, introduction.pdf_16.png ---

22. So not only does the Lagrange multiplier technique cleverly consolidate many conditions into the one equation ∇L = 0,
    所以拉格朗日乘数技术不仅巧妙地将许多条件合并到一个方程 ∇L = 0，

23. it also automatically takes into account this special edge case! 
    它还自动考虑了这个特殊的边界情况！

24. Summary:
    概述：

25. Image credit: By Nexcis (Own work) [Public domain], via Wikimedia Commons
    图像来源：通过维基媒体共享，Nexcis（自己的作品）[公共领域]

26. When you want to maximize (or minimize) a multivariable function f(z, y,..) Step 1: Introduce a new variable A, and define a new function £ as follows: L(a,y,---,A)=f(a,y,..) + A(g(a,y,---) — C)
    当你想要最大化（或最小化）一个多变量函数f(z, y,..) 步骤1：引入一个新的变量A，并定义一个新的函数£如下：L(a,y,---,A)=f(a,y,..) + A(g(a,y,---) — C)

27. This function L is called the "Lagrangian", and the new variable is referred to as a "Lagrange multiplier"
    这个函数L被称为“拉格朗日量”，新变量被称为“拉格朗日乘数”

28. Step 2: Set the gradient of £ equal to the zero vector. ∇L(a,y,..
    步骤2：将函数£的梯度设为零向量。∇L(a,y,..

--- pic\Lagrange multipliers, introduction.pdf_17.png ---

29. In other words, find the critical points of ∇L. 
    换句话说，找到∇L的关键点。

30. Step 3: Consider each solution, which will look something like (x0, y0,---, A0). Plug each one into f. 
    步骤3：考虑每个解，它会看起来像(x0, y0,---, A0)。将每个解代入f。

31. Or rather, first remove the A0 component, then plug it into f, since $f$ does not have X as an input. 
    或者，首先去掉A0成分，然后代入f，因为f没有X作为输入。

32. Whichever one gives the greatest (or smallest) value is the maximum (or minimum) point you are seeking.
    哪个给出的值最大(或最小)，就是你要找的最大(或最小)点。
