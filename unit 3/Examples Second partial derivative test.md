
--- pic\Examples Second partial derivative test.pdf_00.png ---

1. Examples: Second partial derivative test
   例子：二阶偏导数检验

2. Practice using the second partial derivative test
   练习使用二阶偏导数检验

3. Background
   背景

4. e Second partial derivative test
   二阶偏导数检验

5. Prepare for the slog
   准备进行艰难的工作

6. I have a challenge for you. In this article, you can walk through two examples of finding maxima and minima in multivariable functions.
   我有一个挑战给你。在这篇文章中，你可以通过两个例子，找到多元函数的最大值和最小值。

7. In modern applications, most of the steps involved in solving these sorts of problems would be performed by a computer.
   在现代应用中，解决这类问题的大多数步骤都会由计算机执行。

8. However, the only way to test that you really understand how the second partial derivative test is used is to walk through it yourself, at least once.
   然而，测试你是否真正理解如何使用二阶偏导数检验的唯一方法是自己亲自操作一遍。

9. After all, you may one day need to write the program to tell a computer how to do this, which requires somewhat of an intimate knowledge of all the steps involved.
   毕竟，你可能有一天需要编写程序来告诉计算机如何做这个，这需要对所有涉及的步骤有一些深入的了解。

10. Moreover, it is a good way to become more fluent with partial derivatives.
    此外，这是提高偏导数应用流畅性的好方法。

11. So my challenge to you is this: try entering the answer to each step as you move through the article to test your own understanding.
    所以我的挑战给你是这样的：尝试在阅读文章的过程中，对每一步输入答案，来测试你自己的理解。

12. The statement of the second partial derivative test (for reference)
    二阶偏导数检验的声明（供参考）

13. Start by finding a point $(x_0, y_0)$ where both partial derivatives of $f$ are $0$.
    从找到一个点$(x_0, y_0)$开始，该点的$f$的两个偏导数都是$0$。

14. $f_{x}(x_0, y_0) = 0$
    $f_{x}(x_0, y_0) = 0$

15. $f_{y}(x_0, y_0) = 0$
    $f_{y}(x_0, y_0) = 0$

16. The second partial derivative test tells us how to determine if $(x_0, y_0)$ is a local maximum, local minimum, or saddle point.
    二阶偏导数检验告诉我们如何确定$(x_0, y_0)$是局部最大值，局部最小值还是鞍点。

--- pic\Examples Second partial derivative test.pdf_01.png ---

1. $H = f_{xx}(x_0, y_0)f_{yy}(x_0, y_0) - (f_{xy}(x_0, y_0))^2$ 
    $H = f_{xx}(x_0, y_0)f_{yy}(x_0, y_0) - (f_{xy}(x_0, y_0))^2$ 

1. where $f_{xx}$, $f_{yy}$ and $f_{xy}$ are the second partial derivatives of $f$.
其中，$f_{xx}$，$f_{yy}$ 和 $f_{xy}$ 是 $f$ 的二阶偏导数。

18. If $H < 0$, then $f$ has a neither minimum nor maximum at $(x_0, y_0)$, but instead has a saddle point.
    如果 $H < 0$，那么函数$f$在点$(x_0, y_0)$既不是最小值也不是最大值，而是一个鞍点。

2. If $H > 0$, then $f$ definitely has either a maximum or minimum at $(x_0, y_0)$, and we must look at the sign of $f_{xx}(x_0, y_0)$ to figure out which one it is.
如果 $H > 0$，那么 $f$ 在 $(x_0, y_0)$ 处肯定有一个最大值或最小值，我们必须查看 $f_{xx}(x_0, y_0)$ 的符号来确定是哪一个。

20. If $f_{xx}(x_0, y_0) > 0$, then $f$ has a local minimum.
    如果 $f_{xx}(x_0, y_0) > 0$，那么函数$f$在这里有一个局部最小值。

--- pic\Examples Second partial derivative test.pdf_02.png ---
1. If $f_{xx}(x_0, y_0) < 0$, then $f$ has a local maximum.
    如果 $f_{xx}(x_0, y_0) < 0$，那么函数$f$在这里有一个局部最大值。

--- pic\Examples Second partial derivative test.pdf_03.png ---

1. If $H = 0$, the second derivatives alone cannot tell us whether $f$ has a local minimum or maximum.
    如果 $H = 0$，仅二阶导数不能告诉我们函数$f$是否具有局部最小值或最大值。

22. Example 1: All of the stable points! 
    例1：所有的稳定点！
   
23. Problem: Find all the stable points (also called critical points) of the function and determine whether each one gives a local maximum, local minimum, or a saddle point.
    问题：找出函数的所有稳定点（也称为关键点），并确定每个点是局部最大值、局部最小值还是鞍点。

24. Step 1: Find all stable points
    步骤1：找到所有稳定点

25. The stable points are all the pairs $(x_0, y_0)$ where both partial derivatives equal $0$.
    所有的稳定点都是偏导数等于$0$的$(x_0, y_0)$对。

26. First, compute each partial derivative.
    首先，计算每个偏导数。

27. Next, find all the points $(x_0, y_0)$ where both partial derivatives are $0$, which is to say, solve the system of equations.
    接下来，找出所有偏导数都为$0$的点$(x_0, y_0)$，也就是说，解这个方程组。

28. Which of the following pairs satisfying the system of equations?
    下面哪对能满足这个方程组？

--- pic\Examples Second partial derivative test.pdf_04.png ---

1. Choose all answers that apply:
    选择所有适用的答案：

2.  Putting in our partial derivatives, the system of equations looks like .
    将我们的偏导数代入，方程组看起来像。

3.  We are lucky, because the first equation has only an $x$, and the second equation has only $y$, so solving the system in this case just means solving each problem separately.
    我们很幸运，因为第一个方程只有$x$，第二个方程只有$y$，所以在这种情况下，解这个方程组就意味着分别解决每个问题。

1. The first equation factors as $4x^3 - 8x = 0$
第一个方程式可以因式分解为 $4x^3 - 8x = 0$

2. $4x(x^2 - 2) = 0$
$4x(x^2 - 2) = 0$

3. so its roots are $x = 0$, $x = \sqrt{2}$, and $x = -\sqrt{2}$.
所以它的根是 $x = 0$，$x = \sqrt{2}$，和 $x = -\sqrt{2}$。


5.  The second equation has only the solution $y = 0$.
    第二个方程只有$y = 0$这一个解。

4. Therefore our stable points are
因此我们的稳定点是

--- pic\Examples Second partial derivative test.pdf_05.png ---

1. Step 2: Apply second derivative test
    第二步：应用二阶导数检验

32. To start, find all three second partial derivatives of $f(x, y) = x^4 - 4x^2 + y^2$?
    首先，找到函数 $f(x, y) = x^4 - 4x^2 + y^2$? 的所有三个二阶偏导数

1. The expression we care about for the second partial derivative test is
我们关心的二阶偏导数检验的表达式是

--- pic\Examples Second partial derivative test.pdf_06.png ---

1. lf we apply the second derivatives we just found, what does this expression become (as a function of $x$ and $y$ )? 
    如果我们应用刚刚找到的二阶导数，这个表达式会变成什么（作为$x$ 和 $y$ 的函数）？

34. To apply the second derivative test, we plug in each of our stable points to this expression and see if it becomes positive or negative.
    要应用二阶导数检验，我们将每一个稳定点代入这个表达式，看它变成正还是负。

35. Stable point 1:
    稳定点1：

36. At $(x, y) = (0,0)$, the expression evaluates as 
在$(x, y) = (0,0)$时，表达式的值为

1.  This is negative, so according to the second partial derivative test, the point (0,0) is a saddle point.
    这是负的，所以根据二阶导数检验，点(0,0)是一个鞍点。

2.  Stable point 2: At $(x_0, y_0) = (\sqrt{2}, 0)$, the expression becomes
    稳定点2：在$(x_0, y_0) = (\sqrt{2}, 0)$处，表达式变为 

3. This is positive.
   这是正的。

--- pic\Examples Second partial derivative test.pdf_07.png ---

1. Therefore, the point $(\sqrt{2}, 0)$ must be a local minimum.
    因此，点$(\sqrt{2}, 0)$必须是一个局部最小值。

1. Stable point $(-\sqrt{2}, 0)$ : We could plug in the point just as we have with the other stable points, but we could also notice that the function $f ( x , y ) = x^4 − 4 x^2 + y^2$ is symmetric, in the sense that replacing $x$ with $− x$ will yield the same expression:
稳定点 $(-\sqrt{2}, 0)$ : 我们可以像处理其他稳定点一样插入这个点，但我们也可以注意到函数 $f ( x , y ) = x^4 − 4 x^2 + y^2$ 是对称的，意味着将$x$替换为$−x$将得到相同的表达式：

1. Therefore the point $(-\sqrt{2}, 0)$ will have precisely the same behavior as $(\sqrt{2}, 0)$.
因此，点$(-\sqrt{2}, 0)$将具有与$(\sqrt{2}, 0)$完全相同的行为。

3.  Here is a clip of the graph of $f(x, y)$ rotating, where the two local minima are clear, and we can see that the point at the origin is indeed a saddle point.
    这是函数$f(x, y)$的图像旋转的片段，其中两个局部最小值非常明显，我们可以看到原点确实是一个鞍点。

--- pic\Examples Second partial derivative test.pdf_08.png ---

1. Graph with two local minima rotating
    两个局部最小值旋转的图

42. Example 2: Getting more intricate
    示例 2：变得更复杂

43. Let's not sugarcoat things; optimization problems can get long. Very long.
    让我们不要粉饰事实；优化问题可能会很长。非常长。

44. Problem: Find all the stable points (also called critical points) of the function.  
    问题：找出函数的所有稳定点（也叫临界点）。

1. And determine whether each one gives a local maximum, local minimum, or a saddle point.
并确定每一个点是局部最大值、局部最小值还是鞍点。

45. Step 1: Find stable points
    第一步：找稳定点

46. We need to find where both partial derivatives are zero, so start by finding both partial derivatives of $f(x,y)$.
    我们需要找到偏导数都为零的地方，所以首先找到$f(x,y)$的两个偏导数。

--- pic\Examples Second partial derivative test.pdf_09.png ---

1. So we must solve the system of equations
    所以我们必须解这个方程组

48. In the real world, when you come across a system of equations, you should almost certainly use a computer to solve it.
    在现实世界中，当你遇到一个方程组时，你应该几乎肯定使用电脑来解决它。

49. For the sake of practice, though, and to see that optimization problems are not always that simple, let's do something crazy and actually work it out ourselves.
    然而，为了练习，也为了看到优化问题并不总是那么简单，让我们做些疯狂的事情，实际上自己来解决它。

50. In general, the way you might go about this would go something like this: 
    一般来说，你可能会这样做：

51. Solve one equation to get y in terms of x. 
    解一个方程得到y关于x的表达式。
5x. Plug that into the other expression to get an equation with only x. 
    将其代入另一个表达式得到只有x的方程。
53. Solve for x. 
    解出x。
54. Plug each solution for x into both equations and solve for y. 
    将每个解x代入两个方程并求解y。
55. Check which resulting (x, y) pairs actually solve the expression.
    检查哪个结果的(x, y)对实际上解出了表达式。

56. This can be a real mess since you might use the quadratic formula to solve for y treating x as a constant, and plug that nasty expression in elsewhere. 
    这可能会非常混乱，因为你可能会用二次公式解y，将x视为常数，然后将那个讨厌的表达式插入其他地方。

57. Otherwise, you might find yourself solving a degree 4 equation, which aside from being a pain gives quite a few solutions to plug in.
    否则，你可能会发现自己在解一个4阶方程，这除了痛苦之外还给出了相当多的解来代入。

53. In this particular system, the equations feel very symmetric, which is an indication that adding/subtracting them might make things simpler.
    在这个特定的系统中，这些方程感觉很对称，这是一个暗示，添加/减去它们可能会使事情变得更简单。

1. Indeed, if we add them together, we get
确实，如果我们把它们加在一起，我们得到的是

--- pic\Examples Second partial derivative test.pdf_10.png ---
1. What does this equation imply about the relationship between $x$ and $y$? 
    这个等式对 $x$和$y$ 的关系有什么含义？

1. Express each answer as an equation involving the variables $x$ and $y$.
将每个答案表示为涉及变量 $x$和$y$ 的等式。

55. For $(x + y)(x - y - 2) = 0$ to be true, one of the factors $(x + y)$ or $(x - y - 2)$ must be zero, which implies $x+y=0$ or $x-y-2=0$.
    对于 $(x + y)(x - y - 2) = 0$ 为真，因子 $(x + y)$ 或 $(x - y - 2)$ 中的一个必须为零，这就意味着 $x+y=0$ 或者 $x-y-2=0$。

56. Each of these possibilities lets us write x in terms of y, which in turn lets us write one of our equations purely in terms of y.
    这些可能性中的每一种都让我们能够用 y 来表示 x，这反过来又让我们能够纯粹地用 y 来表示我们的一个等式。

57. For example, if you plug in the relation $x = -y$ to the first expression $2xy - y^2 - 2x$, you can get a quadratic expression purely in terms of y.
    例如，如果你将关系 $x = -y$ 代入第一个表达式 $2xy - y^2 - 2x$，你可以得到一个纯粹以 y 为变量的二次表达式。

58. What are the roots of this expression?
    这个表达式的根是什么？
    
1. The roots of this expression are $y = 0$ and $y = \frac{2}{3}$.
这个表达式的根是 $y = 0$ 和 $y = \frac{2}{3}$。

--- pic\Examples Second partial derivative test.pdf_11.png ---

1. Since this arose from assuming x = − y , the corresponding x values are x = − 0 and x = −2/3 respectively.
由于这是由假设x = -y得出的，所以相应的x值分别是x = -0和x = -2/3。

1.  This gives us our first two solution pairs: 
    这给我们提供了前两个解对：

2.  Alternatively, if we consider the case where $x = y + 2$. 
    另一方面，如果我们考虑 $x = y + 2$ 的情况。

1. Again, when we plug this relation into the expression $2xy - y^2 - 2x$, we have a quadratic expression purely in terms of y.
再次，当我们将这个关系代入表达式 $2xy - y^2 - 2x$，我们得到一个纯粹以 y 为变量的二次表达式。

3.  What are the roots of this expression?
    这个表达式的根是什么？

4. Applying the quadratic formula, we have
应用二次公式，我们得到

1. This gives two values of y,
这给出了两个y的值，

--- pic\Examples Second partial derivative test.pdf_12.png ---

1. Because we found these under the assumption that $x = y + 2$, the corresponding values of $x$ are $x=2-1+\sqrt{5}$ and $x=2-1-\sqrt{5}$.
    因为我们在假设 $x = y + 2$ 的情况下找到了这些，所对应的 $x$ 的值是 $x=2-1+\sqrt{5}$ 和 $x=2-1-\sqrt{5}$。

64. This gives two more solution pairs: $(x,y) = (1+\sqrt{5}, -1+\sqrt{5})$ and $(x,y) = (1-\sqrt{5}, -1-\sqrt{5})$.
    这给出了另外两个解对：$(x,y) = (1+\sqrt{5}, -1+\sqrt{5})$ 和 $(x,y) = (1-\sqrt{5}, -1-\sqrt{5})$。

65. We've now exhausted all possibilities since we initially found that either $x= -y$ or $x =y+2$, and we completely solved the equations resulting from each assumption.
    我们现在已经尽可能地找出所有可能，因为我们最初发现 $x= -y$ 或者 $x =y+2$，并且我们完全解决了由每个假设得出的方程。

66. Step 2: Apply second derivative test.
    步骤2：应用二阶导数测试。

67. Man, that was already a lot of work for one example, and we're not even halfway done! 
    天哪，这已经是一个例子的大量工作，我们甚至还没有完成一半！

1. Now we have to apply the second derivative test to each one of these.
现在我们必须对每一个进行二阶导数测试。

1. First, find all of the second derivatives of our function
首先，找出我们函数的所有二阶导数。

--- pic\Examples Second partial derivative test.pdf_13.png ---
1.  According to the second derivative test, to analyze whether each of our stable points is a local maximum or minimum, we plug them into the expression $f_{xx}(x,y) f_{yy}(x,y) - (f_{xy}(x,y))^2$.
    根据二阶导数测试，为了分析我们的每个稳定点是局部最大值还是最小值，我们将它们代入表达式 $f_{xx}(x,y) f_{yy}(x,y) - (f_{xy}(x,y))^2$。

2.  What does this expression become when we apply the second derivatives you just found?
    当我们应用刚刚找到的二阶导数时，这个表达式变为什么？

3.  Since we only care about whether this expression Is positive or negative, we can divide everything by 4 to make things a bit simpler.
    由于我们只关心这个表达式是正还是负，我们可以把所有的东西都除以4，以使事情变得简单一点。

4.  Now we see what the sign of this expression is for each of our stable points.
    现在我们看看这个表达式对于我们每一个稳定点的符号是什么。

1. Stable point  $( 0 , 0 )$  :
稳定点  $( 0 , 0 )$  ：

2. At the point  $( x , y ) = ( 0 , 0 )$  , the key expression above evaluates to 1.
在点  $( x , y ) = ( 0 , 0 )$  ，上述关键表达式的值为1。

3. Plugging  $( 0 , 0 )$  into the expression above, we get $( 0 − 1 ) ( 0 − 1 ) − ( 0 − 0 ) ^2= 1$ 
将  $( 0 , 0 )$  代入上述表达式，我们得到 $( 0 − 1 ) ( 0 − 1 ) − ( 0 − 0 ) ^2= 1$

--- pic\Examples Second partial derivative test.pdf_14.png ---

1. Because this is positive, $(0,0)$ is either a local minimum point or a local maximum point.
    因为这个是正数，$(0,0)$ 或者是局部最小点，或者是局部最大点。

1. To find out which, we look at the sign of $f_{xx}(0,0)$:
为了找出哪一个，我们查看 $f_{xx}(0,0)$ 的符号：

73. From this we conclude that $(0, 0)$ is either a local minimum point or a local maximum point. 
    从这里我们得出结论，(0,0)$ 或者是局部最小点，或者是局部最大点。

74. Now, We evaluate $f_{xx}(0,0) = 2(0) - 2 = -2$, and conclude that f has a local maximum at $(0, 0)$.
    现在，我们求出 $f_{xx}(0,0) = 2(0) - 2 = -2$，并得出 f 在 $(0, 0)$ 有一个局部最大值。

75. Because $-2$ is negative, f has negative concavity at$(-\frac{2}{3},\frac{2}{3})$, so the stable point$(-\frac{2}{3},\frac{2}{3})$ must be a local maximum point.

  因为 $-2$ 是负数，f 在$(-\frac{2}{3},\frac{2}{3})$ 有负的凹度，所以稳定点$(-\frac{2}{3},\frac{2}{3})$ 必须是一个局部最大点。

76. At the point $(x, y) = (-\frac{2}{3},\frac{2}{3})$, the key expression above evaluates to $y = -\frac{15}{9}$.

  在点 $(x, y) = (-\frac{2}{3},\frac{2}{3})$，上面的关键表达式求值为 $y = -\frac{15}{9}$。

77. Plugging  $(-\frac{2}{3},\frac{2}{3})$  into the expression above, we get

将  $(-\frac{2}{3},\frac{2}{3})$  代入上述表达式，我们得到的是

--- pic\Examples Second partial derivative test.pdf_15.png ---

1. From this we conclude that $(-\frac{2}{3},\frac{2}{3})$ is a saddle point.
从这个我们可以得出结论，$(-\frac{2}{3},\frac{2}{3})$ 是一个鞍点。

2. Now, We are done.
现在，我们完成了。

3. Because $-\frac{15}{9}$ is negative, $(-\frac{2}{3},\frac{2}{3})$ is a saddle point. Looking at $f_{xx}$ is unnecessary.
因为 $-\frac{15}{9}$ 是负数，$(-\frac{2}{3},\frac{2}{3})$ 是一个鞍点。查看 $f_{xx}$ 是不必要的。

4. Stable point $(1 + \sqrt{5} , -1 + \sqrt{5})$:
稳定点 $(1 + \sqrt{5} , -1 + \sqrt{5})$：

5. At the point $(x , y) = (1 + \sqrt{5} , -1 + \sqrt{5})$, the key expression above evaluates to -5.
在点 $(x , y) = (1 + \sqrt{5} , -1 + \sqrt{5})$，上述关键表达式的值为 -5。

--- pic\Examples Second partial derivative test.pdf_16.png ---

1. Plugging $(1 + \sqrt{5} , -1 + \sqrt{5})$ into the expression above, we get  -5
将 $(1 + \sqrt{5} , -1 + \sqrt{5})$ 代入上述表达式，我们得到 -5。

2. From this we conclude that $(1 + \sqrt{5} , -1 + \sqrt{5})$ is a saddle point.
由此我们得出，$(1 + \sqrt{5} , -1 + \sqrt{5})$ 是一个鞍点。

3. Now, We are done.
现在，我们完成了。

4. Because − 5 is negative, $(1 + \sqrt{5} , -1 + \sqrt{5})$ is a saddle point.
因为 -5 是负数，所以 $(1 + \sqrt{5} , -1 + \sqrt{5})$ 是一个鞍点。

5. Looking at $f_{xx}$ is unnecessary.
查看 $f_{xx}$ 是不必要的。

6. Stable point $(1 - \sqrt{5} , -1 - \sqrt{5})$
稳定点 $(1 - \sqrt{5} , -1 - \sqrt{5})$

7. The arithmetic here is almost identical to the previous case.
这里的算术几乎与前一种情况相同。

--- pic\Examples Second partial derivative test.pdf_17.png ---
1.  In a deep sense, this is not just similar to the previous case, but equivalent.
    在深层意义上，这不仅与前一种情况相似，而且等同。

2.  This is because our function $f$ has a certain symmetry, namely  
    这是因为我们的函数$f$有一定的对称性，即 

3.  Try it yourself to see why! 
    试试看为什么！

1. Applying the operation $(x, y) \rarr (-y, -x)$ to the third stable point $(1 + \sqrt{5}, -1 + \sqrt{5})$ gives the fourth stable point $(1 - \sqrt{5}, -1 - \sqrt{5})$, so the behavior of the function at both of these points should be identical.
将操作$(x, y) \rarr (-y, -x)$应用到第三个稳定点$(1 + \sqrt{5}, -1 + \sqrt{5})$，我们得到第四个稳定点$(1 - \sqrt{5}, -1 - \sqrt{5})$，因此这两点处的函数行为应该是相同的。

1.  The symmetry of this function is very visible in the graph pictured below. 
    这个函数的对称性在下面的图中非常明显。

2.  Rotating graph of graph with four Gritical points.
具有四个关键点的图形的旋转图。

2. Here is a short clip of the graph of $f ( x , y ) = x^2 y − y^2 x − x^2 − y^2$ rotating, where you can see the three saddle points and the one local maximum at the origin.
这是函数$f ( x , y ) = x^2 y − y^2 x − x^2 − y^2$的图形旋转的短片段，你可以看到三个鞍点和原点处的一个局部最大值。

1.  Pat yourself on the back.
    对自己表示赞赏。

2.  These are long problems, so if you actually worked through them, give yourself some hearty congratulations!
    这些都是长篇的问题，如果你真的解决了它们，那么给你自己热烈的祝贺！

