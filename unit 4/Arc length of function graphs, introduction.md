
--- pic\Arc length of function graphs, introduction.pdf_00.png ---

1. Arc length of function graphs, introduction
    函数图的弧长介绍

2. The length of a curve, called its "arc length", can be found using a certain integral.
    曲线的长度，被称为“弧长”，可以使用某个积分来找到。

3. Background
    背景

4. Ordinary integrals
 普通积分

1. What Is arc length? 
   圆的周长

1. Circumference of a circle
    什么是弧长？

2. We usually measure length with a straight line, but curves have length too.
    我们通常用直线测量长度，但曲线也有长度。

3. A familiar example is the circumference of a circle, which has length $2\pi r$ for radius $r$.
    熟悉的例子是圆的周长，对于半径$r$，它的长度为$2\pi r$。

4. In general, the length of a curve is called the arc length.
    一般来说，曲线的长度被称为弧长。

5.  But how do you find the arc length of an arbitrary curve? Let's find out.
    但是你如何找到任意曲线的弧长呢？让我们找出答案。

6.  What we're building to
    我们正在构建什么

7.  You can find the arc length of a curve with an integral that looks something like this:
    你可以找到一个积分来计算曲线的弧长，它看起来像这样：

8.  The bounds of this integral depend on how you define the curve.
    这个积分的边界取决于你如何定义曲线。

9.  If the curve is the graph of a function $y = f(x)$, replace the $dy$ term in the integral with $f'(x)dx$, then factor out the $dx$.
    如果曲线是函数$y = f(x)$的图，那么在积分中用$f'(x)dx$替换$dy$项，然后提取出$dx$。

--- pic\Arc length of function graphs, introduction.pdf_01.png ---

1. Warmup: Approximating arc length
    热身：近似弧长

16. Let's look at the parabola defined by the following equation:
    让我们看看由下列等式定义的抛物线：

17. $y=f(x)=x^2$
    $y=f(x)=x^2$

18. Consider the portion of the curve between $x = -2$ and $x = 2$.
    考虑曲线在$x = -2$和$x = 2$之间的部分。

19. Key question: What is the arc length of this curve?
    关键问题：这条曲线的弧长是多少？

20. Just so the question is clear, imagine the curve was a piece of string.
    为了明确问题，想象曲线是一根绳子。

21. You pull this string straight and measure it with a ruler.
    你拉直这根绳子，用尺子测量它。

--- pic\Arc length of function graphs, introduction.pdf_02.png ---
1. If you had to guess, you could start by approximating this curve with some lines.
如果你需要猜测，你可以开始用一些线来近似这个曲线

1. Here's how that might look:
    下面是可能的样子：

2. A line from $(-2, 4)$ to $(-1, 1)$
一条从$(-2, 4)$到$(-1, 1)$的线。

3. A line from $(-1, 1)$ to $(0, 0)$
一条从$(-1, 1)$到$(0, 0)$的线。

4. A line from $(0, 0)$ to $(1, 1)$
一条从$(0, 0)$到$(1, 1)$的线。

5. A line from $(1, 1)$ to $(2, 4)$
一条从$(1, 1)$到$(2, 4)$的线。

23. It would be tedious, but you could calculate the length of each line segment using the Pythagorean theorem, then add them up.
    这会很繁琐，但你可以使用勾股定理计算每个线段的长度，然后将它们加起来。

24. Concept check: What is the length of the line from $(-2, 4)$ to $(-1,1)$?
    概念检查：从$(-2, 4)$到$(-1,1)$的线的长度是多少？

--- pic\Arc length of function graphs, introduction.pdf_03.png ---

1. Consider the triangle pictured here:
    考虑这里描绘的三角形：

26. The hypotenuse is the line whose length we wish to calculate.
    斜边是我们希望计算长度的线。

27. One leg is parallel to the $x$-axis and has length $-1 -(-2) =1$, and the other leg is parallel to the $y$-axis and has length $4-1=3$.
    一条腿平行于$x$轴，长度为$-1 -(-2) =1$，另一条腿平行于$y$轴，长度为$4-1=3$。

28. The length of the hypotenuse is therefore $\sqrt{1^2 + 3^2} = \sqrt{10}$.
    因此，斜边的长度为$\sqrt{1^2 + 3^2} = \sqrt{10}$。

29. For an even more accurate estimate, you could approximate the curve with many tiny lines.
    为了得到更准确的估计，你可以用许多小线段近似曲线。

--- pic\Arc length of function graphs, introduction.pdf_04.png ---

1. Computing all their lengths and adding them up would be painfully mind-numbing, but let's break down what it would actually look like.
    计算所有线段的长度并把它们加起来将非常枯燥乏味，但是让我们详细说明它实际上会是什么样子。

31. Zoom in on one of the little lines.
    放大查看其中一条小线。

32. First look at the change in the $x$ value from the start of the line to its end. 
    首先看看从线的开始到结束$x$值的变化。

1. Let's call that $\Delta x$.
我们称之为$\Delta x$。

33. Similarly, let's say the change in the $y$-value is $\Delta y$.
    同样，我们说$y$值的变化是$\Delta y$。

34. Then, using the Pythagorean theorem, we can write the length of the line as $\sqrt{(\Delta x)^2 + (\Delta y)^2}$.
    然后，使用勾股定理，我们可以将线的长度写为$\sqrt{(\Delta x)^2 + (\Delta y)^2}$。

35. Our approximation for the length of the curve will then be the sum of the lengths of all these little lines.
    我们对曲线长度的近似值将是所有这些小线的长度之和。

1. When expressing an idea like this with symbols, it's common for writers to be a little loose with the notation and write something like this:
当用符号表达这样的想法时，作者通常会对记号稍微宽松一些，写出如下的东西：

--- pic\Arc length of function graphs, introduction.pdf_05.png ---

1. You might be used to reading sums like this:
    你可能习惯于读这样的和：

2. The variable $n$ is what's known as an indexing variable.
    变量$n$被称为索引变量。

3. This indexing variable has a specified range, in this case from 1 to 100.
    这个索引变量有一个指定的范围，在这种情况下从1到100。

1. The portion inside the sum, in this case $n^2$, is called the summand, and it is written in terms of $n$.
在这种情况下，求和内的部分，即 $n^2$，被称为求和项，它是以 $n$ 的形式写的。

1. In comparison, the sum I wrote to approximate the length of the parabola is not at all rigorous.
    相比之下，我写的用于近似抛物线长度的和一点都不严谨。

2. It has no indexing variable.
   它没有索引变量。

3. There is no specified range.
    没有指定的范围。

4. The summand certainly isn't written in terms of an indexing variable (since there isn't one).
    这个加数肯定不是以索引变量（因为没有）的形式写的。

5.  Out of laziness, it is left to you, the intelligent human reader, to understand it in context.
    出于懒惰，这被留给你，聪明的人类读者，以理解其上下文。

6.  Namely, in the context of our discussion, there were many tiny lines approximating the parabola, so I put the words “all little lines" under the $\Sigma$.
    即在我们的讨论中，有许多小线在近似抛物线，所以我在$\Sigma$下面写上了“所有的小线”。

7.  It should also be understood that the value of the summand $\sqrt{(\Delta x)^2 + (\Delta y)^2}$.
    还应该理解加数的值是 $\sqrt{(\Delta x)^2 + (\Delta y)^2}$。

8.  Also, the expressions $\Delta x$ and $\Delta y$ are not given using formulas, but were instead defined using English words from the paragraphs preceding.
    此外，$\Delta x$和$\Delta y$的表达式并没有使用公式给出，而是使用前面段落的英语单词定义的。

9.  It is important to be able to read loose notation like this and understand what it means.
    能够阅读这样的松散记号并理解其含义是很重要的。

10. Throughout multivariable calculus, something very similar happens with how integrals are written, where the terms and bounds reference the context of a discussion.
    在多元微积分中，类似的情况发生在积分的写法上，其中的项和边界引用了讨论的上下文。

11. In fact, you're about to see one such example in the next section.
    实际上，你将在下一节看到这样的一个例子。

12. Writers use loose notation like this when the key takeaway point is a broader conceptual idea, not a specific computation.
    当关键要点是更广泛的概念性想法，而不是特定的计算时，作者会使用这样的松散记号。

13. When the time comes to do a computation, though, this kind of notation gets tightened up into something rigorously defined.
    然而，当到了进行计算的时候，这种记号就会被严格定义。

--- pic\Arc length of function graphs, introduction.pdf_06.png ---

1. Bringing in integrals
    引入积分

20. Hmm, let's see.
    嗯，让我们看看。

21. With tinier steps and a larger sum, we will get a better approximation.
    如果步子更小，和更大，我们将得到更好的近似值。

22. Sound familiar?
    听起来熟悉吗？

23. Problems like this one are exactly what integrals were made for.
    这类问题正是积分的用途。

24. Most people first learn about integration in the context of computing the area under a curve.
    大多数人首次学习积分是在计算曲线下面积的上下文中。

25. You imagine approximating that area with a bunch of thin rectangles.
    你可以想象用一堆细长的矩形来近似那个面积。

26. The width of each one is thought of as $\mathrm{d}x$, some tiny change in the $x$-value.
    每个的宽度被认为是"$\mathrm{d}x$"，是$x$值的一些微小变化。

27. The height of a rectangle at a given $x$-value is $f(x)$.
    在给定$x$值的矩形的高度是$f(x)$。

28. Therefore, the area of each rectangle is $f(x)dx$.
    因此，每个矩形的面积是 $f(x)dx$。

29. The full area under the curve is then expressed with an integral: 
    然后，曲线下的全部面积用积分表示为：

30. This integral is a powerful machine, like a $\Sigma$ on steroids.
    这个积分是一个强大的机器，就像打了类固醇的$\Sigma$。

31. It does not merely sum over the values $f(x)\mathrm{d}x$ for a particular tiny value of $\mathrm{d}x$; it considers the limiting value of such a sum as the tiny width $\mathrm{d}x$ tends toward 0.
它不仅仅是对特定的微小$\mathrm{d}x$值的$f(x)\mathrm{d}x$求和，而是考虑当微小宽度$\mathrm{d}x$趋近于0时这种和的极限值。

32. In other words, as the approximation using rectangles comes closer and closer to the true area under the curve.
    换句话说，当使用矩形的近似值越来越接近曲线下的真实面积。

33. But this powerful machine can be used in many contexts unrelated to the area under a curve.
    但是这个强大的机器可以在许多与曲线下面积无关的上下文中使用。

34. Anytime you get that sensation of wanting to add a very large number of very small things, the integral swoops in to simultaneously make things less tedious and more accurate.
    任何时候，你只要有想要加上非常大数量的非常小的东西的感觉，积分就会立即让事情变得不那么繁琐而更准确。


--- pic\Arc length of function graphs, introduction.pdf_07.png ---

1. For example, we get that sensation when approximating arc length with the vague sum:
   例如，当我们用模糊的总和近似弧长时，我们会有这种感觉：

2. So we turn it into an integral:
   所以我们将它转化为积分：

3. One thing this notation does not communicate well is that $\mathrm{d}y$, the change in height across one of our little approximation lines, is dependent on $\mathrm{d}x$, the horizontal component of that line.
   这种表示法没有很好地传达的一点是，$\mathrm{d}y$，即我们的小近似线在高度上的变化，依赖于$\mathrm{d}x$，即该线的水平分量。

4. Specifically, since the curve is defined by the relation $y = x^2$, we can take the derivative of each side to see how $\mathrm{d}y$ depends on $\mathrm{d}x$,
   具体来说，因为曲线由关系$y = x^2$定义，我们可以对每一边取导数，看看$\mathrm{d}y$如何依赖于$\mathrm{d}x$，

5. If this is very strange, consider reviewing implicit differentiation.
如果这很奇怪，可以考虑复习隐函数微分。

1. If you prefer, you can imagine taking the $\frac{d}{dx}$-style derivative of each side, then rearranging the "fraction" $\frac{dy}{dx}$.
如果你愿意，你可以想象对每一边取$\frac{d}{dx}$形式的导数，然后重新排列"分数" $\frac{dy}{dx}$。

1. When we put this into our integral, it unfolds to look a bit more familiar.
当我们将这个放入我们的积分中，它展开后看起来会更熟悉一些。


--- pic\Arc length of function graphs, introduction.pdf_08.png ---

1. I've been purposefully lazy about placing bounds on this integral, but now that everything inside the integral is in terms of $x$, with no $\mathrm{d}y$'s mucking it up, it makes sense to define the bounds of integration in terms of the $x$ value, which in this case is from $-2$ to $2$.
    我一直故意在给这个积分定界限上偷懒，但现在积分内的所有东西都是用$x$表示的，没有$\mathrm{d}y$来搞乱它，所以用$x$值来定义积分的界限是有意义的，在这个例子中，$x$值从$-2$到$2$。

2. This looks like something we can compute.
    这看起来像是我们可以计算的东西。

3. Well, actually, in this case, it turns out to be quite a tricky integral, but in this day and age, we can just plug integrals into a computer if we need to.
   实际上，在这种情况下，这是一个相当棘手的积分，但在这个时代，如果我们需要的话，我们只需要把积分输入电脑就可以了。

4. The point is that the idea of approximating our curve's length with little lines, which was at first vaguely written with loose notation, has now turned into a concrete, computable integral.
   关键是，我们用小线来近似曲线长度的想法，最初是以宽松的符号模糊地写出来的，现在已经变成了一个具体的、可以计算的积分。

5. For now, rather than getting bogged down with the details of this integral (there's plenty of that coming in the next article), I want to highlight some points from this example.
   现在，我并不想深陷在这个积分的细节中（在下一篇文章中会有很多），我想强调一下这个例子的一些要点。

6. Takeaways
   重要的收获

1. The central expression to remember is $\sqrt{dx^2 + dy^2}$, which represents a tiny unit of arc length in terms of $x$ and $y$.
需要记住的核心表达式是 $\sqrt{dx^2 + dy^2}$，它用 $x$ 和 $y$ 表示了一小段弧长。

8. The arc length integral you set up starts its life looking like this: 
   你设定的弧长积分开始时就像这样：

9.  Before computing the integral, we had to write the differential $\mathrm{d}y$ in terms of the differential $\mathrm{d}x$. 
   在计算积分之前，我们必须将微分$\mathrm{d}y$写成微分$\mathrm{d}x$的形式。

1. To do this, we took the derivative of the function defining the curve.
为了做到这一点，我们取了定义曲线的函数的导数。

10. In general, an integral can only be computed with respect to a single differential, and finding relations between differentials can be done using the derivative.
   一般来说，一个积分只能相对于一个微分来计算，而找到微分之间的关系可以通过求导来完成。

11. Maybe the most important lesson to take away from this is that integrals can be used to do things other than finding the area under a curve.
   或许从这里得到的最重要的教训是，积分可以用来做一些除了找曲线下面积之外的事情。

--- pic\Arc length of function graphs, introduction.pdf_09.png ---

24. To solidify your understanding, you can practice more arc length problems in the next article.
    为了加固你的理解，你可以在下一篇文章中做更多的弧长问题练习。