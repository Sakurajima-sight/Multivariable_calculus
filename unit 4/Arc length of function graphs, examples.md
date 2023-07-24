
--- pic\Arc length of function graphs, examples.pdf_00.png ---

1. Arc length of function graphs, examples
   函数图形的弧长，示例

2. Practice finding the arc length of various function graphs.
   练习寻找各种函数图形的弧长。

3. Background
   背景

4. Arc length of function graphs, introduction
   函数图形的弧长，简介

5. Example 1: Practice with a semicircle
   示例1：用半圆做练习

6. Consider a semicircle of radius 1, centered at the origin, as pictured on the right.
   考虑一个半径为1、以原点为中心的半圆，如右图所示。

7. From geometry, we know that the length of this curve is $\pi$.
   从几何学中，我们知道这条曲线的长度是$\pi$。

8. Let's practice our newfound method of computing arc length to rediscover the length of a semicircle.
   让我们练习我们新发现的计算弧长的方法，以重新发现半圆的长度。

9.  By definition, all points $(x, y)$ on the circle are a distance 1 from the origin, so we have
    根据定义，圆上的所有点$(x, y)$与原点的距离为1，所以我们有

10. Rearranging to write $y$ as a function of $x$, we have
    重新排列，将$y$写成$x$的函数，我们得到

11. As you set up the arc length integral, it helps to imagine approximating this curve with a bunch of small lines.
    当你设定弧长积分时，想象用一堆小线来近似这条曲线会有所帮助。

--- pic\Arc length of function graphs, examples.pdf_01.png ---

1. Writing down the arc-length integral, ignoring the bounds for just a moment, we get:
    写下弧长积分，暂时忽略边界，我们得到：

1. Just as before, we think of the integrand  $\sqrt{(dx)^2+(dy)^2}$ as representing the length of one of these little lines approximating the curve (via the Pythagorean theorem).
正如之前一样，我们将积分函数 $\sqrt{(dx)^2+(dy)^2}$ 视为表示这些近似曲线的小线段的长度（通过勾股定理）。

3.  Now we start plugging in the definition of our particular curve into the integral.
    现在我们开始将我们特定曲线的定义代入到积分中。

--- pic\Arc length of function graphs, examples.pdf_02.png ---

1. Step 1: Write $dy$ in terms of $dx$
    步骤1：将$dy$写成$dx$的形式

2. Use the fact that $y = \sqrt{1 - x^2}$ to write $dy$ in terms of $dx$.
使用事实 $y = \sqrt{1 - x^2}$ 将 $dy$ 表示为 $dx$ 的函数。

2. We take the derivative of both sides of the equation $y = \sqrt{1 - x^2}$, using the chain rule for the right side:
我们对等式 $y = \sqrt{1 - x^2}$ 的两边取导数，对右侧使用链式法则：

19. We take the derivative of both sides of the equation $y = 1 - x^2$.
    我们对等式$y = 1 - x^2$的两边取导数。

20. Step 2: Replace $dy$ in the integral
    步骤2：在积分中替换$dy$

21. Plug this expression for $dy$ into the integral to write the integrand completely in terms of $x$ and $dx$.
    将这个表示$dy$的表达式代入积分，以便将被积函数完全写成$x$和$dx$的形式。

--- pic\Arc length of function graphs, examples.pdf_03.png ---

1. Step 3: Place bounds on the integral and solve
    步骤3：放置积分的边界并解决

24. Since the curve is defined between when $x = -1$ and $x = 1$, set these values as the bounds of your integral and solve it.
    由于曲线在$x = -1$和$x = 1$之间定义，将这些值设置为你的积分的边界并解决它。

25. Sorry, no entry box with a happy green checkmark. 
    抱歉，没有带有绿色勾选标记的输入框。

1. We know from geometry that the arc length is $\pi$, but the interesting part is to work through it to see how $\pi$ pops out when using an arc length integral.
我们从几何知道弧长是$\pi$，但有趣的部分是通过计算看到在使用弧长积分时$\pi$如何突显出来。

26. Our integral looks like this: 
    我们的积分看起来像这样：

27. Now, there are a few ways you might proceed from here.
    现在，你可以从这里开始尝试几种方法。

28. Plug this integral into a calculator or computer algebra system and watch the answer pop out.
    将这个积分输入计算器或计算机代数系统，看答案如何弹出。

29. Somehow remember or recognize that this integral is $\arcsin(x)$.
    以某种方式记住或识别出这个积分就是$\arcsin(x)$。

30. Solve the integral using trigonometric substitution.
    使用三角函数代换来解积分。

31. All of these are valid, but the interesting one to focus on is the trigonometric substitution.
    所有这些都是有效的，但值得关注的是三角函数代换。

32. Rather than just plugging and chugging, I want to shed some light on what this substitution actually means geometrically.
    而不仅仅是代入和计算，我想阐明这种代换在几何上实际上是什么意思。

1. Hopefully, this makes clear how and why this technique works, which will help you recognize whether or not such a substitution will work in other integrals that you might encounter.
    希望这能清楚地解释这种技术的工作原理以及为什么它能工作，这将帮助你判断这种替换是否适用于你可能遇到的其他积分。

--- pic\Arc length of function graphs, examples.pdf_04.png ---

1. What does it mean that our integral is currently written in terms of $x$? 
    我们的积分目前以$x$为参数是什么意思呢？

1. It basically has you walking along the x-axis, from $-1$ to $1$, measuring the snippet of arc length on the circle above your head as you go.
它基本上让你沿着$x$轴从$-1$走到$1$，并在行进过程中测量你头顶上圆的一段弧长。

34. However, in this case, it might be natural to imagine walking along the circle itself.
    然而，在这种情况下，你可能会自然地想象沿着圆自身行走。

35. Each point of the circle can be described with a value of the angle $\theta$, ranging from $0$ to $\pi$.
    圆的每一点都可以用角度$\theta$的值来描述，范围从$0$到$\pi$。

36. Moreover, since the radius is $1$, the value of $\theta$ measured in radians actually reflects arc length.
    而且，由于半径为$1$，以弧度计算的$\theta$值实际上反映了弧长。

37. A tiny change $d\theta$ will correspond with a tiny change in arc length.
    一个微小的变化$d\theta$将对应一个微小的弧长变化。

38. Therefore, it should seem reasonable that an alternative integral describing the desired arc length is $\int_0^\pi d\theta$.
    因此，一个合理的描述所需弧长的替代积分应该是$\int_0^\pi d\theta$。

39. In a sense, we're done. It's easy to see that this integral evaluates to $\pi$, which is indeed the arc length of our semi-circle.
    从某种意义上说，我们已经完成了。可以轻易看出，这个积分的结果是$\pi$，这确实是我们半圆的弧长。

40. But what's the relationship between this and our previous integral?
    但这个和我们之前的积分有什么关系呢？

1. Since the $x$ value of any point on the circle is $x = -\cos(\theta)$, this suggests that substituting $-\cos(\theta)$ for $x$ will simplify our integral. 
由于圆上任意点的 $x$ 值为 $x = -\cos(\theta)$，这表明将 $-\cos(\theta)$ 替换为 $x$ 将简化我们的积分。

--- pic\Arc length of function graphs, examples.pdf_05.png ---

1. Let's actually walk through that process.
   让我们实际走过这个过程。

2. When we apply this substitution, we have to do three things.
   当我们应用这种替代时，我们需要做三件事。

3. Step 1: Replace $x$ with $-\cos(\theta)$.
   第一步：用$-\cos(\theta)$替换$x$。

4. Step 2: Replace $dx$ with $d(-\cos(\theta)) = \sin(\theta) d\theta$.
   第二步：将$dx$替换为$d(-\cos(\theta)) = \sin(\theta) d\theta$。

5. Step 3: Write the integral's limits $x = -1$ and $x = 1$ in terms of $\theta$.
   第三步：将积分的限制$x = -1$和$x = 1$写成$\theta$的形式。

6. The relation $x = -1$ translates to the relation $-\cos(\theta) = -1$.
   $x = -1$的关系转化为$-\cos(\theta) = -1$的关系。

7. This happens when $\theta = 0$.
   这在$\theta = 0$时发生。

8. The relation $x = 1$ translates to the relation $-\cos(\theta) = 1$.
   $x = 1$的关系转化为$-\cos(\theta) = 1$的关系。

9. This happens when $\theta = \pi$.
   这在$\theta = \pi$时发生。

10. Applying all of these exchanges, we get to 
    应用所有这些交换，我们得到

1. Simplifying, using the identity $\sin^2(\theta) + \cos^2(\theta) = 1$, this becomes
简化，使用恒等式 $\sin^2(\theta) + \cos^2(\theta) = 1$，我们得到

11. Simplifying, using the identity $\sin^2(\theta) + \cos^2(\theta) = 1$, we get $\int |\sin^2(\theta) \sin(\theta)d\theta$.
    简化，使用恒等式$\sin^2(\theta) + \cos^2(\theta) = 1$，我们得到$\int |\sin^2(\theta) \sin(\theta)d\theta$。

12. So yes, trigonometric substitution greatly simplifies our integral, but it's not just magic.
    所以，三角函数代换大大简化了我们的积分，但这并不仅仅是魔术。

13. The reason it makes things simpler is that the curve is more naturally described with the value $\theta$ shown in the diagram above.
    它使事情变得更简单的原因是，曲线用上图中显示的$\theta$值更自然地描述。

2. Practice setting up arc length integrals
练习设置弧长积分


--- pic\Arc length of function graphs, examples.pdf_06.png ---

1.  The actual integral you get for arc length is often difficult to compute.
    你得到的实际弧长的积分通常难以计算。

2.  However, the important skill to practice is setting up that integral.
    然而，需要练习的重要技巧是设置那个积分。

3.  So let's practice that a few times without worrying about computing the final integral (you can use a calculator or Wolfram Alpha once you get a concrete integral).
    所以，让我们练习几次，不用担心计算最后的积分（一旦你得到一个具体的积分，你就可以使用计算器或Wolfram Alpha）。

4.  Example 2: Sine curve.
    例2：正弦曲线。

5.  What integral represents the arc length of the graph of $y = \sin(x)$ between $x = 0$ and $x = 2\pi$?
    在$x = 0$和$x = 2\pi$之间，什么积分代表了$y = \sin(x)$图的弧长？

--- pic\Arc length of function graphs, examples.pdf_07.png ---
1. As always, the integral starts its life looking like this:
    像往常一样，积分从这样开始：

1.  Step 1: Write $dy$ in terms of $dx$. 
    第一步：用$dx$表示$dy$。
    
2.  I think it's enlightening to remind yourself of what this means, beyond just throwing the symbol $d$ in front of everything.
    我认为，提醒自己这意味着什么，不仅仅是在所有东西前面加上符号$d$，是很有启发性的。

3.  If you are sitting at a point $(x, y)$ on the curve, and you take a tiny step $dx$ to the right, the amount you must step up to end up back on the curve happens to be $\cos(x) dx$.
    如果你坐在曲线上的一个点$(x, y)$，然后你向右走一小步$dx$，你必须向上走的距离才能回到曲线上，刚好是$\cos(x) dx$。

4.  Step 2: Plug this value of $dy$ into the integral.
    第二步：将$dy$的这个值插入积分。

5.  Step 3: Put bounds on the integral.
    第三步：在积分上设置界限。

6.  In this case, the problem explicitly states that $x$ runs from $0$ to $2\pi$.
    在这个案例中，问题明确指出$x$从$0$运行到$2\pi$。

1. Example 3: Up, not right
示例3：向上，而不是向右

--- pic\Arc length of function graphs, examples.pdf_08.png ---

1. Consider the curve representing  
    考虑曲线

1. For all values where $x \leq 4$.
其中$x \leq 4$。

1. Find an integral expressing this curve's arc length.
    找到一个表示这个曲线弧长的积分。

2. But this time, write everything in the integral in terms of $y$, not $x$.
    但这次，把积分中的所有东西都用$y$表示，而不是$x$。

--- pic\Arc length of function graphs, examples.pdf_09.png ---

1. Unlike all examples up to this point, the curve is not the graph of a single function of $x$. 
    与此前所有的例子不同，这个曲线不是$x$的单一函数的图像。

1. Instead, it involves two separate functions:
相反，它涉及到两个独立的函数：

2. However, it is the graph of a function of $y$ with respect to $x$: $x = y^2$
    然而，它是一个关于$y$对$x$的函数的图像：$x = y^2$

3. So rather than constructing two separate integrals in terms of $dx$, each of which could be thought of as a rightward walk along the graph, we construct a single integral with respect to $dy$, which can be thought of as walk along the curve from bottom to top.
    所以，我们不是构造两个以$dx$为单位的单独积分，每个都可以被认为是沿图形向右走，而是构造一个以$dy$为单位的单独积分，可以被认为是从底部向顶部沿曲线走。

4. The steps to setting up this integral are nearly identical to everything we've done up to this point, but pay careful attention to how we are now writing all expressions with $x$ in terms of $y$, rather than vice versa.
    设置这个积分的步骤几乎与我们至今为止所做的一切相同，但请特别注意我们现在如何将所有与$x$有关的表达式写成以$y$为单位，而不是反过来。

5. Step 1: Write $dx$ in terms of $dy$
    步骤1：将$dx$写成$dy$的形式

6. Step 2: Plug this value of $dx$ into the integral
    步骤2：将$dx$的这个值代入积分中

7.  Step 3: Place bounds on the integral
    步骤3：对积分设定边界

8.  This time, everything in the integral is in terms of $y$, so the bounds must reflect $y$ values.
    这次，积分中的所有内容都是以$y$为单位的，所以边界必须反映$y$的值。

--- pic\Arc length of function graphs, examples.pdf_10.png ---

1. Looking at the graph above, we see that the end points of the curve which correspond with $x = 4$ have y values $y = -2$ and $y = 2$.
    观察上图，我们看到对应$x = 4$的曲线的端点有$y$值 $y = -2$ 和 $y = 2$。

2.   The fundamental reason for writing things in terms of $y$ instead of $x$ is that It's easier to think of moving along this curve from bottom to top, rather than from left to right.
     以$y$而不是$x$来写作的基本原因是，我们更容易想象沿着这条曲线从下到上移动，而不是从左到右。

3.  In general, and this is an important principle to remember, when you are integrating along a curve, the formulas and symbols you use should reflect how you would actually walk along the curve.
    一般来说，这是一个重要的原则需要记住，当你沿着一个曲线进行积分时，你使用的公式和符号应该反映你实际上如何沿着曲线行走。

4.  Example 4: Full generality 
    示例4：完全一般性 

1. Suppose you have any arbitrary function $f(x)$, with derivative $f'(x)$. 
假设你有任意函数$f(x)$，其导数为$f'(x)$。


1. Which of the following represents the arc length of the graph $y = f(x)$ between the points $x = a$ and $x = b$?
下面哪一个代表了点$x = a$ 和 $x = b$ 之间的图形$y = f(x)$的弧长？

--- pic\Arc length of function graphs, examples.pdf_11.png ---

1.  Step 1: Write $dy$ in terms of $dx$
    步骤1：将$dy$写成$dx$的形式

2.  Step 2: Plug this expression for $dy$ into the arc length integral
    步骤2：将$dy$的这个表达式代入弧长积分中

3.  Step 3: Put bounds on the integral. 
    步骤3：对积分设置边界。

1. These are given explicitly, albeit abstractly, as $x = a$ and $x = b$.
这些边界被明确给出，尽管是抽象地，$x = a$ 和 $x = b$。

--- pic\Arc length of function graphs, examples.pdf_12.png ---

1. Oftentimes people will start teaching arc length by presenting this formula. 
    通常人们会开始教弧长，通过提出这个公式。

1. Personally, I think that takes all the fun out of discovering it yourself and getting a genuine feel for what it really represents.
个人认为，这就失去了自己发现它和真正理解它代表什么的乐趣。

21. We use the words arc length to describe how long a curve is. 
    我们用弧长这个词来描述曲线有多长。

1. If you imagine the curve as a string, this is the length of that string once you pull it taut.
如果你把曲线想象成一个线条，那么这就是你拉直这个线条后的长度。

22. You can find the arc length of a curve with an integral of the form $\int \sqrt{(dx)^2 + (dy)^2}$
    你可以通过一个形如$\int \sqrt{(dx)^2 + (dy)^2}$的积分来找到曲线的弧长

23. If the curve is the graph of a function $y = f(x)$, replace the $dy$ term in the integral with $f'(x)dx$, then factor out the $dx$.
    如果曲线是函数$y = f(x)$的图，那么在积分中用$f'(x)dx$替换$dy$，然后提取出$dx$。

24. The boundary values of the integral will be the leftmost and rightmost $x$-values of the curve.
    积分的边界值将是曲线的最左和最右的$x$值。

25. When setting up an arc length integral, it helps to think about how you would actually choose to walk along the curve.
    在设置弧长积分时，考虑你实际上如何选择沿曲线行走会有所帮助。